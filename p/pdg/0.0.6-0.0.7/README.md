# Comparing `tmp/pdg-0.0.6.tar.gz` & `tmp/pdg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pdg-0.0.6.tar", last modified: Fri Dec 15 02:09:20 2023, max compression
+gzip compressed data, was "dist/pdg-0.0.7.tar", last modified: Tue May 28 22:24:43 2024, max compression
```

## Comparing `pdg-0.0.6.tar` & `pdg-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jb        (1000) users      (100)        0 2023-12-15 02:09:20.000000 pdg-0.0.6/
--rw-r--r--   0 jb        (1000) users      (100)      268 2023-05-26 20:05:07.000000 pdg-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 jb        (1000) users      (100)     2490 2023-04-18 00:36:31.000000 pdg-0.0.6/LICENSE.txt
--rw-r--r--   0 jb        (1000) users      (100)       25 2023-05-21 19:11:59.000000 pdg-0.0.6/MANIFEST.in
--rw-r--r--   0 jb        (1000) users      (100)     1782 2023-12-15 02:09:20.000000 pdg-0.0.6/PKG-INFO
--rw-r--r--   0 jb        (1000) users      (100)      887 2023-06-01 03:45:38.000000 pdg-0.0.6/README.md
-drwxr-xr-x   0 jb        (1000) users      (100)        0 2023-12-15 02:09:20.000000 pdg-0.0.6/pdg/
--rw-r--r--   0 jb        (1000) users      (100)     1209 2023-06-01 04:16:53.000000 pdg-0.0.6/pdg/__init__.py
--rw-r--r--   0 jb        (1000) users      (100)    12022 2023-12-15 01:35:55.000000 pdg-0.0.6/pdg/api.py
--rw-r--r--   0 jb        (1000) users      (100)    17315 2023-12-15 01:35:55.000000 pdg-0.0.6/pdg/data.py
--rw-r--r--   0 jb        (1000) users      (100)      912 2023-05-14 03:00:02.000000 pdg-0.0.6/pdg/decay.py
--rw-r--r--   0 jb        (1000) users      (100)      601 2023-05-19 02:24:13.000000 pdg-0.0.6/pdg/errors.py
--rw-r--r--   0 jb        (1000) users      (100)    17053 2023-12-15 01:35:55.000000 pdg-0.0.6/pdg/particle.py
--rw-r--r--   0 jb        (1000) users      (100)  4521984 2023-12-15 01:56:33.000000 pdg-0.0.6/pdg/pdg.sqlite
--rw-r--r--   0 jb        (1000) users      (100)     1154 2023-12-15 01:35:55.000000 pdg-0.0.6/pdg/units.py
--rw-r--r--   0 jb        (1000) users      (100)     3366 2023-12-15 01:35:55.000000 pdg-0.0.6/pdg/utils.py
-drwxr-xr-x   0 jb        (1000) users      (100)        0 2023-12-15 02:09:20.000000 pdg-0.0.6/pdg.egg-info/
--rw-r--r--   0 jb        (1000) users      (100)     1782 2023-12-15 02:09:20.000000 pdg-0.0.6/pdg.egg-info/PKG-INFO
--rw-r--r--   0 jb        (1000) users      (100)      315 2023-12-15 02:09:20.000000 pdg-0.0.6/pdg.egg-info/SOURCES.txt
--rw-r--r--   0 jb        (1000) users      (100)        1 2023-12-15 02:09:20.000000 pdg-0.0.6/pdg.egg-info/dependency_links.txt
--rw-r--r--   0 jb        (1000) users      (100)       16 2023-12-15 02:09:20.000000 pdg-0.0.6/pdg.egg-info/requires.txt
--rw-r--r--   0 jb        (1000) users      (100)        4 2023-12-15 02:09:20.000000 pdg-0.0.6/pdg.egg-info/top_level.txt
--rw-r--r--   0 jb        (1000) users      (100)       38 2023-12-15 02:09:20.000000 pdg-0.0.6/setup.cfg
--rw-r--r--   0 jb        (1000) users      (100)     1610 2023-06-01 04:16:53.000000 pdg-0.0.6/setup.py
+drwxr-xr-x   0 jb        (1000) users      (100)        0 2024-05-28 22:24:43.000000 pdg-0.0.7/
+-rw-r--r--   0 jb        (1000) users      (100)      268 2023-12-22 02:02:05.000000 pdg-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 jb        (1000) users      (100)     2490 2023-12-22 02:02:05.000000 pdg-0.0.7/LICENSE.txt
+-rw-r--r--   0 jb        (1000) users      (100)       25 2023-12-22 02:02:05.000000 pdg-0.0.7/MANIFEST.in
+-rw-r--r--   0 jb        (1000) users      (100)     2881 2024-05-28 22:24:43.000000 pdg-0.0.7/PKG-INFO
+-rw-r--r--   0 jb        (1000) users      (100)     1607 2024-05-28 20:00:21.000000 pdg-0.0.7/README.md
+drwxr-xr-x   0 jb        (1000) users      (100)        0 2024-05-28 22:24:43.000000 pdg-0.0.7/pdg/
+-rw-r--r--   0 jb        (1000) users      (100)     1209 2023-12-22 02:03:45.000000 pdg-0.0.7/pdg/__init__.py
+-rw-r--r--   0 jb        (1000) users      (100)    13242 2024-05-24 22:02:33.000000 pdg-0.0.7/pdg/api.py
+-rw-r--r--   0 jb        (1000) users      (100)    17729 2024-05-24 22:02:33.000000 pdg-0.0.7/pdg/data.py
+-rw-r--r--   0 jb        (1000) users      (100)     3035 2024-05-24 22:02:33.000000 pdg-0.0.7/pdg/decay.py
+-rw-r--r--   0 jb        (1000) users      (100)      601 2023-12-22 02:02:05.000000 pdg-0.0.7/pdg/errors.py
+-rw-r--r--   0 jb        (1000) users      (100)    22290 2024-05-24 22:02:33.000000 pdg-0.0.7/pdg/particle.py
+-rw-r--r--   0 jb        (1000) users      (100)  7426048 2024-05-28 20:00:21.000000 pdg-0.0.7/pdg/pdg.sqlite
+-rw-r--r--   0 jb        (1000) users      (100)     1154 2023-12-22 02:02:07.000000 pdg-0.0.7/pdg/units.py
+-rw-r--r--   0 jb        (1000) users      (100)     3188 2024-05-24 22:02:33.000000 pdg-0.0.7/pdg/utils.py
+drwxr-xr-x   0 jb        (1000) users      (100)        0 2024-05-28 22:24:43.000000 pdg-0.0.7/pdg.egg-info/
+-rw-r--r--   0 jb        (1000) users      (100)     2881 2024-05-28 22:24:43.000000 pdg-0.0.7/pdg.egg-info/PKG-INFO
+-rw-r--r--   0 jb        (1000) users      (100)      315 2024-05-28 22:24:43.000000 pdg-0.0.7/pdg.egg-info/SOURCES.txt
+-rw-r--r--   0 jb        (1000) users      (100)        1 2024-05-28 22:24:43.000000 pdg-0.0.7/pdg.egg-info/dependency_links.txt
+-rw-r--r--   0 jb        (1000) users      (100)       16 2024-05-28 22:24:43.000000 pdg-0.0.7/pdg.egg-info/requires.txt
+-rw-r--r--   0 jb        (1000) users      (100)        4 2024-05-28 22:24:43.000000 pdg-0.0.7/pdg.egg-info/top_level.txt
+-rw-r--r--   0 jb        (1000) users      (100)       38 2024-05-28 22:24:43.000000 pdg-0.0.7/setup.cfg
+-rw-r--r--   0 jb        (1000) users      (100)     1813 2024-05-28 20:00:21.000000 pdg-0.0.7/setup.py
```

### Comparing `pdg-0.0.6/LICENSE.txt` & `pdg-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdg-0.0.6/pdg/__init__.py` & `pdg-0.0.7/pdg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 For documentation see https://pdgapi.lbl.gov/doc.
 
 For general information about PDG and the Review of Particle Physics
 please visit https://pdg.lbl.gov.
 """
 __author__ = 'Particle Data Group'
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 
 
 import os
 from pdg.api import PdgApi
 from pdg.errors import PdgApiError
 
 
 # Constants
 SQLITE_FILENAME = 'pdg.sqlite'      # Default SQLite database file used by this API
-MIN_SCHEMA_VERSION = 0.1            # Minimum schema version required by this version of the API
+MIN_SCHEMA_VERSION = 0.2            # Minimum schema version required by this version of the API
 
 
 def connect(database_url=None, pedantic=False):
     """Connect to PDG database and return configured PDG API object."""
     if database_url is None:
         api = PdgApi('sqlite:///%s' % os.path.join(os.path.dirname(__file__), SQLITE_FILENAME), pedantic)
     else:
```

### Comparing `pdg-0.0.6/pdg/api.py` & `pdg-0.0.7/pdg/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 PDG API top-level class.
 """
 
 import sqlalchemy
 from sqlalchemy import func, select, bindparam, distinct, desc
 import pdg
-from pdg.errors import PdgInvalidPdgIdError, PdgNoDataError
-from pdg.utils import base_id
+from pdg.errors import PdgAmbiguousValueError, PdgInvalidPdgIdError, PdgNoDataError
+from pdg.utils import parse_id
 from pdg.data import PdgProperty, PdgMass, PdgWidth, PdgLifetime
-from pdg.decay import PdgBranchingFraction
-from pdg.particle import PdgParticle
+from pdg.decay import PdgBranchingFraction, PdgItem
+from pdg.particle import PdgParticle, PdgParticleList
 
 
 # Map PDG data type codes to corresponding classes
 DATA_TYPE_MAP = {
-    'PART': PdgParticle,
+    'PART': PdgParticleList,
     'M':    PdgMass,
     'BFX':  PdgBranchingFraction,
     'BFX1': PdgBranchingFraction,
     'BFX2': PdgBranchingFraction,
     'BFX3': PdgBranchingFraction,
     'BFX4': PdgBranchingFraction,
     'BFX5': PdgBranchingFraction,
@@ -92,31 +92,35 @@
 
     def get(self, pdgid, edition=None):
         """Return PdgData object for given PDG Identifier.
 
         The get method checks what data the PDG Identifier describes and returns an
         object of the most appropriate class derived from the PdgData base class.
         For example, for a PDG Identifier describing a particle, an object of class
-        PdgParticle is returned, while for a branching fraction a PdgBranchingFraction
+        PdgParticleList is returned, while for a branching fraction a PdgBranchingFraction
         object is returned.
 
         edition can be set to a specific edition, from which the data should later be retrieved.
         """
+        if edition is None:
+            baseid, edition = parse_id(pdgid)
+        else:
+            baseid = pdgid
         pdgid_table = self.db.tables['pdgid']
         try:
             query = select(pdgid_table.c.data_type).where(pdgid_table.c.pdgid == bindparam('pdgid'))
             with self.engine.connect() as conn:
-                data_type = conn.execute(query, {'pdgid': base_id(pdgid)}).fetchone()[0]
+                data_type = conn.execute(query, {'pdgid': baseid}).fetchone()[0]
         except Exception:
             raise PdgInvalidPdgIdError('PDG Identifier %s not found' % pdgid)
         try:
             cls = DATA_TYPE_MAP[data_type]
         except KeyError:
             cls = PdgProperty
-        return cls(self, pdgid, edition)
+        return cls(self, baseid, edition)
 
     def get_all(self, data_type_key=None, edition=None):
         """Return iterator over all PDG Identifiers / quantities. Returns PdgProperties or derived classes.
 
         If data_type_key is set, only quantities of the given type are returned.
         See doc_data_type_keys() for the list of possible data type codes.
 
@@ -131,37 +135,59 @@
             for item in conn.execute(query, {'data_type_key': data_type_key}):
                 try:
                     cls = DATA_TYPE_MAP[item.data_type]
                 except KeyError:
                     cls = PdgProperty
                 yield cls(self, item.pdgid, edition)
 
-    def get_particle_by_name(self, name, case_sensitive=True, edition=None):
-        """Get particle by its name.
-
-        case_sensitive can be set False to indicate that the particle name should be
-        considered not case-sensitive.
-
-        edition can be set to a specific edition, from which data should later be retrieved.
+    def _get_particles_by_name(self, name, case_sensitive=True, edition=None, unique=True):
+        """Helper function used by get_particle(s)_by_name. Returns a
+        PdgParticle (list thereof) if unique is True (False). Raises a
+        PdgAmbiguousValueError if more than one PdgItem exists with the given
+        name, or if unique=True and the PdgItem refers to more than one
+        particle.
         """
-        pdgparticle_table = self.db.tables['pdgparticle']
-        query = select(pdgparticle_table.c.pdgid, pdgparticle_table.c.mcid)
+        pdgitem_table = self.db.tables['pdgitem']
+        query = select(pdgitem_table.c.id)
         if case_sensitive:
-            query = query.where(pdgparticle_table.c.name == bindparam('name'))
+            query = query.where(pdgitem_table.c.name == bindparam('name'))
         else:
             name = name.lower()
-            query = query.where(func.lower(pdgparticle_table.c.name) == bindparam('name'))
+            query = query.where(func.lower(pdgitem_table.c.name) == bindparam('name'))
         with self.engine.connect() as conn:
             matches = conn.execute(query, {'name': name}).fetchall()
         if len(matches) == 0:
             raise ValueError('No particle found with name %s' % name)
         elif len(matches) == 1:
-            return PdgParticle(self, matches[0].pdgid, edition, set_mcid=matches[0].mcid)
+            item = PdgItem(self, matches[0].id, edition=edition)
+            return item.particle if unique else item.particles
         else:
-            raise ValueError('%s matches %i particles with PDG Identifiers %s' % (name, len(matches), matches))
+            raise PdgAmbiguousValueError('More than one PDGITEM named %s', name)
+
+    def get_particle_by_name(self, name, case_sensitive=True, edition=None):
+        """Get particle by its name.
+
+        case_sensitive can be set False to indicate that the particle name should be
+        considered not case-sensitive.
+
+        edition can be set to a specific edition, from which data should later be retrieved.
+        """
+        return self._get_particles_by_name(name, case_sensitive=case_sensitive,
+                                           edition=edition, unique=True)
+
+    def get_particles_by_name(self, name, case_sensitive=True, edition=None):
+        """Get all particles for a (possibly generic) name.
+
+        case_sensitive can be set False to indicate that the particle name should be
+        considered not case-sensitive.
+
+        edition can be set to a specific edition, from which data should later be retrieved.
+        """
+        return self._get_particles_by_name(name, case_sensitive=case_sensitive,
+                                           edition=edition, unique=False)
 
     def get_particle_by_mcid(self, mcid, edition=None):
         """Get particle by its MC ID.
 
         edition can be set to a specific edition, from which data should later be retrieved.
         """
         pdgparticle_table = self.db.tables['pdgparticle']
@@ -184,15 +210,15 @@
         pdgid_table = self.db.tables['pdgid']
         pdgparticle_table = self.db.tables['pdgparticle']
         query = select(distinct(pdgid_table.c.pdgid)).join(pdgparticle_table)
         query = query.where(pdgid_table.c.data_type == 'PART')
         query = query.order_by(pdgid_table.c.sort)
         with self.engine.connect() as conn:
             for item in conn.execute(query):
-                yield PdgParticle(self, item.pdgid, edition)
+                yield PdgParticleList(self, item.pdgid, edition)
 
     def doc_key_value(self, table_name, column_name, key):
         """Get documentation on the meaning of key values or flags used in the PDG API."""
         pdgdoc_table = self.db.tables['pdgdoc']
         query = select(pdgdoc_table)
         query = query.where(pdgdoc_table.c.table_name == bindparam('table_name'))
         query = query.where(pdgdoc_table.c.column_name == bindparam('column_name'))
```

### Comparing `pdg-0.0.6/pdg/data.py` & `pdg-0.0.7/pdg/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,21 +299,31 @@
     def get_parent_pdgid(self, include_edition=True):
         """Return PDG Identifiers of parent quantity."""
         if include_edition:
             return make_id(self._get_pdgid()['parent_pdgid'], self.edition)
         else:
             return self._get_pdgid()['parent_pdgid']
 
-    def get_particle(self):
-        """Return PdgParticle for this property's particle."""
+    def get_particles(self):
+        """Return PdgParticleList for this property's particle."""
         p = self
         while p.baseid != p.get_parent_pdgid(False) and p.get_parent_pdgid(False):
             p = self.api.get(p.get_parent_pdgid())
         return p
 
+    def get_particle(self):
+        """Returns PdgParticle for this property's particle. Raises
+        PdgAmbiguousValueError when there are multiple matches."""
+        ps = self.get_particles()
+        assert len(ps) > 0
+        if len(ps) > 1:
+            err = "More than one PdgParticle found. Consider using get_particles() instead."
+            raise PdgAmbiguousValueError(err)
+        return ps[0]
+
     @property
     def edition(self):
         """Year of edition for which data is requested."""
         return self._edition
 
     @edition.setter
     def edition(self, edition):
```

### Comparing `pdg-0.0.6/pdg/errors.py` & `pdg-0.0.7/pdg/errors.py`

 * *Files identical despite different names*

### Comparing `pdg-0.0.6/pdg/particle.py` & `pdg-0.0.7/pdg/particle.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,153 @@
 """
 Definition of top-level particle container class.
 """
 
-from sqlalchemy import select, bindparam, distinct
+from sqlalchemy import select, bindparam, distinct, func
 from sqlalchemy import and_, or_
 from pdg.errors import PdgApiError, PdgNoDataError, PdgAmbiguousValueError
 from pdg.utils import make_id, best
 from pdg.data import PdgData
 from pdg.units import HBAR_IN_GEV_S
 
 
+class PdgItem:
+    """A class to represent an "item" encountered in e.g. a description of a
+    decay's products. An item can correspond directly to one particle,
+    indirectly to one particle (as an alias), to a set of particles (as a
+    generic name), or to an arbitrary string. When possible, a PdgItem can be
+    queried (via the particle/particles properties) for the associated
+    particle(s).
+    """
+    def __init__(self, api, pdgitem_id, edition=None):
+        """Constructor for a PdgItem. Intended for internal API use."""
+        self.api = api
+        self.pdgitem_id = pdgitem_id
+        self.cache = {}
+        self.edition = edition
+
+    def __repr__(self):
+        """Return a human-readable representation of the PdgItem."""
+        name = self._get_pdgitem()['name']
+        return 'PdgItem("%s")' % name
+
+    def _get_pdgitem(self):
+        """Load the PdgItem's data from the database."""
+        if 'pdgitem' not in self.cache:
+            pdgitem_table = self.api.db.tables['pdgitem']
+            query = select(pdgitem_table).where(pdgitem_table.c.id == bindparam('pdgitem_id'))
+            with self.api.engine.connect() as conn:
+                result = conn.execute(query, {'pdgitem_id': self.pdgitem_id}).fetchone()
+                if result is None:
+                    raise PdgNoDataError('No PDGITEM entry for %s' % self.pdgitem_id)
+                self.cache['pdgitem'] = result._mapping
+        return self.cache['pdgitem']
+
+    def _get_targets(self):
+        """Get all PdgItems that this one maps directly to. Does not recurse."""
+        pdgitem_map_table = self.api.db.tables['pdgitem_map']
+        query = select(pdgitem_map_table).where(pdgitem_map_table.c.pdgitem_id == bindparam('pdgitem_id'))
+        with self.api.engine.connect() as conn:
+            rows = conn.execute(query, {'pdgitem_id': self.pdgitem_id}).fetchall()
+            for row in rows:
+                yield PdgItem(self.api, row.target_id)
+
+    @property
+    def has_particle(self):
+        """Whether the PdgItem is associated with exactly one particle. The
+        property has_particles indicates whether it is associated with one or
+        more.
+        """
+        if 'has_particle' not in self.cache:
+            pdgparticle_table = self.api.db.tables['pdgparticle']
+            query = select(pdgparticle_table).where(pdgparticle_table.c.pdgitem_id == bindparam('pdgitem_id'))
+            with self.api.engine.connect() as conn:
+                result = conn.execute(query, {'pdgitem_id': self.pdgitem_id}).fetchone()
+                if result:
+                    self.cache['pdgparticle'] = result._mapping
+                    self.cache['has_particle'] = True
+                else:
+                    targets = list(self._get_targets())
+                    if len(targets) == 1 and targets[0].has_particle:
+                        self.cache['pdgparticle'] = targets[0].cache['pdgparticle']
+                        self.cache['has_particle'] = True
+                    else:
+                        self.cache['has_particle'] = False
+        return self.cache['has_particle']
+
+    @property
+    def particle(self):
+        """The particle associated with the PdgItem, if there is exactly one
+        such particle. Raises PdgAmbiguousValueError if there are more than one,
+        in which case the particles property can be used instead.
+        """
+        if not self.has_particle:
+            if self.has_particles:
+                raise PdgAmbiguousValueError('No unique PDGPARTICLE for PDGITEM %s' % self.pdgitem_id)
+            raise PdgNoDataError('No PDGPARTICLE for PDGITEM %s' % self.pdgitem_id)
+        p = self.cache['pdgparticle']
+        return PdgParticle(self.api, p['pdgid'], edition=self.edition, set_mcid=p['mcid'])
+
+    @property
+    def particles(self):
+        """The list of all particles associated with the PdgItem."""
+        if self.has_particle:
+            return [self.particle]
+        else:
+            result = []
+            for target in self._get_targets():
+                for p in target.particles:
+                    result.append(p)
+            return result
+
+    @property
+    def has_particles(self):
+        """Whether the PdgItem is associated with at least one particle."""
+        return len(list(self.particles)) > 0
+
+    @property
+    def name(self):
+        """The name of the PdgItem."""
+        return self._get_pdgitem()['name']
+
+    # @property
+    # def name_tex(self):
+    #     """The TeX name of the PdgItem."""
+    #     return self._get_pdgitem()['name_tex']
+
+    @property
+    def item_type(self):
+        """The type of the PdgItem. A single character with the following meanings:
+              'P': specific state (e.g. "pi+"),
+              'A': "also" alias,
+              'W': "was" alias,
+              'S': shortcut,
+              'B': both charges (e.g. "pi+-"),
+              'C': both charges, conjugate (e.g. "pi-+"),
+              'G': generic state (e.g. "pi"),
+              'L': general list (e.g. "leptons"),
+              'I': inclusive indicator (e.g. "X"),
+              'T': arbitrary text
+        """
+        return self._get_pdgitem()['item_type']
+
+
 class PdgParticle(PdgData):
     """Container class for all information about a given particle.
 
     In addition to access to basic particle properties such as mass, charge, quantum numbers and
     PDG MC ID, this class provides methods to iterate over the data on all particle properties listed
     in Particle Listings and Summary Tables, including branching fractions, masses, life-times, etc.
     """
 
-    def __init__(self, api, pdgid, edition=None, set_mcid=None):
+    def __init__(self, api, pdgid, edition=None, set_mcid=None, set_name=None):
         """Constructor for a PdgParticle given its PDG Identifier and possibly its MC ID."""
         super(PdgParticle, self).__init__(api, pdgid, edition)
         self.set_mcid = set_mcid
-        self.cc_type_flag = 'P'
-        if set_mcid is not None and set_mcid < 0:
-            self.cc_type_flag = 'A'
+        self.set_name = set_name
 
     def __str__(self):
         try:
             return 'Data for PDG Particle %s: %s' % (self.pdgid, self.name)
         except PdgAmbiguousValueError:
             return 'Data for PDG Particle %s: multiple particle matches' % self.pdgid
 
@@ -36,32 +155,28 @@
         """Get particle data."""
         if 'pdgparticle' not in self.cache:
             pdgparticle_table = self.api.db.tables['pdgparticle']
             query = select(pdgparticle_table)
             query = query.where(pdgparticle_table.c.pdgid == bindparam('pdgid'))
             if self.set_mcid is not None:
                 query = query.where(pdgparticle_table.c.mcid == bindparam('mcid'))
-            query = query.where(pdgparticle_table.c.entry_type == 'P')
-            query = query.where(or_(and_(pdgparticle_table.c.charge_type == 'S', pdgparticle_table.c.cc_type == bindparam('cc_type')),
-                                    and_(pdgparticle_table.c.charge_type == 'S', pdgparticle_table.c.cc_type == 'S'),
-                                    and_(pdgparticle_table.c.charge_type == 'E', pdgparticle_table.c.cc_type.is_(None))))
+            if self.set_name is not None:
+                query = query.where(pdgparticle_table.c.name == bindparam('name'))
             with self.api.engine.connect() as conn:
-                params = {'pdgid': self.baseid, 'cc_type': self.cc_type_flag, 'mcid': self.set_mcid}
+                params = {'pdgid': self.baseid, 'mcid': self.set_mcid, 'name': self.set_name}
                 matches = conn.execute(query, params).fetchall()
             if len(matches) == 1:
                 self.cache['pdgparticle'] = matches[0]._mapping
             else:
-                # Charge-specific state either not found or ambiguous - try looking for entry with CHARGE_TYPE='G'
+                # Charge-specific state either not found or ambiguous
                 query = select(pdgparticle_table)
                 query = query.where(pdgparticle_table.c.pdgid == bindparam('pdgid'))
                 if self.set_mcid is not None:
                     query = query.where(pdgparticle_table.c.mcid == bindparam('mcid'))
-                query = query.where(pdgparticle_table.c.entry_type == 'P')
-                query = query.where(pdgparticle_table.c.charge_type == 'G')
-                query = query.where(pdgparticle_table.c.cc_type.is_(None))
+                query = query.where(pdgparticle_table.c.cc_type == 'S')
                 query = query.where(pdgparticle_table.c.name.notlike('%bar%'))   # Exclude generic "*bar" states
                 with self.api.engine.connect() as conn:
                     params = {'pdgid': self.baseid, 'mcid': self.set_mcid}
                     matches_g = conn.execute(query, params).fetchall()
                 if len(matches_g) == 0:
                     mcid_string = ', MC ID = %s' % self.set_mcid if self.set_mcid else ''
                     raise PdgNoDataError('Particle data for %s%s not found' % (self.pdgid, mcid_string))
@@ -274,98 +389,111 @@
 
     @property
     def is_baryon(self):
         """True if particle is a baryon."""
         return 'B' in self.data_flags
 
     @property
-    def is_generic(self):
-        """True if particle represents a generic charge state."""
-        return self._get_particle_data()['charge_type'] == 'G'
-
-    @property
     def mass(self):
         """Mass of the particle in GeV."""
-        best_mass_property = best(self.masses(), self.api.pedantic, '%s mass (%s)' % (self.name, self.pdgid),
-                                  self.is_generic)
+        best_mass_property = best(self.masses(), self.api.pedantic, '%s mass (%s)' % (self.name, self.pdgid))
         return best_mass_property.best_summary().get_value('GeV')
 
     @property
     def mass_error(self):
         """Symmetric error on mass of particle in GeV, or None if mass error are asymmetric or mass is a limit."""
-        best_mass_property = best(self.masses(), self.api.pedantic, '%s (%s)' % (self.pdgid, self.description),
-                                  self.is_generic)
+        best_mass_property = best(self.masses(), self.api.pedantic, '%s (%s)' % (self.pdgid, self.description))
         return best_mass_property.best_summary().get_error('GeV')
 
     @property
     def width(self):
         """Width of the particle in GeV."""
         try:
-            best_width_property = best(self.widths(), self.api.pedantic, '%s width (%s)' % (self.name, self.pdgid),
-                                       self.is_generic)
+            best_width_property = best(self.widths(), self.api.pedantic, '%s width (%s)' % (self.name, self.pdgid))
             return best_width_property.best_summary().get_value('GeV')
         except PdgNoDataError:
             if self.api.pedantic:
                 raise
             # S063 has a lifetime entry but it's NULL
             if (not self.has_lifetime_entry) or (self.lifetime is None):
                 return 0.
             return HBAR_IN_GEV_S / self.lifetime
 
     @property
     def width_error(self):
         """Symmetric error on width of particle in GeV, or None if width error are asymmetric or width is a limit."""
         try:
-            best_width_property = best(self.widths(), self.api.pedantic, '%s (%s)' % (self.pdgid, self.description),
-                                       self.is_generic)
+            best_width_property = best(self.widths(), self.api.pedantic, '%s (%s)' % (self.pdgid, self.description))
             return best_width_property.best_summary().get_error('GeV')
         except PdgNoDataError:
             if self.api.pedantic:
                 raise
             # S063 has a lifetime entry but it's NULL
             if (not self.has_lifetime_entry) or (self.lifetime is None):
                 return 0.
             return self.lifetime_error * HBAR_IN_GEV_S / self.lifetime**2
 
     @property
     def lifetime(self):
         """Lifetime of the particle in seconds."""
         try:
-            best_lifetime_property = best(self.lifetimes(), self.api.pedantic, '%s lifetime (%s)' % (self.name, self.pdgid),
-                                          self.is_generic)
+            best_lifetime_property = best(self.lifetimes(), self.api.pedantic, '%s lifetime (%s)' % (self.name, self.pdgid))
             return best_lifetime_property.best_summary().get_value('s')
         except PdgNoDataError:
             if self.api.pedantic:
                 raise
             if not self.has_width_entry:
                 return float('inf')
             return HBAR_IN_GEV_S / self.width
 
     @property
     def lifetime_error(self):
         """Symmetric error on lifetime of particle in seconds, or None if lifetime error are asymmetric or lifetime is a limit."""
         try:
-            best_lifetime_property = best(self.lifetimes(), self.api.pedantic, '%s (%s)' % (self.pdgid, self.description),
-                                          self.is_generic)
+            best_lifetime_property = best(self.lifetimes(), self.api.pedantic, '%s (%s)' % (self.pdgid, self.description))
             err = best_lifetime_property.best_summary().get_error('s')
             if err is None:
                 err = 0.
             return err
         except PdgNoDataError:
             if self.api.pedantic:
                 raise
             if not self.has_width_entry:
                 return 0.
             return self.width_error * HBAR_IN_GEV_S / self.width**2
 
 
     @property
     def has_width_entry(self):
+        """Whether the particle has at least one defined decay width."""
         return next(self.widths(), None) is not None
 
     @property
     def has_lifetime_entry(self):
+        """Whether the particle has at least one defined lifetime."""
         return next(self.lifetimes(), None) is not None
 
     @property
     def is_stable(self):
+        """Whether the particle is stable (i.e. does not have a defined lifetime
+        or decay width).
+        """
         return not (self.has_width_entry() or self.has_lifetime_entry())
+
+
+class PdgParticleList(PdgData, list):
+    """A PdgData subclass to represent a list of PdgParticles. A PdgParticleList
+    is returned when PdgApi.get is called with the PDGID of a (group of)
+    particles.
+    """
+    def __init__(self, api, pdgid, edition=None):
+        """Constructor for a PdgParticleList given its PDG Identifier."""
+        super(PdgParticleList, self).__init__(api, pdgid, edition)
+
+        pdgparticle_table = self.api.db.tables['pdgparticle']
+        query = select(pdgparticle_table)
+        query = query.where(func.lower(pdgparticle_table.c.pdgid) == bindparam('pdgid'))
+        with self.api.engine.connect() as conn:
+            result = conn.execute(query, {'pdgid': pdgid.lower()}).fetchall()
+            for row in result:
+                self.append(PdgParticle(api, pdgid, edition=edition, set_mcid=row.mcid,
+                                        set_name=row.name))
```

### Comparing `pdg-0.0.6/pdg/units.py` & `pdg-0.0.7/pdg/units.py`

 * *Files identical despite different names*

### Comparing `pdg-0.0.6/pdg/utils.py` & `pdg-0.0.7/pdg/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         return None
     if edition is None:
         return baseid.upper()
     else:
         return ('%s/%s' % (baseid, edition)).upper()
 
 
-def best(properties, pedantic=False, quantity=None, is_generic=False):
+def best(properties, pedantic=False, quantity=None):
     """Return the "best" property from an iterable of properties, or raise an exception.
 
     best does (pedantic=False) or does not (pedantic=True) make assumptions about what the best property might
     be in cases where the choice may be ambiguous. In the latter case, a PdgAmbiguous exception is raised while in the
     former case the best property is determined based on data flags and position in the Summary Tables.
     PdgNoDataError will be raised if there is no property that qualifies as best one.
 
@@ -72,18 +72,16 @@
         props_without_alternates = [p for p in props_without_alternates
                                     if 's' not in p.data_flags]
     if len(props_without_alternates) == 0:
         raise PdgNoDataError('No best property found%s' % for_what)
     elif len(props_without_alternates) == 1:
         return props_without_alternates[0]
     else:
-        if is_generic or pedantic:
+        if pedantic:
             err = 'Ambiguous best property%s' % for_what
-            if is_generic:
-                err += '. This is a generic charge state; try selecting a specific charge (e.g. by setting the MC ID)'
             raise PdgAmbiguousValueError(err)
         else:
             props_best = [p for p in props_without_alternates if 'D' in p.data_flags]
             if len(props_best) >= 1:
                 return props_best[0]
             else:
                 return props_without_alternates[0]
```

### Comparing `pdg-0.0.6/setup.py` & `pdg-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,40 +10,45 @@
     def _get_rc_file(self):
         return os.path.join('.', '.pypirc')
 
 
 # Standard package setup
 from setuptools import setup, find_packages
 
-with open("README.md","r") as fh:
+with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    name = 'pdg',
-    version = '0.0.6',
-    author = 'Particle Data Group',
-    author_email = 'jberinger@lbl.gov',
-    description = 'Python API for accessing PDG data',
-    long_description = long_description,
-    long_description_content_type = 'text/markdown',
-    url = 'https://pdg.lbl.gov',
-    license = 'Modified BSD',
-    packages = find_packages(),
+    name='pdg',
+    version='0.0.7',
+    author='Particle Data Group',
+    author_email='jberinger@lbl.gov',
+    description='Python API for accessing PDG data',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://pdg.lbl.gov',
+    license='Modified BSD',
+    packages=find_packages(),
     package_data={"pdg": ["pdg.sqlite"]},
-    install_requires = ['SQLAlchemy>=1.4'],
-    classifiers = [
+    install_requires=['SQLAlchemy>=1.4'],
+    classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Topic :: Database :: Front-Ends',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Physics'
         ],
-    keywords = 'PDG, particle physics',
+    keywords='PDG, particle physics',
+    project_urls={
+        'Documentation': 'https://pdgapi.lbl.gov/doc/',
+        'GitHub': 'https://github.com/particledatagroup/api',
+        'Changelog': 'https://github.com/particledatagroup/api/blob/main/README.md'
+    },
     cmdclass={
         'register': register,
         'upload': upload
         }
 )
```

