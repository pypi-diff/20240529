# Comparing `tmp/goit_phone_book_bot-0.2.0.tar.gz` & `tmp/goit_phone_book_bot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goit_phone_book_bot-0.2.0.tar", last modified: Sun May 26 14:52:59 2024, max compression
+gzip compressed data, was "goit_phone_book_bot-0.2.1.tar", last modified: Wed May 29 15:30:33 2024, max compression
```

## Comparing `goit_phone_book_bot-0.2.0.tar` & `goit_phone_book_bot-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:52:59.631452 goit_phone_book_bot-0.2.0/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit_phone_book_bot-0.2.0/LICENSE
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      742 2024-05-26 14:52:59.631248 goit_phone_book_bot-0.2.0/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      216 2024-05-26 14:51:27.000000 goit_phone_book_bot-0.2.0/README.md
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:52:59.631007 goit_phone_book_bot-0.2.0/goit_phone_book_bot.egg-info/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      742 2024-05-26 14:52:59.000000 goit_phone_book_bot-0.2.0/goit_phone_book_bot.egg-info/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      637 2024-05-26 14:52:59.000000 goit_phone_book_bot-0.2.0/goit_phone_book_bot.egg-info/SOURCES.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-26 14:52:59.000000 goit_phone_book_bot-0.2.0/goit_phone_book_bot.egg-info/dependency_links.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       54 2024-05-26 14:52:59.000000 goit_phone_book_bot-0.2.0/goit_phone_book_bot.egg-info/entry_points.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-26 14:52:59.000000 goit_phone_book_bot-0.2.0/goit_phone_book_bot.egg-info/requires.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-26 14:52:59.000000 goit_phone_book_bot-0.2.0/goit_phone_book_bot.egg-info/top_level.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-26 14:52:59.631493 goit_phone_book_bot-0.2.0/setup.cfg
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      822 2024-05-26 14:51:39.000000 goit_phone_book_bot-0.2.0/setup.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:52:59.626917 goit_phone_book_bot-0.2.0/src/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:38:25.000000 goit_phone_book_bot-0.2.0/src/__init__.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:52:59.629891 goit_phone_book_bot-0.2.0/src/classes/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:46:19.000000 goit_phone_book_bot-0.2.0/src/classes/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      408 2024-05-25 18:33:44.000000 goit_phone_book_bot-0.2.0/src/classes/address.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4492 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.2.0/src/classes/address_book.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1703 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.2.0/src/classes/birthday.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      915 2024-05-25 22:34:07.000000 goit_phone_book_bot-0.2.0/src/classes/email.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      126 2024-05-25 18:13:46.000000 goit_phone_book_bot-0.2.0/src/classes/field.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      251 2024-05-23 17:44:13.000000 goit_phone_book_bot-0.2.0/src/classes/note.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     3102 2024-05-25 18:58:18.000000 goit_phone_book_bot-0.2.0/src/classes/notes_book.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1240 2024-05-25 22:34:07.000000 goit_phone_book_bot-0.2.0/src/classes/phone.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4245 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.2.0/src/classes/record.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:52:59.630258 goit_phone_book_bot-0.2.0/src/constants/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:48:38.000000 goit_phone_book_bot-0.2.0/src/constants/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     2001 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.2.0/src/constants/commands.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4394 2024-05-26 14:46:56.000000 goit_phone_book_bot-0.2.0/src/main.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:52:59.630652 goit_phone_book_bot-0.2.0/src/utils/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:46:28.000000 goit_phone_book_bot-0.2.0/src/utils/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)    10711 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.2.0/src/utils/utils.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-29 15:30:33.937604 goit_phone_book_bot-0.2.1/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit_phone_book_bot-0.2.1/LICENSE
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1019 2024-05-29 15:30:33.937371 goit_phone_book_bot-0.2.1/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      493 2024-05-26 15:16:37.000000 goit_phone_book_bot-0.2.1/README.md
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-29 15:30:33.937113 goit_phone_book_bot-0.2.1/goit_phone_book_bot.egg-info/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1019 2024-05-29 15:30:33.000000 goit_phone_book_bot-0.2.1/goit_phone_book_bot.egg-info/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      637 2024-05-29 15:30:33.000000 goit_phone_book_bot-0.2.1/goit_phone_book_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-29 15:30:33.000000 goit_phone_book_bot-0.2.1/goit_phone_book_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       54 2024-05-29 15:30:33.000000 goit_phone_book_bot-0.2.1/goit_phone_book_bot.egg-info/entry_points.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-29 15:30:33.000000 goit_phone_book_bot-0.2.1/goit_phone_book_bot.egg-info/requires.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-29 15:30:33.000000 goit_phone_book_bot-0.2.1/goit_phone_book_bot.egg-info/top_level.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-29 15:30:33.937643 goit_phone_book_bot-0.2.1/setup.cfg
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      822 2024-05-29 15:29:46.000000 goit_phone_book_bot-0.2.1/setup.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-29 15:30:33.933158 goit_phone_book_bot-0.2.1/src/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:38:25.000000 goit_phone_book_bot-0.2.1/src/__init__.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-29 15:30:33.936001 goit_phone_book_bot-0.2.1/src/classes/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:46:19.000000 goit_phone_book_bot-0.2.1/src/classes/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      408 2024-05-25 18:33:44.000000 goit_phone_book_bot-0.2.1/src/classes/address.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4469 2024-05-29 15:28:31.000000 goit_phone_book_bot-0.2.1/src/classes/address_book.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1703 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.2.1/src/classes/birthday.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      915 2024-05-25 22:34:07.000000 goit_phone_book_bot-0.2.1/src/classes/email.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      126 2024-05-25 18:13:46.000000 goit_phone_book_bot-0.2.1/src/classes/field.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      251 2024-05-23 17:44:13.000000 goit_phone_book_bot-0.2.1/src/classes/note.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     3102 2024-05-25 18:58:18.000000 goit_phone_book_bot-0.2.1/src/classes/notes_book.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1240 2024-05-25 22:34:07.000000 goit_phone_book_bot-0.2.1/src/classes/phone.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4206 2024-05-29 15:24:47.000000 goit_phone_book_bot-0.2.1/src/classes/record.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-29 15:30:33.936399 goit_phone_book_bot-0.2.1/src/constants/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:48:38.000000 goit_phone_book_bot-0.2.1/src/constants/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     2001 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.2.1/src/constants/commands.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4394 2024-05-26 14:46:56.000000 goit_phone_book_bot-0.2.1/src/main.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-29 15:30:33.936743 goit_phone_book_bot-0.2.1/src/utils/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-26 14:46:28.000000 goit_phone_book_bot-0.2.1/src/utils/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)    10711 2024-05-26 14:28:46.000000 goit_phone_book_bot-0.2.1/src/utils/utils.py
```

### Comparing `goit_phone_book_bot-0.2.0/LICENSE` & `goit_phone_book_bot-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.2.0/goit_phone_book_bot.egg-info/SOURCES.txt` & `goit_phone_book_bot-0.2.1/goit_phone_book_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.2.0/setup.py` & `goit_phone_book_bot-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='goit-phone-book-bot',
-    version='0.2.0',
+    version='0.2.1',
     author='Vasyl Martyniv',
     author_email='doc.people97@gmail.com',
     description='Phone Book bot developed by team #5 - CREATORS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VasylMartyniv/GoIT_Phone_Book_bot',
     packages=find_packages(),
```

### Comparing `goit_phone_book_bot-0.2.0/src/classes/address_book.py` & `goit_phone_book_bot-0.2.1/src/classes/address_book.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,39 +26,38 @@
     def add_record(self, record: Record):
         if record.name in self.data:
             raise ValueError("ERROR: An element with the specified name already exists in the AddressBook ")
         else:
             self.data[record.name] = record
 
     # Видаляти запис із списку
-    def delete_record(self, record: Record):
-        if record.name in self.data:
-            self.data.pop(record.name)
+    def delete_record(self, name: str):
+        if name in self.data:
+            self.data.pop(name)
         else:
             raise ValueError("ERROR: An element does not exist in the AddressBook ")
 
     # Змінювати ключ запису (Це зміна імені разом із зміною імені у запису через метод класу Record)
     def change_record_name(self, old_record: Record, new_name: str):
         if old_record.name in self.data:
             if new_name in self.data:
                 raise ValueError("ERROR: An element with the specified name already exists in the AddressBook ")
             else:
                 self.data[new_name] = self.data[old_record.name]
                 self.data[new_name].name = new_name
                 del self.data[old_record.name]
         else:
             raise ValueError("ERROR: An element does not exist in the AddressBook ")
-    
+
     def find_by_name(self, name):
         for record in self.data.values():
             if record.name.lower() == name.lower():
                 return record
         raise KeyError("ERROR: The item with the specified name does not exist in AddressBook")
 
-
     # Пошук контакту за телефономa
     def find_by_phone(self, phone: str):
         for record in self.data:
             if self.data[record].find_phone(phone):
                 return self.data[record]
         raise KeyError("ERROR: The item with the specified phone does not exist in AddressBook")
 
@@ -93,8 +92,8 @@
                         birthdays_in_range.append((record.name, next_birthday_date))
 
         # Sort birthdays by date
         birthdays_in_range.sort(key=lambda x: x[1])
 
         # Print the next birthdays
         for name, birthday_date in birthdays_in_range:
-            print(f"{name}: {birthday_date.strftime('%d-%m-%Y')}")
+            print(f"{name}: {birthday_date.strftime('%d-%m-%Y')}")
```

### Comparing `goit_phone_book_bot-0.2.0/src/classes/birthday.py` & `goit_phone_book_bot-0.2.1/src/classes/birthday.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.2.0/src/classes/email.py` & `goit_phone_book_bot-0.2.1/src/classes/email.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.2.0/src/classes/notes_book.py` & `goit_phone_book_bot-0.2.1/src/classes/notes_book.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.2.0/src/classes/phone.py` & `goit_phone_book_bot-0.2.1/src/classes/phone.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.2.0/src/classes/record.py` & `goit_phone_book_bot-0.2.1/src/classes/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from src.classes.address import Address
 from src.classes.email import Email
 from src.classes.phone import Phone
-from src.classes.birthday import Birthday
 
 
 class Record:
     def __init__(self, name: str):
         self.name = name
         self.phones = list()
         self.emails = list()
@@ -35,38 +34,35 @@
         # Зібрати адресу
         if self.address:
             address = "Address: " + self.address.value + "\n"
         else:
             address = ""
 
         # Зібрати день народження
-        if self.birthday:
+        if self.birthday.value:
             birthday = "Birthday:" + self.birthday.value + "\n"
         else:
             birthday = ""
 
         # Зібрати стрічку
         return f"{name}{phones}{emails}{address}{birthday}" + "\n"
 
-
     def add_birthday(users_db):
         name = input("Enter the name of the contact to add birthday: ")
         birthday_str = input("Enter the birthday (DD-MM-YYYY): ")
         try:
             record = users_db.get(name)
             if record:
                 record.set_birthday(birthday_str)
                 print(f"Birthday {birthday_str} added to contact {name}.")
             else:
                 print(f"No contact found with the name {name}.")
         except ValueError as e:
             print(e)
 
-
-
     # Tools for working with the field:   phones
     def add_phone(self, phone):
         self.phones.append(Phone(phone))
 
     def edit_phone(self, old_phone: str, new_phone: str):
         is_exception = True
         for i in range(len(self.phones)):
```

### Comparing `goit_phone_book_bot-0.2.0/src/constants/commands.py` & `goit_phone_book_bot-0.2.1/src/constants/commands.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.2.0/src/main.py` & `goit_phone_book_bot-0.2.1/src/main.py`

 * *Files identical despite different names*

### Comparing `goit_phone_book_bot-0.2.0/src/utils/utils.py` & `goit_phone_book_bot-0.2.1/src/utils/utils.py`

 * *Files identical despite different names*

