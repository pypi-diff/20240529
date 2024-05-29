# Comparing `tmp/refvars-0.6-py3-none-any.whl.zip` & `tmp/refvars-0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,11 @@
-Zip file size: 12449 bytes, number of entries: 6
--rw-r--r--  2.0 unx     3157 b- defN 24-Apr-12 03:53 refvars/__init__.py
--rw-r--r--  2.0 unx    25171 b- defN 24-Apr-12 05:23 refvars-0.6.dist-info/LICENCE
--rw-r--r--  2.0 unx     2322 b- defN 24-Apr-12 05:23 refvars-0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 05:23 refvars-0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-12 05:23 refvars-0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      452 b- defN 24-Apr-12 05:23 refvars-0.6.dist-info/RECORD
-6 files, 31202 bytes uncompressed, 11635 bytes compressed:  62.7%
+Zip file size: 88506 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      502 b- defN 24-Mar-14 11:13 reference/__init__.py
+-rw-rw-rw-  2.0 fat     8565 b- defN 24-May-29 06:05 refvars/__init__.py
+-rw-rw-rw-  2.0 fat     1920 b- defN 24-May-28 15:10 refvars/mem_win_x86.py
+-rw-rw-rw-  2.0 fat   138752 b- defN 24-May-28 15:10 refvars/mem_win_x86_lib.dll
+-rw-rw-rw-  2.0 fat    25652 b- defN 24-May-29 06:57 refvars-0.7.dist-info/LICENCE
+-rw-rw-rw-  2.0 fat     3701 b- defN 24-May-29 06:57 refvars-0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-29 06:57 refvars-0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-29 06:57 refvars-0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      694 b- defN 24-May-29 06:57 refvars-0.7.dist-info/RECORD
+9 files, 179886 bytes uncompressed, 87324 bytes compressed:  51.5%
```

## zipnote {}

```diff
@@ -1,19 +1,28 @@
+Filename: reference/__init__.py
+Comment: 
+
 Filename: refvars/__init__.py
 Comment: 
 
-Filename: refvars-0.6.dist-info/LICENCE
+Filename: refvars/mem_win_x86.py
+Comment: 
+
+Filename: refvars/mem_win_x86_lib.dll
+Comment: 
+
+Filename: refvars-0.7.dist-info/LICENCE
 Comment: 
 
-Filename: refvars-0.6.dist-info/METADATA
+Filename: refvars-0.7.dist-info/METADATA
 Comment: 
 
-Filename: refvars-0.6.dist-info/WHEEL
+Filename: refvars-0.7.dist-info/WHEEL
 Comment: 
 
-Filename: refvars-0.6.dist-info/top_level.txt
+Filename: refvars-0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: refvars-0.6.dist-info/RECORD
+Filename: refvars-0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## refvars/__init__.py

```diff
@@ -1,90 +1,228 @@
-from typing import Any, Generic, TypeVar
-import inspect
-
-
-
-T_PYTHON_REFERENCE = TypeVar('T_PYTHON_REFERENCE')
-_REF_VARS_SPECIAL_SAUCE = False
-
-
-
-class Reference_Instance (Generic[T_PYTHON_REFERENCE]):
-	def __init__(self, type_:"str", value_:"T_PYTHON_REFERENCE"):
-		global _REF_VARS_SPECIAL_SAUCE
-		if _REF_VARS_SPECIAL_SAUCE == True:
-			self.type = type_
-			self.value = value_
-		else:
-			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
-			err_msg += f"Do not instantiate the class `ReferenceInstance` directly.\n"
-			err_msg += f"Instead, use the class `Make_Reference`.\n"
-			raise SyntaxError(err_msg)
-
-	def get(self) -> "T_PYTHON_REFERENCE":
-		return self.value
-
-	def set(self, value_:"T_PYTHON_REFERENCE"):
-		if value_.__class__.__name__ != self.type:
-			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
-			err_msg += f"Argument 1 of `ReferenceInstance.set` is not of type [{self.type}].\n"
-			raise TypeError(err_msg)
-		self.value = value_
-
-
-
-class Make_Reference (Generic[T_PYTHON_REFERENCE]):
-	@property
-	def reference(self) -> "Reference_Instance[T_PYTHON_REFERENCE]":
-		return self._reference
-
-	def __validate_type(self, line:str, file:str, line_no:int):
-		# Need to get the type of the class.
-		# The type is the part of the line after the square brackets.
-		s = line.split("=")[1].strip()
-		s = s.split("[")[1].strip()
-		s = s.split("]")[0].strip()
-		if self._type != s:
-			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
-			err_msg += f"For the class `Make_Reference`, the value passed in must match the generic.\n"
-			err_msg += f"Example of incorrect:  `my_ref = Make_Reference[bool](\"x\").reference`.\n"
-			err_msg += f"Example of correct:    `my_ref = Make_Reference[bool](True).reference`.\n"
-			err_msg += f"> Notice the `True` is a correct value for the generic `bool`.\n\n"
-			err_msg += f"Error occurred at line [{line_no}] in file [{file}].\n"
-			err_msg += f"> You tried to match the value type of [{self._type}]"
-			err_msg += f" with the generic type of [{s}].\n"
-			raise SyntaxError(err_msg)
-
-	def _validate(self):
-		# Need to get the line where the class was instantiated.
-		stack = inspect.stack()
-		caller = stack[3]
-		line_no = caller.lineno
-		file = caller.filename
-		with open(file, "r") as f:
-			lines = f.readlines()
-		_line = lines[line_no-1]
-		line = _line.strip().split("#")[0]
-		if not line.endswith(".reference"):
-			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
-			err_msg += f"For the class `Make_Reference`, the class instantiation must be assigned"
-			err_msg += f" using the syntax `my_ref = Make_Reference[< type >](< initial value >).reference`.\n"
-			err_msg += f"> Notice the `.reference` at the end of the instantiation.\n"
-			err_msg += f"Error occurred at line [{line_no}] in file [{file}].\n"
-			raise SyntaxError(err_msg)
-		self.__validate_type(line, file, line_no)
-
-	def __init__(self, value_:"T_PYTHON_REFERENCE"):
-		global _REF_VARS_SPECIAL_SAUCE
-		self._value = value_
-		self._type = value_.__class__.__name__
-		self._validate()
-		try:
-			_REF_VARS_SPECIAL_SAUCE = True
-			self._reference = Reference_Instance[type(value_)](self._type, value_)
-		finally:
-			_REF_VARS_SPECIAL_SAUCE = False
-
-
-
-
-
+from typing import Any, Callable, Generic, TypeVar
+import inspect
+
+
+
+_T_PYTHON_REFERENCE = TypeVar('_T_PYTHON_REFERENCE')
+_REF_VARS_SPECIAL_SAUCE = False
+_DO_RUNTIME_USAGE_CHECKS = True
+def disable_runtime_usage_checks():
+	global _DO_RUNTIME_USAGE_CHECKS
+	_DO_RUNTIME_USAGE_CHECKS = False
+
+
+
+class Reference (Generic[_T_PYTHON_REFERENCE]):
+	def __init__(self, type_:"str", value_:"_T_PYTHON_REFERENCE", do_runtime_usage_checks_:"bool"):
+		global _REF_VARS_SPECIAL_SAUCE
+		if _REF_VARS_SPECIAL_SAUCE == True:
+			self.type = type_
+			self.value = value_
+			self.__do_runtime_usage_checks = do_runtime_usage_checks_
+		else:
+			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+			err_msg += f"Do not instantiate the class `Reference` directly.\n"
+			err_msg += f"Instead, use the class `new`.\n"
+			raise SyntaxError(err_msg)
+
+	def get(self) -> "_T_PYTHON_REFERENCE":
+		return self.value
+
+	def set(self, value_:"_T_PYTHON_REFERENCE"):
+		if self.__do_runtime_usage_checks and value_.__class__.__name__ != self.type:
+			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+			err_msg += f"Argument 1 of `Reference.set` is not of type [{self.type}].\n"
+			raise TypeError(err_msg)
+		self.value = value_
+
+
+
+
+class new (Generic[_T_PYTHON_REFERENCE]):
+	def get_ref(self) -> "Reference[_T_PYTHON_REFERENCE]":
+		return self.__reference
+
+	def __validate_type(self, line_:"str"):
+		# Need to get the type of the class.
+		# The type is the part of the line after the square brackets.
+		s = line_
+		error_to_raise = 0
+		try:
+			s = s.split("[")[1].strip()
+			s = s.split("]")[0].strip()
+		except IndexError:
+			error_to_raise = 1
+		if error_to_raise == 1:
+			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+			err_msg += f"For the class `new`, you MUST provide generic type in square brackets.\n"
+			err_msg += f"Example of incorrect:  `my_ref = new(\"x\").get_ref()`.\n"
+			err_msg += f"Example of correct:    `my_ref = new[bool](True).get_ref()`.\n"
+			err_msg += f"                                    ~~~~~~ This is what you need.\n"
+			raise SyntaxError(err_msg)
+		if self.__type != s:
+			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+			err_msg += f"For the class `new`, the value passed in must match the generic.\n"
+			err_msg += f"Example of incorrect:  `my_ref = new[bool](\"x\").get_ref()`.\n"
+			err_msg += f"Example of correct:    `my_ref = new[bool](True).get_ref()`.\n"
+			err_msg += f"> Notice the `True` is a correct value for the generic `bool`.\n"
+			err_msg += f"> You tried to match the value type of [{self.__type}]"
+			err_msg += f" with the generic type of [{s}].\n"
+			raise SyntaxError(err_msg)
+
+	def _validate(self):
+		# Need to get the line where the class was instantiated.
+		stack = inspect.stack()
+		error_to_raise = 0
+		line = None
+		try:
+			caller = None
+			for stack_frame in stack:
+				f_name = stack_frame.filename
+				with open(f_name, "r") as f:
+					ctx = f.readlines()
+				l = ctx[stack_frame.lineno-1]
+				l = l.strip().split("#")[0]
+				if "=" in l:
+					splitted = l.split("=")
+					if len(splitted) > 1 and splitted[1].strip().startswith("new"):
+						caller = stack_frame
+						break
+				else:
+					if l.startswith("new") or l.startswith("refvars.new"):
+						caller = stack_frame
+						break
+			if caller is None:
+				error_to_raise = 3
+			else:
+				line_no = caller.lineno
+				file = caller.filename
+				with open(file, "r") as f:
+					lines = f.readlines()
+				_line = lines[line_no-1]
+				line = _line.strip().split("#")[0]
+				if not line.strip().endswith(".get_ref()"):
+					error_to_raise = 1
+		except IndexError:
+			error_to_raise = 2
+		if error_to_raise == 1:
+			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+			err_msg += f"For the class `new`, the class instantiation must be assigned using the syntax:\n"
+			err_msg += f"  `my_ref = new[< type >](< initial value >).get_ref()`.\n"
+			err_msg += f"                                            ~~~~~~~~~~\n"
+			err_msg += f"The highlighted part is one in which you must add to the end of the instantiation.\n"
+			err_msg += f"It must be exactly as printed and must be on the same line as the instantiation.\n"
+			raise SyntaxError(err_msg)
+		assert line is not None
+		self.__validate_type(line)
+
+	def __init__(self, value_:"_T_PYTHON_REFERENCE"):
+		global _REF_VARS_SPECIAL_SAUCE
+		global _DO_RUNTIME_USAGE_CHECKS
+		self.__type = value_.__class__.__name__
+		if _DO_RUNTIME_USAGE_CHECKS:
+			self._validate()
+		try:
+			_REF_VARS_SPECIAL_SAUCE = True
+			self.__reference = Reference[type(value_)](self.__type, value_, _DO_RUNTIME_USAGE_CHECKS)
+		finally:
+			_REF_VARS_SPECIAL_SAUCE = False
+
+
+
+class Pointer:
+	def __init__(self, addr_:"int", size_:"int") -> None:
+		global _REF_VARS_SPECIAL_SAUCE
+		if not _REF_VARS_SPECIAL_SAUCE == True:
+			self.address = addr_
+			self.size = size_
+		else:
+			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+			err_msg += f"Do not instantiate the class `Pointer` directly.\n"
+			err_msg += f"Instead, use the class `alloc`.\n"
+			raise SyntaxError(err_msg)
+		
+	def write(self, value_:"bytes") -> None:
+		from .mem_win_x86 import write
+		if len(value_) > self.size:
+			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+			err_msg += f"Out of bounds.\n"
+			raise MemoryError(err_msg)
+		write(self.address, value_)
+	
+	def read(self, size_:"int") -> "bytes":
+		from .mem_win_x86 import read
+		if size_ > self.size:
+			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+			err_msg += f"Out of bounds.\n"
+			raise MemoryError(err_msg)
+		return read(self.address, size_)
+	
+	def read_until_null_byte(self) -> "bytes":
+		all_data = self.read(self.size)
+		null_byte_index = all_data.find(b"\0")
+		if null_byte_index == -1:
+			raise ValueError("No null byte found.")
+		return all_data[:null_byte_index]
+
+
+
+class alloc:
+	def safe_access(self, callback_:"Callable[[Pointer],None]") -> "None":
+		from .mem_win_x86 import memory_access
+		def wrapper(_addr_:int) -> None:
+			nonlocal callback_
+			ptr = Pointer(_addr_, self.__size)
+			callback_(ptr)
+		memory_access(self.__size, wrapper)
+
+	def _validate(self):
+		# Need to get the line where the class was instantiated.
+		stack = inspect.stack()
+		caller = stack[-1]
+		line_no = caller.lineno
+		file = caller.filename
+		with open(file, "r") as f:
+			lines = f.readlines()
+		_line = lines[line_no-1]
+		line = _line.strip().split("#")[0]
+		if not len(line.split(").safe_access(")) == 2:
+			err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+			err_msg += f"For the class `alloc`, the class instantiation must be assigned using the syntax:\n"
+			err_msg += f"  `my_ptr = alloc(< size >).safe_access(< your callback >)`.\n"
+			err_msg += f"                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n"
+			err_msg += f"The highlighted part is one in which you must add to the end of the instantiation.\n"
+			err_msg += f"It must be exactly as printed and must be on the same line as the instantiation.\n"
+			err_msg += f"\n"
+			err_msg += f"Also note: The callback must be a function that takes `cb:'Callable[[int],None]'`.\n"
+			err_msg += f"             The first argument is the memory address.\n"
+			err_msg += f"             Do what ever you want with the memory address.\n"
+			err_msg += f"             On return of the function, the memory will be freed.\n"
+			raise SyntaxError(err_msg)
+		
+	def __init__(self, size_:"int") -> None:
+		global _REF_VARS_SPECIAL_SAUCE
+		global _DO_RUNTIME_USAGE_CHECKS
+		try:
+			MAX_MALLOC_SIZE_IN_C = 18_446_744_073_709_551_615  # Unsigned 64-bit integer (unsigned long long).
+			# We need to get the host architecture.
+			from platform import machine
+			arch = machine()
+			if arch != "AMD64":
+				raise NotImplementedError("The `alloc` class is only implemented for the AMD64 architecture.")
+			from os import name
+			if name != "nt":
+				raise NotImplementedError("The `alloc` class is only implemented for the Windows operating system.")
+			if size_ < 0:
+				err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+				err_msg += f"The size of the memory block must be a positive integer.\n"
+				raise ValueError(err_msg)
+			if size_ > MAX_MALLOC_SIZE_IN_C:
+				err_msg = "\n\n[[[ ERROR FROM `refvars`! ]]]\n"
+				err_msg += f"The size of the memory block is too large.\n"
+				err_msg += f"Please use a size less than {MAX_MALLOC_SIZE_IN_C}.\n"
+				raise ValueError(err_msg)
+			self.__size = size_
+			self._validate()
+		finally:
+			_REF_VARS_SPECIAL_SAUCE = False
+
```

## Comparing `refvars-0.6.dist-info/LICENCE` & `refvars-0.7.dist-info/LICENCE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,482 +1,482 @@
-# GNU LIBRARY GENERAL PUBLIC LICENSE
-
-Version 2, June 1991
-
-    Copyright (C) 1991 Free Software Foundation, Inc.
-    51 Franklin St, Fifth Floor, Boston, MA  02110-1301, USA
-    
-    Everyone is permitted to copy and distribute verbatim copies
-    of this license document, but changing it is not allowed.
-
-    [This is the first released version of the library GPL.  It is
-     numbered 2 because it goes with version 2 of the ordinary GPL.]
-
-## Preamble
-
-The licenses for most software are designed to take away your freedom
-to share and change it. By contrast, the GNU General Public Licenses
-are intended to guarantee your freedom to share and change free
-software--to make sure the software is free for all its users.
-
-This license, the Library General Public License, applies to some
-specially designated Free Software Foundation software, and to any
-other libraries whose authors decide to use it. You can use it for
-your libraries, too.
-
-When we speak of free software, we are referring to freedom, not
-price. Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-this service if you wish), that you receive source code or can get it
-if you want it, that you can change the software or use pieces of it
-in new free programs; and that you know you can do these things.
-
-To protect your rights, we need to make restrictions that forbid
-anyone to deny you these rights or to ask you to surrender the rights.
-These restrictions translate to certain responsibilities for you if
-you distribute copies of the library, or if you modify it.
-
-For example, if you distribute copies of the library, whether gratis
-or for a fee, you must give the recipients all the rights that we gave
-you. You must make sure that they, too, receive or can get the source
-code. If you link a program with the library, you must provide
-complete object files to the recipients so that they can relink them
-with the library, after making changes to the library and recompiling
-it. And you must show them these terms so they know their rights.
-
-Our method of protecting your rights has two steps: (1) copyright the
-library, and (2) offer you this license which gives you legal
-permission to copy, distribute and/or modify the library.
-
-Also, for each distributor's protection, we want to make certain that
-everyone understands that there is no warranty for this free library.
-If the library is modified by someone else and passed on, we want its
-recipients to know that what they have is not the original version, so
-that any problems introduced by others will not reflect on the
-original authors' reputations.
-
-Finally, any free program is threatened constantly by software
-patents. We wish to avoid the danger that companies distributing free
-software will individually obtain patent licenses, thus in effect
-transforming the program into proprietary software. To prevent this,
-we have made it clear that any patent must be licensed for everyone's
-free use or not licensed at all.
-
-Most GNU software, including some libraries, is covered by the
-ordinary GNU General Public License, which was designed for utility
-programs. This license, the GNU Library General Public License,
-applies to certain designated libraries. This license is quite
-different from the ordinary one; be sure to read it in full, and don't
-assume that anything in it is the same as in the ordinary license.
-
-The reason we have a separate public license for some libraries is
-that they blur the distinction we usually make between modifying or
-adding to a program and simply using it. Linking a program with a
-library, without changing the library, is in some sense simply using
-the library, and is analogous to running a utility program or
-application program. However, in a textual and legal sense, the linked
-executable is a combined work, a derivative of the original library,
-and the ordinary General Public License treats it as such.
-
-Because of this blurred distinction, using the ordinary General Public
-License for libraries did not effectively promote software sharing,
-because most developers did not use the libraries. We concluded that
-weaker conditions might promote sharing better.
-
-However, unrestricted linking of non-free programs would deprive the
-users of those programs of all benefit from the free status of the
-libraries themselves. This Library General Public License is intended
-to permit developers of non-free programs to use free libraries, while
-preserving your freedom as a user of such programs to change the free
-libraries that are incorporated in them. (We have not seen how to
-achieve this as regards changes in header files, but we have achieved
-it as regards changes in the actual functions of the Library.) The
-hope is that this will lead to faster development of free libraries.
-
-The precise terms and conditions for copying, distribution and
-modification follow. Pay close attention to the difference between a
-"work based on the library" and a "work that uses the library". The
-former contains code derived from the library, while the latter only
-works together with the library.
-
-Note that it is possible for a library to be covered by the ordinary
-General Public License rather than by this special one.
-
-## TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
-
-**0.** This License Agreement applies to any software library which
-contains a notice placed by the copyright holder or other authorized
-party saying it may be distributed under the terms of this Library
-General Public License (also called "this License"). Each licensee is
-addressed as "you".
-
-A "library" means a collection of software functions and/or data
-prepared so as to be conveniently linked with application programs
-(which use some of those functions and data) to form executables.
-
-The "Library", below, refers to any such software library or work
-which has been distributed under these terms. A "work based on the
-Library" means either the Library or any derivative work under
-copyright law: that is to say, a work containing the Library or a
-portion of it, either verbatim or with modifications and/or translated
-straightforwardly into another language. (Hereinafter, translation is
-included without limitation in the term "modification".)
-
-"Source code" for a work means the preferred form of the work for
-making modifications to it. For a library, complete source code means
-all the source code for all modules it contains, plus any associated
-interface definition files, plus the scripts used to control
-compilation and installation of the library.
-
-Activities other than copying, distribution and modification are not
-covered by this License; they are outside its scope. The act of
-running a program using the Library is not restricted, and output from
-such a program is covered only if its contents constitute a work based
-on the Library (independent of the use of the Library in a tool for
-writing it). Whether that is true depends on what the Library does and
-what the program that uses the Library does.
-
-**1.** You may copy and distribute verbatim copies of the Library's
-complete source code as you receive it, in any medium, provided that
-you conspicuously and appropriately publish on each copy an
-appropriate copyright notice and disclaimer of warranty; keep intact
-all the notices that refer to this License and to the absence of any
-warranty; and distribute a copy of this License along with the
-Library.
-
-You may charge a fee for the physical act of transferring a copy, and
-you may at your option offer warranty protection in exchange for a
-fee.
-
-**2.** You may modify your copy or copies of the Library or any
-portion of it, thus forming a work based on the Library, and copy and
-distribute such modifications or work under the terms of Section 1
-above, provided that you also meet all of these conditions:
-
--   **a)** The modified work must itself be a software library.
--   **b)** You must cause the files modified to carry prominent
-    notices stating that you changed the files and the date of
-    any change.
--   **c)** You must cause the whole of the work to be licensed at no
-    charge to all third parties under the terms of this License.
--   **d)** If a facility in the modified Library refers to a function
-    or a table of data to be supplied by an application program that
-    uses the facility, other than as an argument passed when the
-    facility is invoked, then you must make a good faith effort to
-    ensure that, in the event an application does not supply such
-    function or table, the facility still operates, and performs
-    whatever part of its purpose remains meaningful.
-
-    (For example, a function in a library to compute square roots has
-    a purpose that is entirely well-defined independent of
-    the application. Therefore, Subsection 2d requires that any
-    application-supplied function or table used by this function must
-    be optional: if the application does not supply it, the square
-    root function must still compute square roots.)
-
-These requirements apply to the modified work as a whole. If
-identifiable sections of that work are not derived from the Library,
-and can be reasonably considered independent and separate works in
-themselves, then this License, and its terms, do not apply to those
-sections when you distribute them as separate works. But when you
-distribute the same sections as part of a whole which is a work based
-on the Library, the distribution of the whole must be on the terms of
-this License, whose permissions for other licensees extend to the
-entire whole, and thus to each and every part regardless of who wrote
-it.
-
-Thus, it is not the intent of this section to claim rights or contest
-your rights to work written entirely by you; rather, the intent is to
-exercise the right to control the distribution of derivative or
-collective works based on the Library.
-
-In addition, mere aggregation of another work not based on the Library
-with the Library (or with a work based on the Library) on a volume of
-a storage or distribution medium does not bring the other work under
-the scope of this License.
-
-**3.** You may opt to apply the terms of the ordinary GNU General
-Public License instead of this License to a given copy of the Library.
-To do this, you must alter all the notices that refer to this License,
-so that they refer to the ordinary GNU General Public License, version
-2, instead of to this License. (If a newer version than version 2 of
-the ordinary GNU General Public License has appeared, then you can
-specify that version instead if you wish.) Do not make any other
-change in these notices.
-
-Once this change is made in a given copy, it is irreversible for that
-copy, so the ordinary GNU General Public License applies to all
-subsequent copies and derivative works made from that copy.
-
-This option is useful when you wish to copy part of the code of the
-Library into a program that is not a library.
-
-**4.** You may copy and distribute the Library (or a portion or
-derivative of it, under Section 2) in object code or executable form
-under the terms of Sections 1 and 2 above provided that you accompany
-it with the complete corresponding machine-readable source code, which
-must be distributed under the terms of Sections 1 and 2 above on a
-medium customarily used for software interchange.
-
-If distribution of object code is made by offering access to copy from
-a designated place, then offering equivalent access to copy the source
-code from the same place satisfies the requirement to distribute the
-source code, even though third parties are not compelled to copy the
-source along with the object code.
-
-**5.** A program that contains no derivative of any portion of the
-Library, but is designed to work with the Library by being compiled or
-linked with it, is called a "work that uses the Library". Such a work,
-in isolation, is not a derivative work of the Library, and therefore
-falls outside the scope of this License.
-
-However, linking a "work that uses the Library" with the Library
-creates an executable that is a derivative of the Library (because it
-contains portions of the Library), rather than a "work that uses the
-library". The executable is therefore covered by this License. Section
-6 states terms for distribution of such executables.
-
-When a "work that uses the Library" uses material from a header file
-that is part of the Library, the object code for the work may be a
-derivative work of the Library even though the source code is not.
-Whether this is true is especially significant if the work can be
-linked without the Library, or if the work is itself a library. The
-threshold for this to be true is not precisely defined by law.
-
-If such an object file uses only numerical parameters, data structure
-layouts and accessors, and small macros and small inline functions
-(ten lines or less in length), then the use of the object file is
-unrestricted, regardless of whether it is legally a derivative work.
-(Executables containing this object code plus portions of the Library
-will still fall under Section 6.)
-
-Otherwise, if the work is a derivative of the Library, you may
-distribute the object code for the work under the terms of Section 6.
-Any executables containing that work also fall under Section 6,
-whether or not they are linked directly with the Library itself.
-
-**6.** As an exception to the Sections above, you may also compile or
-link a "work that uses the Library" with the Library to produce a work
-containing portions of the Library, and distribute that work under
-terms of your choice, provided that the terms permit modification of
-the work for the customer's own use and reverse engineering for
-debugging such modifications.
-
-You must give prominent notice with each copy of the work that the
-Library is used in it and that the Library and its use are covered by
-this License. You must supply a copy of this License. If the work
-during execution displays copyright notices, you must include the
-copyright notice for the Library among them, as well as a reference
-directing the user to the copy of this License. Also, you must do one
-of these things:
-
--   **a)** Accompany the work with the complete corresponding
-    machine-readable source code for the Library including whatever
-    changes were used in the work (which must be distributed under
-    Sections 1 and 2 above); and, if the work is an executable linked
-    with the Library, with the complete machine-readable "work that
-    uses the Library", as object code and/or source code, so that the
-    user can modify the Library and then relink to produce a modified
-    executable containing the modified Library. (It is understood that
-    the user who changes the contents of definitions files in the
-    Library will not necessarily be able to recompile the application
-    to use the modified definitions.)
--   **b)** Accompany the work with a written offer, valid for at least
-    three years, to give the same user the materials specified in
-    Subsection 6a, above, for a charge no more than the cost of
-    performing this distribution.
--   **c)** If distribution of the work is made by offering access to
-    copy from a designated place, offer equivalent access to copy the
-    above specified materials from the same place.
--   **d)** Verify that the user has already received a copy of these
-    materials or that you have already sent this user a copy.
-
-For an executable, the required form of the "work that uses the
-Library" must include any data and utility programs needed for
-reproducing the executable from it. However, as a special exception,
-the source code distributed need not include anything that is normally
-distributed (in either source or binary form) with the major
-components (compiler, kernel, and so on) of the operating system on
-which the executable runs, unless that component itself accompanies
-the executable.
-
-It may happen that this requirement contradicts the license
-restrictions of other proprietary libraries that do not normally
-accompany the operating system. Such a contradiction means you cannot
-use both them and the Library together in an executable that you
-distribute.
-
-**7.** You may place library facilities that are a work based on the
-Library side-by-side in a single library together with other library
-facilities not covered by this License, and distribute such a combined
-library, provided that the separate distribution of the work based on
-the Library and of the other library facilities is otherwise
-permitted, and provided that you do these two things:
-
--   **a)** Accompany the combined library with a copy of the same work
-    based on the Library, uncombined with any other
-    library facilities. This must be distributed under the terms of
-    the Sections above.
--   **b)** Give prominent notice with the combined library of the fact
-    that part of it is a work based on the Library, and explaining
-    where to find the accompanying uncombined form of the same work.
-
-**8.** You may not copy, modify, sublicense, link with, or distribute
-the Library except as expressly provided under this License. Any
-attempt otherwise to copy, modify, sublicense, link with, or
-distribute the Library is void, and will automatically terminate your
-rights under this License. However, parties who have received copies,
-or rights, from you under this License will not have their licenses
-terminated so long as such parties remain in full compliance.
-
-**9.** You are not required to accept this License, since you have not
-signed it. However, nothing else grants you permission to modify or
-distribute the Library or its derivative works. These actions are
-prohibited by law if you do not accept this License. Therefore, by
-modifying or distributing the Library (or any work based on the
-Library), you indicate your acceptance of this License to do so, and
-all its terms and conditions for copying, distributing or modifying
-the Library or works based on it.
-
-**10.** Each time you redistribute the Library (or any work based on
-the Library), the recipient automatically receives a license from the
-original licensor to copy, distribute, link with or modify the Library
-subject to these terms and conditions. You may not impose any further
-restrictions on the recipients' exercise of the rights granted herein.
-You are not responsible for enforcing compliance by third parties to
-this License.
-
-**11.** If, as a consequence of a court judgment or allegation of
-patent infringement or for any other reason (not limited to patent
-issues), conditions are imposed on you (whether by court order,
-agreement or otherwise) that contradict the conditions of this
-License, they do not excuse you from the conditions of this License.
-If you cannot distribute so as to satisfy simultaneously your
-obligations under this License and any other pertinent obligations,
-then as a consequence you may not distribute the Library at all. For
-example, if a patent license would not permit royalty-free
-redistribution of the Library by all those who receive copies directly
-or indirectly through you, then the only way you could satisfy both it
-and this License would be to refrain entirely from distribution of the
-Library.
-
-If any portion of this section is held invalid or unenforceable under
-any particular circumstance, the balance of the section is intended to
-apply, and the section as a whole is intended to apply in other
-circumstances.
-
-It is not the purpose of this section to induce you to infringe any
-patents or other property right claims or to contest validity of any
-such claims; this section has the sole purpose of protecting the
-integrity of the free software distribution system which is
-implemented by public license practices. Many people have made
-generous contributions to the wide range of software distributed
-through that system in reliance on consistent application of that
-system; it is up to the author/donor to decide if he or she is willing
-to distribute software through any other system and a licensee cannot
-impose that choice.
-
-This section is intended to make thoroughly clear what is believed to
-be a consequence of the rest of this License.
-
-**12.** If the distribution and/or use of the Library is restricted in
-certain countries either by patents or by copyrighted interfaces, the
-original copyright holder who places the Library under this License
-may add an explicit geographical distribution limitation excluding
-those countries, so that distribution is permitted only in or among
-countries not thus excluded. In such case, this License incorporates
-the limitation as if written in the body of this License.
-
-**13.** The Free Software Foundation may publish revised and/or new
-versions of the Library General Public License from time to time. Such
-new versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Library
-specifies a version number of this License which applies to it and
-"any later version", you have the option of following the terms and
-conditions either of that version or of any later version published by
-the Free Software Foundation. If the Library does not specify a
-license version number, you may choose any version ever published by
-the Free Software Foundation.
-
-**14.** If you wish to incorporate parts of the Library into other
-free programs whose distribution conditions are incompatible with
-these, write to the author to ask for permission. For software which
-is copyrighted by the Free Software Foundation, write to the Free
-Software Foundation; we sometimes make exceptions for this. Our
-decision will be guided by the two goals of preserving the free status
-of all derivatives of our free software and of promoting the sharing
-and reuse of software generally.
-
-**NO WARRANTY**
-
-**15.** BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
-WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
-EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
-OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
-KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
-LIBRARY IS WITH YOU. SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
-THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-**16.** IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
-WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
-AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
-FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
-CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
-LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
-RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
-FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
-SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
-DAMAGES.
-
-END OF TERMS AND CONDITIONS
-
-## How to Apply These Terms to Your New Libraries
-
-If you develop a new library, and you want it to be of the greatest
-possible use to the public, we recommend making it free software that
-everyone can redistribute and change. You can do so by permitting
-redistribution under these terms (or, alternatively, under the terms
-of the ordinary General Public License).
-
-To apply these terms, attach the following notices to the library. It
-is safest to attach them to the start of each source file to most
-effectively convey the exclusion of warranty; and each file should
-have at least the "copyright" line and a pointer to where the full
-notice is found.
-
-    one line to give the library's name and an idea of what it does.
-    Copyright (C) year  name of author
-
-    This library is free software; you can redistribute it and/or
-    modify it under the terms of the GNU Library General Public
-    License as published by the Free Software Foundation; either
-    version 2 of the License, or (at your option) any later version.
-
-    This library is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-    Library General Public License for more details.
-
-    You should have received a copy of the GNU Library General Public
-    License along with this library; if not, write to the
-    Free Software Foundation, Inc., 51 Franklin St, Fifth Floor,
-    Boston, MA  02110-1301, USA.
-
-Also add information on how to contact you by electronic and paper
-mail.
-
-You should also get your employer (if you work as a programmer) or
-your school, if any, to sign a "copyright disclaimer" for the library,
-if necessary. Here is a sample; alter the names:
-
-    Yoyodyne, Inc., hereby disclaims all copyright interest in
-    the library `Frob' (a library for tweaking knobs) written
-    by James Random Hacker.
-
-    signature of Ty Coon, 1 April 1990
-    Ty Coon, President of Vice
-
+# GNU LIBRARY GENERAL PUBLIC LICENSE
+
+Version 2, June 1991
+
+    Copyright (C) 1991 Free Software Foundation, Inc.
+    51 Franklin St, Fifth Floor, Boston, MA  02110-1301, USA
+    
+    Everyone is permitted to copy and distribute verbatim copies
+    of this license document, but changing it is not allowed.
+
+    [This is the first released version of the library GPL.  It is
+     numbered 2 because it goes with version 2 of the ordinary GPL.]
+
+## Preamble
+
+The licenses for most software are designed to take away your freedom
+to share and change it. By contrast, the GNU General Public Licenses
+are intended to guarantee your freedom to share and change free
+software--to make sure the software is free for all its users.
+
+This license, the Library General Public License, applies to some
+specially designated Free Software Foundation software, and to any
+other libraries whose authors decide to use it. You can use it for
+your libraries, too.
+
+When we speak of free software, we are referring to freedom, not
+price. Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+this service if you wish), that you receive source code or can get it
+if you want it, that you can change the software or use pieces of it
+in new free programs; and that you know you can do these things.
+
+To protect your rights, we need to make restrictions that forbid
+anyone to deny you these rights or to ask you to surrender the rights.
+These restrictions translate to certain responsibilities for you if
+you distribute copies of the library, or if you modify it.
+
+For example, if you distribute copies of the library, whether gratis
+or for a fee, you must give the recipients all the rights that we gave
+you. You must make sure that they, too, receive or can get the source
+code. If you link a program with the library, you must provide
+complete object files to the recipients so that they can relink them
+with the library, after making changes to the library and recompiling
+it. And you must show them these terms so they know their rights.
+
+Our method of protecting your rights has two steps: (1) copyright the
+library, and (2) offer you this license which gives you legal
+permission to copy, distribute and/or modify the library.
+
+Also, for each distributor's protection, we want to make certain that
+everyone understands that there is no warranty for this free library.
+If the library is modified by someone else and passed on, we want its
+recipients to know that what they have is not the original version, so
+that any problems introduced by others will not reflect on the
+original authors' reputations.
+
+Finally, any free program is threatened constantly by software
+patents. We wish to avoid the danger that companies distributing free
+software will individually obtain patent licenses, thus in effect
+transforming the program into proprietary software. To prevent this,
+we have made it clear that any patent must be licensed for everyone's
+free use or not licensed at all.
+
+Most GNU software, including some libraries, is covered by the
+ordinary GNU General Public License, which was designed for utility
+programs. This license, the GNU Library General Public License,
+applies to certain designated libraries. This license is quite
+different from the ordinary one; be sure to read it in full, and don't
+assume that anything in it is the same as in the ordinary license.
+
+The reason we have a separate public license for some libraries is
+that they blur the distinction we usually make between modifying or
+adding to a program and simply using it. Linking a program with a
+library, without changing the library, is in some sense simply using
+the library, and is analogous to running a utility program or
+application program. However, in a textual and legal sense, the linked
+executable is a combined work, a derivative of the original library,
+and the ordinary General Public License treats it as such.
+
+Because of this blurred distinction, using the ordinary General Public
+License for libraries did not effectively promote software sharing,
+because most developers did not use the libraries. We concluded that
+weaker conditions might promote sharing better.
+
+However, unrestricted linking of non-free programs would deprive the
+users of those programs of all benefit from the free status of the
+libraries themselves. This Library General Public License is intended
+to permit developers of non-free programs to use free libraries, while
+preserving your freedom as a user of such programs to change the free
+libraries that are incorporated in them. (We have not seen how to
+achieve this as regards changes in header files, but we have achieved
+it as regards changes in the actual functions of the Library.) The
+hope is that this will lead to faster development of free libraries.
+
+The precise terms and conditions for copying, distribution and
+modification follow. Pay close attention to the difference between a
+"work based on the library" and a "work that uses the library". The
+former contains code derived from the library, while the latter only
+works together with the library.
+
+Note that it is possible for a library to be covered by the ordinary
+General Public License rather than by this special one.
+
+## TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+**0.** This License Agreement applies to any software library which
+contains a notice placed by the copyright holder or other authorized
+party saying it may be distributed under the terms of this Library
+General Public License (also called "this License"). Each licensee is
+addressed as "you".
+
+A "library" means a collection of software functions and/or data
+prepared so as to be conveniently linked with application programs
+(which use some of those functions and data) to form executables.
+
+The "Library", below, refers to any such software library or work
+which has been distributed under these terms. A "work based on the
+Library" means either the Library or any derivative work under
+copyright law: that is to say, a work containing the Library or a
+portion of it, either verbatim or with modifications and/or translated
+straightforwardly into another language. (Hereinafter, translation is
+included without limitation in the term "modification".)
+
+"Source code" for a work means the preferred form of the work for
+making modifications to it. For a library, complete source code means
+all the source code for all modules it contains, plus any associated
+interface definition files, plus the scripts used to control
+compilation and installation of the library.
+
+Activities other than copying, distribution and modification are not
+covered by this License; they are outside its scope. The act of
+running a program using the Library is not restricted, and output from
+such a program is covered only if its contents constitute a work based
+on the Library (independent of the use of the Library in a tool for
+writing it). Whether that is true depends on what the Library does and
+what the program that uses the Library does.
+
+**1.** You may copy and distribute verbatim copies of the Library's
+complete source code as you receive it, in any medium, provided that
+you conspicuously and appropriately publish on each copy an
+appropriate copyright notice and disclaimer of warranty; keep intact
+all the notices that refer to this License and to the absence of any
+warranty; and distribute a copy of this License along with the
+Library.
+
+You may charge a fee for the physical act of transferring a copy, and
+you may at your option offer warranty protection in exchange for a
+fee.
+
+**2.** You may modify your copy or copies of the Library or any
+portion of it, thus forming a work based on the Library, and copy and
+distribute such modifications or work under the terms of Section 1
+above, provided that you also meet all of these conditions:
+
+-   **a)** The modified work must itself be a software library.
+-   **b)** You must cause the files modified to carry prominent
+    notices stating that you changed the files and the date of
+    any change.
+-   **c)** You must cause the whole of the work to be licensed at no
+    charge to all third parties under the terms of this License.
+-   **d)** If a facility in the modified Library refers to a function
+    or a table of data to be supplied by an application program that
+    uses the facility, other than as an argument passed when the
+    facility is invoked, then you must make a good faith effort to
+    ensure that, in the event an application does not supply such
+    function or table, the facility still operates, and performs
+    whatever part of its purpose remains meaningful.
+
+    (For example, a function in a library to compute square roots has
+    a purpose that is entirely well-defined independent of
+    the application. Therefore, Subsection 2d requires that any
+    application-supplied function or table used by this function must
+    be optional: if the application does not supply it, the square
+    root function must still compute square roots.)
+
+These requirements apply to the modified work as a whole. If
+identifiable sections of that work are not derived from the Library,
+and can be reasonably considered independent and separate works in
+themselves, then this License, and its terms, do not apply to those
+sections when you distribute them as separate works. But when you
+distribute the same sections as part of a whole which is a work based
+on the Library, the distribution of the whole must be on the terms of
+this License, whose permissions for other licensees extend to the
+entire whole, and thus to each and every part regardless of who wrote
+it.
+
+Thus, it is not the intent of this section to claim rights or contest
+your rights to work written entirely by you; rather, the intent is to
+exercise the right to control the distribution of derivative or
+collective works based on the Library.
+
+In addition, mere aggregation of another work not based on the Library
+with the Library (or with a work based on the Library) on a volume of
+a storage or distribution medium does not bring the other work under
+the scope of this License.
+
+**3.** You may opt to apply the terms of the ordinary GNU General
+Public License instead of this License to a given copy of the Library.
+To do this, you must alter all the notices that refer to this License,
+so that they refer to the ordinary GNU General Public License, version
+2, instead of to this License. (If a newer version than version 2 of
+the ordinary GNU General Public License has appeared, then you can
+specify that version instead if you wish.) Do not make any other
+change in these notices.
+
+Once this change is made in a given copy, it is irreversible for that
+copy, so the ordinary GNU General Public License applies to all
+subsequent copies and derivative works made from that copy.
+
+This option is useful when you wish to copy part of the code of the
+Library into a program that is not a library.
+
+**4.** You may copy and distribute the Library (or a portion or
+derivative of it, under Section 2) in object code or executable form
+under the terms of Sections 1 and 2 above provided that you accompany
+it with the complete corresponding machine-readable source code, which
+must be distributed under the terms of Sections 1 and 2 above on a
+medium customarily used for software interchange.
+
+If distribution of object code is made by offering access to copy from
+a designated place, then offering equivalent access to copy the source
+code from the same place satisfies the requirement to distribute the
+source code, even though third parties are not compelled to copy the
+source along with the object code.
+
+**5.** A program that contains no derivative of any portion of the
+Library, but is designed to work with the Library by being compiled or
+linked with it, is called a "work that uses the Library". Such a work,
+in isolation, is not a derivative work of the Library, and therefore
+falls outside the scope of this License.
+
+However, linking a "work that uses the Library" with the Library
+creates an executable that is a derivative of the Library (because it
+contains portions of the Library), rather than a "work that uses the
+library". The executable is therefore covered by this License. Section
+6 states terms for distribution of such executables.
+
+When a "work that uses the Library" uses material from a header file
+that is part of the Library, the object code for the work may be a
+derivative work of the Library even though the source code is not.
+Whether this is true is especially significant if the work can be
+linked without the Library, or if the work is itself a library. The
+threshold for this to be true is not precisely defined by law.
+
+If such an object file uses only numerical parameters, data structure
+layouts and accessors, and small macros and small inline functions
+(ten lines or less in length), then the use of the object file is
+unrestricted, regardless of whether it is legally a derivative work.
+(Executables containing this object code plus portions of the Library
+will still fall under Section 6.)
+
+Otherwise, if the work is a derivative of the Library, you may
+distribute the object code for the work under the terms of Section 6.
+Any executables containing that work also fall under Section 6,
+whether or not they are linked directly with the Library itself.
+
+**6.** As an exception to the Sections above, you may also compile or
+link a "work that uses the Library" with the Library to produce a work
+containing portions of the Library, and distribute that work under
+terms of your choice, provided that the terms permit modification of
+the work for the customer's own use and reverse engineering for
+debugging such modifications.
+
+You must give prominent notice with each copy of the work that the
+Library is used in it and that the Library and its use are covered by
+this License. You must supply a copy of this License. If the work
+during execution displays copyright notices, you must include the
+copyright notice for the Library among them, as well as a reference
+directing the user to the copy of this License. Also, you must do one
+of these things:
+
+-   **a)** Accompany the work with the complete corresponding
+    machine-readable source code for the Library including whatever
+    changes were used in the work (which must be distributed under
+    Sections 1 and 2 above); and, if the work is an executable linked
+    with the Library, with the complete machine-readable "work that
+    uses the Library", as object code and/or source code, so that the
+    user can modify the Library and then relink to produce a modified
+    executable containing the modified Library. (It is understood that
+    the user who changes the contents of definitions files in the
+    Library will not necessarily be able to recompile the application
+    to use the modified definitions.)
+-   **b)** Accompany the work with a written offer, valid for at least
+    three years, to give the same user the materials specified in
+    Subsection 6a, above, for a charge no more than the cost of
+    performing this distribution.
+-   **c)** If distribution of the work is made by offering access to
+    copy from a designated place, offer equivalent access to copy the
+    above specified materials from the same place.
+-   **d)** Verify that the user has already received a copy of these
+    materials or that you have already sent this user a copy.
+
+For an executable, the required form of the "work that uses the
+Library" must include any data and utility programs needed for
+reproducing the executable from it. However, as a special exception,
+the source code distributed need not include anything that is normally
+distributed (in either source or binary form) with the major
+components (compiler, kernel, and so on) of the operating system on
+which the executable runs, unless that component itself accompanies
+the executable.
+
+It may happen that this requirement contradicts the license
+restrictions of other proprietary libraries that do not normally
+accompany the operating system. Such a contradiction means you cannot
+use both them and the Library together in an executable that you
+distribute.
+
+**7.** You may place library facilities that are a work based on the
+Library side-by-side in a single library together with other library
+facilities not covered by this License, and distribute such a combined
+library, provided that the separate distribution of the work based on
+the Library and of the other library facilities is otherwise
+permitted, and provided that you do these two things:
+
+-   **a)** Accompany the combined library with a copy of the same work
+    based on the Library, uncombined with any other
+    library facilities. This must be distributed under the terms of
+    the Sections above.
+-   **b)** Give prominent notice with the combined library of the fact
+    that part of it is a work based on the Library, and explaining
+    where to find the accompanying uncombined form of the same work.
+
+**8.** You may not copy, modify, sublicense, link with, or distribute
+the Library except as expressly provided under this License. Any
+attempt otherwise to copy, modify, sublicense, link with, or
+distribute the Library is void, and will automatically terminate your
+rights under this License. However, parties who have received copies,
+or rights, from you under this License will not have their licenses
+terminated so long as such parties remain in full compliance.
+
+**9.** You are not required to accept this License, since you have not
+signed it. However, nothing else grants you permission to modify or
+distribute the Library or its derivative works. These actions are
+prohibited by law if you do not accept this License. Therefore, by
+modifying or distributing the Library (or any work based on the
+Library), you indicate your acceptance of this License to do so, and
+all its terms and conditions for copying, distributing or modifying
+the Library or works based on it.
+
+**10.** Each time you redistribute the Library (or any work based on
+the Library), the recipient automatically receives a license from the
+original licensor to copy, distribute, link with or modify the Library
+subject to these terms and conditions. You may not impose any further
+restrictions on the recipients' exercise of the rights granted herein.
+You are not responsible for enforcing compliance by third parties to
+this License.
+
+**11.** If, as a consequence of a court judgment or allegation of
+patent infringement or for any other reason (not limited to patent
+issues), conditions are imposed on you (whether by court order,
+agreement or otherwise) that contradict the conditions of this
+License, they do not excuse you from the conditions of this License.
+If you cannot distribute so as to satisfy simultaneously your
+obligations under this License and any other pertinent obligations,
+then as a consequence you may not distribute the Library at all. For
+example, if a patent license would not permit royalty-free
+redistribution of the Library by all those who receive copies directly
+or indirectly through you, then the only way you could satisfy both it
+and this License would be to refrain entirely from distribution of the
+Library.
+
+If any portion of this section is held invalid or unenforceable under
+any particular circumstance, the balance of the section is intended to
+apply, and the section as a whole is intended to apply in other
+circumstances.
+
+It is not the purpose of this section to induce you to infringe any
+patents or other property right claims or to contest validity of any
+such claims; this section has the sole purpose of protecting the
+integrity of the free software distribution system which is
+implemented by public license practices. Many people have made
+generous contributions to the wide range of software distributed
+through that system in reliance on consistent application of that
+system; it is up to the author/donor to decide if he or she is willing
+to distribute software through any other system and a licensee cannot
+impose that choice.
+
+This section is intended to make thoroughly clear what is believed to
+be a consequence of the rest of this License.
+
+**12.** If the distribution and/or use of the Library is restricted in
+certain countries either by patents or by copyrighted interfaces, the
+original copyright holder who places the Library under this License
+may add an explicit geographical distribution limitation excluding
+those countries, so that distribution is permitted only in or among
+countries not thus excluded. In such case, this License incorporates
+the limitation as if written in the body of this License.
+
+**13.** The Free Software Foundation may publish revised and/or new
+versions of the Library General Public License from time to time. Such
+new versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Library
+specifies a version number of this License which applies to it and
+"any later version", you have the option of following the terms and
+conditions either of that version or of any later version published by
+the Free Software Foundation. If the Library does not specify a
+license version number, you may choose any version ever published by
+the Free Software Foundation.
+
+**14.** If you wish to incorporate parts of the Library into other
+free programs whose distribution conditions are incompatible with
+these, write to the author to ask for permission. For software which
+is copyrighted by the Free Software Foundation, write to the Free
+Software Foundation; we sometimes make exceptions for this. Our
+decision will be guided by the two goals of preserving the free status
+of all derivatives of our free software and of promoting the sharing
+and reuse of software generally.
+
+**NO WARRANTY**
+
+**15.** BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
+WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
+EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
+OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
+KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
+LIBRARY IS WITH YOU. SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
+THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+**16.** IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
+WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
+AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
+FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
+CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
+LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
+RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
+FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
+SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
+DAMAGES.
+
+END OF TERMS AND CONDITIONS
+
+## How to Apply These Terms to Your New Libraries
+
+If you develop a new library, and you want it to be of the greatest
+possible use to the public, we recommend making it free software that
+everyone can redistribute and change. You can do so by permitting
+redistribution under these terms (or, alternatively, under the terms
+of the ordinary General Public License).
+
+To apply these terms, attach the following notices to the library. It
+is safest to attach them to the start of each source file to most
+effectively convey the exclusion of warranty; and each file should
+have at least the "copyright" line and a pointer to where the full
+notice is found.
+
+    one line to give the library's name and an idea of what it does.
+    Copyright (C) year  name of author
+
+    This library is free software; you can redistribute it and/or
+    modify it under the terms of the GNU Library General Public
+    License as published by the Free Software Foundation; either
+    version 2 of the License, or (at your option) any later version.
+
+    This library is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+    Library General Public License for more details.
+
+    You should have received a copy of the GNU Library General Public
+    License along with this library; if not, write to the
+    Free Software Foundation, Inc., 51 Franklin St, Fifth Floor,
+    Boston, MA  02110-1301, USA.
+
+Also add information on how to contact you by electronic and paper
+mail.
+
+You should also get your employer (if you work as a programmer) or
+your school, if any, to sign a "copyright disclaimer" for the library,
+if necessary. Here is a sample; alter the names:
+
+    Yoyodyne, Inc., hereby disclaims all copyright interest in
+    the library `Frob' (a library for tweaking knobs) written
+    by James Random Hacker.
+
+    signature of Ty Coon, 1 April 1990
+    Ty Coon, President of Vice
+
 That's all there is to it!
```

