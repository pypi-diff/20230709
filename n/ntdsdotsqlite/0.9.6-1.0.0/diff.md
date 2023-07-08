# Comparing `tmp/ntdsdotsqlite-0.9.6.tar.gz` & `tmp/ntdsdotsqlite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdsdotsqlite-0.9.6.tar", max compression
+gzip compressed data, was "ntdsdotsqlite-1.0.0.tar", max compression
```

## Comparing `ntdsdotsqlite-0.9.6.tar` & `ntdsdotsqlite-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-0.9.6/ntdsdotsqlite/__init__.py
--rw-r--r--   0        0        0      854 2023-05-08 16:23:21.892529 ntdsdotsqlite-0.9.6/ntdsdotsqlite/__main__.py
--rw-r--r--   0        0        0     5305 2023-05-25 17:10:04.235334 ntdsdotsqlite-0.9.6/ntdsdotsqlite/accounts.py
--rw-r--r--   0        0        0     1454 2023-05-08 09:43:59.572323 ntdsdotsqlite-0.9.6/ntdsdotsqlite/containers.py
--rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-0.9.6/ntdsdotsqlite/decrypt.py
--rw-r--r--   0        0        0     3089 2023-05-08 21:09:08.053917 ntdsdotsqlite-0.9.6/ntdsdotsqlite/domain.py
--rw-r--r--   0        0        0      905 2023-05-08 13:52:27.251046 ntdsdotsqlite-0.9.6/ntdsdotsqlite/groups.py
--rw-r--r--   0        0        0      320 2023-05-08 21:09:14.178994 ntdsdotsqlite-0.9.6/ntdsdotsqlite/links.py
--rw-r--r--   0        0        0     2958 2023-05-25 17:11:24.932653 ntdsdotsqlite-0.9.6/ntdsdotsqlite/model.sql
--rw-r--r--   0        0        0     5104 2023-05-25 17:13:31.077881 ntdsdotsqlite-0.9.6/ntdsdotsqlite/ntdsdotsqlite.py
--rw-r--r--   0        0        0     1769 2023-05-25 17:14:27.627333 ntdsdotsqlite-0.9.6/ntdsdotsqlite/orga_units.py
--rw-r--r--   0        0        0    26966 2023-05-09 20:30:13.020077 ntdsdotsqlite-0.9.6/ntdsdotsqlite/secretsdump.py
--rw-r--r--   0        0        0     2178 2023-05-25 17:13:23.481309 ntdsdotsqlite-0.9.6/ntdsdotsqlite/trusts.py
--rw-r--r--   0        0        0     6185 2023-05-25 17:13:16.795269 ntdsdotsqlite-0.9.6/ntdsdotsqlite/utils.py
--rw-r--r--   0        0        0      695 2023-05-25 18:12:55.859839 ntdsdotsqlite-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-0.9.6/README.md
--rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 ntdsdotsqlite-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-1.0.0/ntdsdotsqlite/__init__.py
+-rw-r--r--   0        0        0      852 2023-07-08 21:57:45.406401 ntdsdotsqlite-1.0.0/ntdsdotsqlite/__main__.py
+-rw-r--r--   0        0        0      389 2023-07-05 17:21:18.207904 ntdsdotsqlite-1.0.0/ntdsdotsqlite/basehandler.py
+-rw-r--r--   0        0        0     5536 2023-07-08 21:41:52.675922 ntdsdotsqlite-1.0.0/ntdsdotsqlite/computerhandler.py
+-rw-r--r--   0        0        0     2117 2023-07-08 19:51:20.130174 ntdsdotsqlite-1.0.0/ntdsdotsqlite/containerhandler.py
+-rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-1.0.0/ntdsdotsqlite/decrypt.py
+-rw-r--r--   0        0        0     4508 2023-07-07 17:30:48.617916 ntdsdotsqlite-1.0.0/ntdsdotsqlite/domainhandler.py
+-rw-r--r--   0        0        0     1788 2023-07-05 20:40:04.710251 ntdsdotsqlite-1.0.0/ntdsdotsqlite/grouphandler.py
+-rw-r--r--   0        0        0     2951 2023-07-08 21:49:06.058097 ntdsdotsqlite-1.0.0/ntdsdotsqlite/model.sql
+-rw-r--r--   0        0        0     5839 2023-07-08 22:19:51.689577 ntdsdotsqlite-1.0.0/ntdsdotsqlite/ntdsdotsqlite.py
+-rw-r--r--   0        0        0     2107 2023-07-08 20:19:52.784084 ntdsdotsqlite-1.0.0/ntdsdotsqlite/organizationalunithandler.py
+-rw-r--r--   0        0        0     5894 2023-07-08 21:37:05.683105 ntdsdotsqlite-1.0.0/ntdsdotsqlite/personhandler.py
+-rw-r--r--   0        0        0    26948 2023-07-05 17:06:07.989661 ntdsdotsqlite-1.0.0/ntdsdotsqlite/secretsdump.py
+-rw-r--r--   0        0        0     2076 2023-07-06 20:00:49.679037 ntdsdotsqlite-1.0.0/ntdsdotsqlite/trusteddomainhandler.py
+-rw-r--r--   0        0        0     3678 2023-07-08 22:04:51.106889 ntdsdotsqlite-1.0.0/ntdsdotsqlite/utils.py
+-rw-r--r--   0        0        0      713 2023-07-08 22:16:21.344278 ntdsdotsqlite-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-1.0.0/README.md
+-rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.0.0/PKG-INFO
```

### Comparing `ntdsdotsqlite-0.9.6/ntdsdotsqlite/__main__.py` & `ntdsdotsqlite-1.0.0/ntdsdotsqlite/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 import argparse
 
-
 from ntdsdotsqlite.ntdsdotsqlite import run
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog="NTDS.sqlite",
         description=(
```

### Comparing `ntdsdotsqlite-0.9.6/ntdsdotsqlite/decrypt.py` & `ntdsdotsqlite-1.0.0/ntdsdotsqlite/decrypt.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.6/ntdsdotsqlite/domain.py` & `ntdsdotsqlite-1.0.0/ntdsdotsqlite/containerhandler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,51 @@
-from ntdsdotsqlite.utils import get_schema_object, raw_to_guid, raw_to_sid
+from ntdsdotsqlite.basehandler import BaseHandler
 from ntdsdotsqlite.utils import escape_dn_chars
 
 
-def get_domain_objects(ese_db):
-    datatable = ese_db.table("datatable")
-    # Locate the ID of the domainDNS schema object
-    domainDNS_dnt, _ = get_schema_object(ese_db, "19195a5b-6da0-11d0-afd3-00c04fd930c9")
-    if domainDNS_dnt is None:
-        print("no domainDNS object ...")
-        exit(1)
-    domain_object = None
-    for row in datatable.records():
-        if (
-            (object_category := row.get(ese_db.column_names["objectCategory"])) and
-            object_category == domainDNS_dnt and
-            row.get(ese_db.column_names["msDS-Behavior-Version"])
-        ):
-            domain_object = row
-            # We only need the first object that represents the main domain
-            break
-    # go up in the tree to get the full domain name
-    cur_object = domain_object
-    parents = []
-    while True:
-        # If we got back to the root object (guid '00'*16, name='$ROOT_OBJECT$\u0000'), break
-        parent_dnt = cur_object.get("PDNT_col")
-        if parent_dnt == 2:
-            break
-        for row in datatable.records():
-            if row.get("DNT_col") == parent_dnt:
-                parents.append(row)
-                cur_object = row
-                break
-    func_levels = {
-        0: "2000", 2: "2003", 3: "2008", 4: "2008R2",
-        5: "2012", 6: "2012R2", 7: "2016"
-    }
-    domain = {
-        "id": domain_object.get("DNT_col"),
-        "netbios_name": domain_object.get(ese_db.column_names["name"]),
-        "name": ".".join([x.get(ese_db.column_names["name"]) for x in [domain_object, *parents]]),
-        "parents": parents,
-        "functional_level": (
-            func_levels[domain_object.get(ese_db.column_names["msDS-Behavior-Version"])]
-        ),
-        "GUID": raw_to_guid(domain_object.get(ese_db.column_names["objectGUID"])),
-        "gplink": domain_object.get(ese_db.column_names["gPLink"]),
-        "SID": raw_to_sid(domain_object.get(ese_db.column_names["objectSid"])),
-        "machineAccountQuota": domain_object.get(ese_db.column_names["ms-DS-MachineAccountQuota"]),
-        # max password age in seconds
-        "maxPwdAge": (
-            domain_object.get(ese_db.column_names["maxPwdAge"]) * -1 / 10000000
-        ),
-        # lockout duration in seconds
-        "lockoutDuration": (
-            domain_object.get(ese_db.column_names["lockoutDuration"]) * -1 / 10000000
-        ),
-        "minPwdLength": domain_object.get(ese_db.column_names["minPwdLength"]),
-        "pwdHistoryLength": domain_object.get(ese_db.column_names["pwdHistoryLength"]),
-        # minimum password age in seconds
-        "minPwdAge": (
-            domain_object.get(ese_db.column_names["minPwdAge"]) * -1 / 10000000
-        ),
-        "dn": "DC=" + ",DC=".join(
-            [
-                escape_dn_chars(x.get(ese_db.column_names["name"]))
-                for x in [domain_object, *parents]
-            ]
-        )
-    }
-    return domain
+class ContainerHandler(BaseHandler):
+    def handle(self, row):
+        container = {
+            "id": row.get("DNT_col"),
+            "name": row.get(self.attributes["name"]),
+            "cn": row.get(self.attributes["cn"]),
+            "description": row.get(self.attributes["description"]),
+            "parent": row.get("PDNT_col"),
+            "is_deleted": row.get(self.attributes["isDeleted"]) == 1
+        }
+        stmt = """
+            INSERT INTO containers VALUES (
+            :id, :name, :description, :cn, :parent, Null, :is_deleted
+            )
+        """
+        self.sqlite_db.execute(stmt, container)
+
+    def callback(self):
+        # compute DNs
+        roots = {domain_id: domain_DN for domain_id, domain_DN in self.sqlite_db.execute(
+            "SELECT id, dn FROM domain_dns"
+        ).fetchall()}
+        containers = {
+            c_id: {"id": c_id, "name": name, "parent": parent, "cn": cn}
+            for c_id, name, parent, cn in self.sqlite_db.execute(
+                "SELECT id, name, parent, commonname FROM containers"
+            ).fetchall()
+        }
+        for container in containers.values():
+            cur_object = container
+            parts = [f"CN={escape_dn_chars(cur_object['cn'])}"]
+            while True:
+                if cur_object["parent"] in containers.keys():
+                    cur_object = containers[cur_object["parent"]]
+                    parts.append(f"CN={escape_dn_chars(cur_object['cn'])}")
+                elif cur_object["parent"] in roots.keys():
+                    parts.append(roots[cur_object["parent"]])
+                    break
+                else:
+                    break
+            container["dn"] = ",".join(parts)
+            if ",DC=" not in container["dn"]:
+                container["dn"] = ""
+            self.sqlite_db.execute(
+                "UPDATE containers SET dn=? WHERE id=?", (container["dn"], container["id"])
+            )
+        self.sqlite_db.commit()
```

### Comparing `ntdsdotsqlite-0.9.6/ntdsdotsqlite/ntdsdotsqlite.py` & `ntdsdotsqlite-1.0.0/ntdsdotsqlite/personhandler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,131 +1,126 @@
-from ntdsdotsqlite.utils import create_database, get_ESE_column_names
-from ntdsdotsqlite.containers import containers_generator
-from ntdsdotsqlite.accounts import account_generator
-from ntdsdotsqlite.domain import get_domain_objects
-from ntdsdotsqlite.orga_units import ou_generator
-from ntdsdotsqlite.decrypt import decrypt_sqlite
-from ntdsdotsqlite.trusts import trust_generator
-from ntdsdotsqlite.groups import group_generator
-from ntdsdotsqlite.links import compute_links
-from dissect.esedb import EseDB
-import sqlite3
+from ntdsdotsqlite.utils import hundredns_to_datetime, UAC_FLAGS
+from ntdsdotsqlite.utils import raw_to_guid, raw_to_sid
+from ntdsdotsqlite.basehandler import BaseHandler
+from ntdsdotsqlite.utils import escape_dn_chars
+
 import json
 
 
-def run(ese_path, outpath, system_path):
-    create_database(outpath)
-    sqlite_db = sqlite3.connect(outpath)
-    fd = open(ese_path, "rb")
-    ese_db = EseDB(fd)
-    cursor = sqlite_db.cursor()
-    # Getting column names
-    column_names = get_ESE_column_names(ese_db)
-    ese_db.column_names = column_names
-    # Compute links
-    print("Retrieving and storing links information ...")
-    link_relations = compute_links(ese_db)
-    # Get the domain
-    print("Retrieving the domain object ...")
-    domain = get_domain_objects(ese_db)
-    # Insert the domain record
-    stmt = (
-        "INSERT INTO domains VALUES(:id, :name, :netbios_name, :functional_level, :GUID, :gplink,"
-        ":SID, :machineAccountQuota, :maxPwdAge, :lockoutDuration, :minPwdLength, :pwdHistoryLength"
-        ", :minPwdAge, :dn)"
-    )
-    cursor.execute(stmt, domain)
-    sqlite_db.commit()
-    # Insert container objects
-    print("Retrieving containers objects ...")
-    stmt = """
-        INSERT INTO containers VALUES (
-        :id, :name, :description, :cn, :parent, :dn, :is_deleted
-        )
-    """
-    cursor.executemany(stmt, containers_generator(ese_db, sqlite_db))
-    sqlite_db.commit()
-    # Insert ou objects records
-    stmt = """
-        INSERT INTO organizational_units VALUES (
-        :id, :name, :description, :parent, :dn, :isDeleted
-        )
-    """
-    print("Retrieving organizational units objects ...")
-    cursor.executemany(stmt, ou_generator(ese_db))
-    sqlite_db.commit()
-    # Insert group objects
-    print("Retrieving groups objects ...")
-    stmt = f"""
-        INSERT INTO groups VALUES (
-        :id, :name, :cn, :samaccountname, :SID, {domain['id']},
-        :is_deleted, :description, ""
-        )
-    """
-    cursor.executemany(stmt, group_generator(ese_db))
-    sqlite_db.commit()
-    # # Handle groups memberships with themselves
-    for row in cursor.execute("SELECT id FROM groups"):
-        memberOf = []
-        new_cur = sqlite_db.cursor()
-        for link in link_relations[row[0]]:
-            res = new_cur.execute(f"SELECT id FROM groups WHERE id={link}")
-            res = res.fetchone()
-            if res is not None:
-                memberOf.append(link)
-        new_cur.execute(
-            "UPDATE groups SET memberOf=? WHERE id=?", (json.dumps(memberOf), row[0])
-        )
-    sqlite_db.commit()
-    # Insert all user account records
-    print("Retrieving user accounts objects ...")
-    accounts_iter = account_generator(
-        ese_db, "bf967aa7-0de6-11d0-a285-00aa003049e2",
-        sqlite_db, link_relations
-    )
-    stmt = f"""
-        INSERT INTO user_accounts VALUES (
-        :id, :nthash, :lmhash, :UAC, :description, :lastLogonTimestamp,
-        :pwdLastSet, :adminCount, :displayName, :GUID, :SID, :SPN,
-        {domain['id']}, :UPN, :login, :samaccountname, :commonname,
-        :supplementalCredentials, :lmPwdHistory, :ntPwdHistory, :accountExpires,
-        :uac_flags, :parent, :dn, :isDeleted, :primaryGroup,
-        :memberOf, :links, :isDisabled
-        )
-    """
-    cursor.executemany(stmt, accounts_iter)
-    sqlite_db.commit()
-    # Insert all machine account records
-    print("Retrieving machine accounts objects ...")
-    machines_iter = account_generator(
-        ese_db, "bf967a86-0de6-11d0-a285-00aa003049e2",
-        sqlite_db, link_relations
-    )
-    stmt = f"""
-        INSERT INTO machine_accounts VALUES (
-        :id, :nthash, :lmhash, :UAC, :description, :lastLogonTimestamp,
-        :pwdLastSet, :adminCount, :displayName, :GUID, :SID, :SPN,
-        {domain['id']}, :UPN, :login, :samaccountname, :commonname,
-        :supplementalCredentials, :lmPwdHistory, :ntPwdHistory, :accountExpires,
-        :uac_flags, :parent, :dn, :isDeleted, :primaryGroup, :links,
-        :isDisabled
-        )
-    """
-    cursor.executemany(stmt, machines_iter)
-    sqlite_db.commit()
-    # Insert trust information
-    print("Retrieving trust information with other domains...")
-    trusts_iter = trust_generator(ese_db)
-    stmt = """
-        INSERT INTO trusted_domains VALUES (
-        :id, :commonname, :name, :trustAttributes, :trustDirection, :trustPartner, :trustType,
-        :attributeFlags
-        )
-    """
-    cursor.executemany(stmt, trusts_iter)
-    sqlite_db.commit()
-    if system_path:
-        print("Decrypting stuff with SYSTEM hive ...")
-        decrypt_sqlite(sqlite_db, ese_path, system_path)
-    if sqlite_db:
-        sqlite_db.close()
-    fd.close()
+class PersonHandler(BaseHandler):
+    def __init__(self, links, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.links = links
+
+    def handle(self, row):
+        lastLogonTimestamp = row.get(self.attributes["lastLogonTimestamp"])
+        pwdlastset = row.get(self.attributes["pwdLastSet"])
+        if pwdlastset:
+            pwdlastset = hundredns_to_datetime(pwdlastset)
+        if lastLogonTimestamp:
+            lastLogonTimestamp = hundredns_to_datetime(lastLogonTimestamp)
+        admincount = row.get(self.attributes["adminCount"])
+        if admincount is None:
+            admincount = 0
+        spn = row.get(self.attributes["servicePrincipalName"])
+        accountExpires = row.get(self.attributes["accountExpires"])
+        if accountExpires:
+            if accountExpires and accountExpires == 0 or accountExpires == 0x7FFFFFFFFFFFFFFF:
+                accountExpires = 0
+            else:
+                accountExpires = hundredns_to_datetime(accountExpires)
+        uac = row.get(self.attributes["userAccountControl"])
+        sid = row.get(self.attributes["objectSid"])
+        guid = row.get(self.attributes["objectGUID"])
+        account = {
+            "id": row.get("DNT_col"), "description": row.get(self.attributes["description"]),
+            "UAC": uac,
+            "SID": raw_to_sid(sid) if sid else None,
+            "samaccountname": row.get(self.attributes["sAMAccountName"]),
+            # unix epoch or NULL if password never set
+            "pwdLastSet": pwdlastset,
+            "nthash": row.get(self.attributes["unicodePwd"]),
+            "commonname": row.get(self.attributes["cn"]),
+            "GUID": raw_to_guid(guid) if guid else None,
+            "adminCount": admincount,
+            "displayName": row.get(self.attributes["displayName"]),
+            "UPN": row.get(self.attributes["userPrincipalName"]),
+            "supplementalCredentials": row.get(self.attributes["supplementalCredentials"]),
+            # unix epoch
+            "lastLogonTimestamp": lastLogonTimestamp,
+            "lmPwdHistory": row.get(self.attributes["lmPwdHistory"]),
+            "ntPwdHistory": row.get(self.attributes["ntPwdHistory"]),
+            "accountExpires": accountExpires,
+            "SPN": spn,
+            "lmhash": row.get(self.attributes["dBCSPwd"]),
+            "parent": row.get("PDNT_col"),
+            "isDeleted": row.get(self.attributes["isDeleted"]) == 1,
+            "primaryGroup": row.get(self.attributes["primaryGroupID"])
+        }
+        account["login"] = (
+            account["UPN"].split("@")[0] if account["UPN"]
+            else account["samaccountname"]
+        )
+        if (spn := account["SPN"]):
+            if type(spn) is str:
+                account["SPN"] = json.dumps([spn])
+            elif type(spn) is list:
+                account["SPN"] = json.dumps(spn)
+            else:
+                print(f"SPN type unknown : {spn} - {type(spn)}")
+                print(account)
+                exit(1)
+        if uac:
+            uac_flags = {
+                k.name: True if uac & k.value else False for k in UAC_FLAGS
+            }
+            account["uac_flags"] = json.dumps(uac_flags)
+            account["isDisabled"] = uac_flags["ACCOUNTDISABLE"]
+        else:
+            account["uac_flags"] = None
+            account["isDisabled"] = None
+        stmt = """
+            INSERT INTO user_accounts VALUES (
+            :id, :nthash, :lmhash, :UAC, :description, :lastLogonTimestamp,
+            :pwdLastSet, :adminCount, :displayName, :GUID, :SID, :SPN,
+            Null, :UPN, :login, :samaccountname, :commonname,
+            :supplementalCredentials, :lmPwdHistory, :ntPwdHistory, :accountExpires,
+            :uac_flags, :parent, Null, :isDeleted, :primaryGroup,
+            Null, :isDisabled
+            )
+        """
+        self.sqlite_db.execute(stmt, account)
+
+    def callback(self):
+        # set the domain id
+        domain_id = self.sqlite_db.execute("SELECT id FROM domains").fetchone()[0]
+        ous = {
+            oid: dn for oid, dn in self.sqlite_db.execute("SELECT id, dn FROM organizational_units")
+        }
+        users = self.sqlite_db.execute(
+            "SELECT id, commonname, parent_OU, primaryGroup FROM user_accounts"
+        )
+        containers = {
+            cid: cdn for (cid, cdn) in self.sqlite_db.execute("SELECT id, dn FROM containers")
+        }
+        domains = {
+            did: ddn for (did, ddn) in self.sqlite_db.execute("SELECT id, dn FROM domain_dns")
+        }
+        group_ids = [x[0] for x in self.sqlite_db.execute("SELECT id FROM groups").fetchall()]
+        for uid, cn, parent_OU, primaryGroup in users:
+            # Compute DN
+            if parent_OU in ous.keys():
+                dn = f"CN={escape_dn_chars(cn)},{ous[parent_OU]}"
+            elif parent_OU in containers.keys():
+                dn = f"CN={escape_dn_chars(cn)},{containers[parent_OU]}"
+            elif parent_OU in domains.keys():
+                dn = f"CN={escape_dn_chars(cn)},{domains[parent_OU]}"
+            else:
+                print(f"Warning: could not compute DN of user {cn}")
+            links_list = self.links[uid]
+            memberof = json.dumps([link for link in links_list if link in group_ids])
+            self.sqlite_db.execute(
+                "UPDATE user_accounts set domain=?, memberOf=?, primaryGroup=("
+                f"SELECT id from groups WHERE SID LIKE '%-{primaryGroup}'"
+                "), dn=? WHERE id=?",
+                (domain_id, memberof, dn, uid)
+            )
```

### Comparing `ntdsdotsqlite-0.9.6/ntdsdotsqlite/orga_units.py` & `ntdsdotsqlite-1.0.0/ntdsdotsqlite/organizationalunithandler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,53 @@
-from ntdsdotsqlite.domain import get_domain_objects
-from ntdsdotsqlite.utils import get_schema_object
+from ntdsdotsqlite.basehandler import BaseHandler
 from ntdsdotsqlite.utils import escape_dn_chars
 
 
-def ou_generator(ese_db):
-    dnt_cat, _ = get_schema_object(ese_db, "bf967aa5-0de6-11d0-a285-00aa003049e2")
-    datatable = ese_db.table("datatable")
-    ous = filter(
-        lambda row: (cat := row.get(ese_db.column_names["objectCategory"])) and cat == dnt_cat,
-        datatable.records()
-    )
-    ous = {
-        ou.get("DNT_col"): ou for ou in ous
-    }
-
-    domain = get_domain_objects(ese_db)
-    domain_id = domain["id"]
-    dn_suffix = domain["dn"]
-    for ou_id, ou in ous.items():
+class OrganizationalUnitHandler(BaseHandler):
+    def handle(self, row):
         ou_object = {
-            "id": ou_id,
-            "description": ou.get(ese_db.column_names["description"]),
-            "name": ou.get(ese_db.column_names["name"]),
-            "parent": ou.get("PDNT_col"),
-            "isDeleted": ou.get(ese_db.column_names["isDeleted"]) == 1
+            "id": row.get("DNT_col"),
+            "description": row.get(self.attributes["description"]),
+            "name": row.get(self.attributes["name"]),
+            "parent": row.get("PDNT_col"),
+            "isDeleted": row.get(self.attributes["isDeleted"]) == 1
+        }
+        stmt = """
+            INSERT INTO organizational_units VALUES (
+            :id, :name, :description, :parent, Null, :isDeleted
+            )
+        """
+        self.sqlite_db.execute(stmt, ou_object)
+
+    def callback(self):
+        # Compute DNs
+        roots = {domain_id: domain_DN for domain_id, domain_DN in self.sqlite_db.execute(
+            "SELECT id, dn FROM domain_dns"
+        ).fetchall()}
+        ous = self.sqlite_db.execute("SELECT id, parent, name FROM organizational_units").fetchall()
+        ous = {
+            ou_id: {"id": ou_id, "name": name, "parent": parent}
+            for ou_id, parent, name in ous
         }
-        # get the full path of the OU
-        dn_prefix = "OU=" + escape_dn_chars(ou_object["name"])
-        cur_object = ou
-        while True:
-            parent_dnt = cur_object.get("PDNT_col")
-            # if $ROOT_OBJECT" is reached or the current object is not an OU anymore
-            if parent_dnt == domain_id:
-                break
-            try:
-                parent = ous[parent_dnt]
-            except KeyError:
-                print(f"Warning: the OU {ou_object['name']} has a missing parent in its path...")
-                break
-            cur_object = parent
-            name = parent.get(ese_db.column_names["name"])
-            dn_prefix += "," + "OU=" + escape_dn_chars(name)
-        ou_object["dn"] = f"{dn_prefix},{dn_suffix}"
-        yield ou_object
+        for ou_id, ou in ous.items():
+            dn_prefix = "OU=" + escape_dn_chars(ou["name"])
+            cur_object = ou
+            while True:
+                parent_dnt = cur_object["parent"]
+                if parent_dnt in ous.keys():
+                    parent = ous[parent_dnt]
+                elif parent_dnt in roots.keys():
+                    dn_prefix += ("," + roots[parent_dnt])
+                    break
+                else:
+                    print(
+                        f"Warning: could not compute DN of OU {cur_object['name']}."
+                    )
+                    break
+                cur_object = parent
+                name = parent["name"]
+                dn_prefix += "," + "OU=" + escape_dn_chars(name)
+            self.sqlite_db.execute(
+                "UPDATE organizational_units SET dn=? WHERE id=?",
+                (dn_prefix, ou_id)
+            )
+        self.sqlite_db.commit()
```

### Comparing `ntdsdotsqlite-0.9.6/ntdsdotsqlite/secretsdump.py` & `ntdsdotsqlite-1.0.0/ntdsdotsqlite/secretsdump.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,19 +344,17 @@
 
                 if cipherText['Header'][:4] == b'\x13\x00\x00\x00':
                     # Win2016 TP4 decryption is different
                     pekIndex = hexlify(cipherText['Header'])
                     plainText = self.__cryptoCommon.decryptAES(self.__PEK[int(pekIndex[8:10])],
                                                                cipherText['EncryptedHash'][4:],
                                                                cipherText['KeyMaterial'])
-                    haveInfo = True
                 else:
                     plainText = self.__removeRC4Layer(cipherText)
-                    haveInfo = True
-
+                haveInfo = len(plainText) > 0x6f + 2 + 4
         if haveInfo:
             answers = []
             try:
                 userProperties = samr.USER_PROPERTIES(plainText)
             except:
                 # On some old w2k3 there might be user properties that don't
                 # match [MS-SAMR] structure, discarding them
```

### Comparing `ntdsdotsqlite-0.9.6/ntdsdotsqlite/trusts.py` & `ntdsdotsqlite-1.0.0/ntdsdotsqlite/trusteddomainhandler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,33 @@
-from ntdsdotsqlite.utils import get_schema_object, raw_to_guid, raw_to_sid
+from ntdsdotsqlite.utils import raw_to_guid, raw_to_sid
+from ntdsdotsqlite.basehandler import BaseHandler
 from ntdsdotsqlite.utils import TRUST_FLAGS
 import json
 
 
-# yields dictionaries representing accounts (users or machines) based
-# on the schema_guid (string) given in parameters.
-def trust_generator(ese_db):
-    dnt_cat, _ = get_schema_object(ese_db, "bf967ab8-0de6-11d0-a285-00aa003049e2")
-    datatable = ese_db.table("datatable")
-
-    trusts = filter(
-        lambda row: row.get(ese_db.column_names["objectCategory"]) == dnt_cat,
-        datatable.records()
-    )
-    for trust in trusts:
-        sid = trust.get(ese_db.column_names["objectSid"])
+class TrustedDomainHandler(BaseHandler):
+    def handle(self, row):
+        sid = row.get(self.attributes["objectSid"])
         sid = raw_to_sid(sid) if sid else None,
-        dnt_id = trust.get("DNT_col")
-        guid = trust.get(ese_db.column_names["objectGUID"])
+        dnt_id = row.get("DNT_col")
+        guid = row.get(self.attributes["objectGUID"])
         guid = raw_to_guid(guid) if guid else None
-        commonname = trust.get(ese_db.column_names["cn"])
-        name = trust.get(ese_db.column_names["name"])
-        trustattributes = trust.get(ese_db.column_names["trustAttributes"])
+        commonname = row.get(self.attributes["cn"])
+        name = row.get(self.attributes["name"])
+        trustattributes = row.get(self.attributes["trustAttributes"])
         trustdirection = (
-            "disabled" if (direction := trust.get(ese_db.column_names["trustDirection"])) == 0 else
+            "disabled" if (direction := row.get(self.attributes["trustDirection"])) == 0 else
             "inbound" if direction == 1 else
             "outbound" if direction == 2 else
             "bidirectional" if direction == 3 else
             None
         )
-        trustpartner = trust.get(ese_db.column_names["trustPartner"])
+        trustpartner = row.get(self.attributes["trustPartner"])
         trusttype = (
-            "downlevel" if (ttype := trust.get(ese_db.column_names["trustType"])) == 1 else
+            "downlevel" if (ttype := row.get(self.attributes["trustType"])) == 1 else
             "uplevel" if ttype == 2 else
             "MIT" if ttype == 3 else
             "DCE" if ttype == 4 else
             None
         )
         attribute_flags = {
             f.name: True if trustattributes & f.value else False for f in TRUST_FLAGS
@@ -46,8 +38,17 @@
             "name": name,
             "trustAttributes": trustattributes,
             "attributeFlags": json.dumps(attribute_flags),
             "trustDirection": trustdirection,
             "trustPartner": trustpartner,
             "trustType": trusttype
         }
-        yield trust
+        stmt = """
+            INSERT INTO trusted_domains VALUES (
+            :id, :commonname, :name, :trustAttributes, :trustDirection, :trustPartner, :trustType,
+            :attributeFlags
+            )
+        """
+        self.sqlite_db.execute(stmt, trust)
+
+    def callback(self):
+        pass
```

### Comparing `ntdsdotsqlite-0.9.6/pyproject.toml` & `ntdsdotsqlite-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "ntdsdotsqlite"
-version = "0.9.6"
+version = "1.0.0"
 description = "A small utility to get an SQLite  database from an NTDS.DIT file."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/ntdsdotsqlite"
 repository = "https://github.com/almandin/ntdsdotsqlite"
 documentation = "https://github.com/almandin/ntdsdotsqlite/README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dissect = {extras = ["ese"], version = "^3.5"}
 impacket = "^0.10"
+tqdm = "^4.65.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ntdsdotsqlite = 'ntdsdotsqlite.__main__:main'
```

### Comparing `ntdsdotsqlite-0.9.6/README.md` & `ntdsdotsqlite-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.6/PKG-INFO` & `ntdsdotsqlite-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ntdsdotsqlite
-Version: 0.9.6
+Version: 1.0.0
 Summary: A small utility to get an SQLite  database from an NTDS.DIT file.
 Home-page: https://github.com/almandin/ntdsdotsqlite
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dissect[ese] (>=3.5,<4.0)
 Requires-Dist: impacket (>=0.10,<0.11)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Documentation, https://github.com/almandin/ntdsdotsqlite/README.md
 Project-URL: Repository, https://github.com/almandin/ntdsdotsqlite
 Description-Content-Type: text/markdown
 
 # NTDS.Sqlite
 
 This software can be used either directly as a CLI utility or as a library to get an SQLite database from an NTDS.DIT one. Encrypted bits can be decrypted if the associated system hive is provided altogether.
```

