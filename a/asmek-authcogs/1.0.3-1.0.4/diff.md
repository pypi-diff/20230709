# Comparing `tmp/asmek_authcogs-1.0.3.tar.gz` & `tmp/asmek_authcogs-1.0.4.tar.gz`

## Comparing `asmek_authcogs-1.0.3.tar` & `asmek_authcogs-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/CHANGELOG.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/__init__.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/app_settings.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/apps.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/auth_hooks.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/Images/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/Images/eve-o-4.png
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/Images/smt_bomb_icon-1.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/cogs/__init__.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/cogs/about.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/cogs/auth.py
--rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/cogs/links.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/migrations/0001_initial.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/migrations/0002_alter_link_name.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/asmek_authcogs/migrations/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/LICENSE
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/README.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/__init__.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/app_settings.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/apps.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/auth_hooks.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/Images/__init__.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/Images/eve-o-4.png
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/Images/smt_bomb_icon-1.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/cogs/__init__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/cogs/about.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/cogs/auth.py
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/cogs/links.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/migrations/0001_initial.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/migrations/0002_alter_link_name.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/asmek_authcogs/migrations/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/LICENSE
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/README.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 asmek_authcogs-1.0.4/PKG-INFO
```

### Comparing `asmek_authcogs-1.0.3/CHANGELOG.md` & `asmek_authcogs-1.0.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/.github/workflows/publish.yml` & `asmek_authcogs-1.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/asmek_authcogs/models.py` & `asmek_authcogs-1.0.4/asmek_authcogs/models.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/asmek_authcogs/Images/eve-o-4.png` & `asmek_authcogs-1.0.4/asmek_authcogs/Images/eve-o-4.png`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/asmek_authcogs/Images/smt_bomb_icon-1.png` & `asmek_authcogs-1.0.4/asmek_authcogs/Images/smt_bomb_icon-1.png`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/asmek_authcogs/cogs/about.py` & `asmek_authcogs-1.0.4/asmek_authcogs/cogs/about.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/asmek_authcogs/cogs/auth.py` & `asmek_authcogs-1.0.4/asmek_authcogs/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/asmek_authcogs/cogs/links.py` & `asmek_authcogs-1.0.4/asmek_authcogs/cogs/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,29 +154,27 @@
 
                 await interaction.response.send_message(msg, ephemeral=True)
             except Exception as e:
                 await interaction.response.send_message(e, ephemeral=True)
             self.stop()
 
     @links_commands.command(name="list", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    # @sender_has_perm("link.manage_links")
+    @sender_has_perm("link.manage_links")
     async def list(self, ctx):
         """
         list all current links
         """
         embed = Embed()
         embed.title = "All the links!!"
         embed.description = f"A list of all links currently stored by the auth bot!"
         await ctx.defer(ephemeral=False)
         links = Link.objects.all()
         if links.count() > 0:
             for i in links:
-                embed.add_field(
-                    name=f"{i.name}: {i.description}", value=i.url, inline=False
-                )
+                embed.add_field(name=f"{i.name}", value=i.url, inline=False)
         else:
             embed.description = f"No Links added!"
 
         await ctx.respond(embed=embed, ephemeral=False)
 
     # //=============================================================================
     # // Add, edit, delete commands
@@ -188,25 +186,25 @@
         """
         add new link
         """
         add_modal = Links.AddModal()
         await ctx.send_modal(add_modal)
 
     @links_commands.command(name="edit", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    # @sender_has_perm("link.manage_links")
+    @sender_has_perm("link.manage_links")
     @option("name", description="Search for a Link!", autocomplete=search_links)
     async def edit(self, ctx, name: str):
         """
         edit link
         """
         edit_modal = Links.EditModal(name)
         await ctx.send_modal(edit_modal)
 
     @links_commands.command(name="delete", guild_ids=[int(settings.DISCORD_GUILD_ID)])
-    # @sender_has_perm("link.manage_links")
+    @sender_has_perm("link.manage_links")
     @option("name", description="Search for a Link!", autocomplete=search_links)
     async def delete(self, ctx, name: str):
         """
         delete link
         """
         delete_modal = Links.DeleteModal(name)
         await ctx.send_modal(delete_modal)
```

### Comparing `asmek_authcogs-1.0.3/asmek_authcogs/migrations/0001_initial.py` & `asmek_authcogs-1.0.4/asmek_authcogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/.gitignore` & `asmek_authcogs-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/LICENSE` & `asmek_authcogs-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/README.md` & `asmek_authcogs-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/pyproject.toml` & `asmek_authcogs-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asmek_authcogs-1.0.3/PKG-INFO` & `asmek_authcogs-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asmek-authcogs
-Version: 1.0.3
+Version: 1.0.4
 Summary: ASMEK customized cogs for aa-discordbot
 Project-URL: Documentation, https://github.com/AstrumMechanica/asmek-authcogs#readme
 Project-URL: Issues, https://github.com/AstrumMechanica/asmek-authcogs/issues
 Project-URL: Source, https://github.com/AstrumMechanica/asmek-authcogs
 Author-email: AstrumMechanica <astrummechanica@gmail.com>
 License-Expression: GPL-3.0
 License-File: LICENSE
```

