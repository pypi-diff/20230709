# Comparing `tmp/qtgql-0.126.0.tar.gz` & `tmp/qtgql-0.127.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.126.0.tar", max compression
+gzip compressed data, was "qtgql-0.127.0.tar", max compression
```

## Comparing `qtgql-0.126.0.tar` & `qtgql-0.127.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1064 2023-07-06 13:59:11.626132 qtgql-0.126.0/LICENSE
--rw-r--r--   0        0        0     1055 2023-07-06 13:59:11.626132 qtgql-0.126.0/README.md
--rw-r--r--   0        0        0     4428 2023-07-06 13:59:33.299759 qtgql-0.126.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1939 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1685 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3091 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     3366 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    14721 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      864 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4237 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8512 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1699 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3347 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     1890 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0      448 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
--rw-r--r--   0        0        0     1060 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
--rw-r--r--   0        0        0     4706 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     2994 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
--rw-r--r--   0        0        0     5049 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     5220 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3237 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    18075 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1147 2023-07-06 13:59:11.638133 qtgql-0.126.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.126.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-09 18:31:46.802182 qtgql-0.127.0/LICENSE
+-rw-r--r--   0        0        0     1055 2023-07-09 18:31:46.802182 qtgql-0.127.0/README.md
+-rw-r--r--   0        0        0     4428 2023-07-09 18:32:06.498201 qtgql-0.127.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1939 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1685 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3091 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     3366 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    14721 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      864 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4237 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1699 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4353 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     2933 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0      448 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/iterate_type_condition.jinja.hpp
+-rw-r--r--   0        0        0     1060 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     4706 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     4041 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp
+-rw-r--r--   0        0        0     5049 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     5220 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3237 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    18213 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1147 2023-07-09 18:31:46.818182 qtgql-0.127.0/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 qtgql-0.127.0/PKG-INFO
```

### Comparing `qtgql-0.126.0/LICENSE` & `qtgql-0.127.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/README.md` & `qtgql-0.127.0/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/pyproject.toml` & `qtgql-0.127.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.126.0"
+version = "0.127.0"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.126.0/qtgqlcodegen/cli.py` & `qtgql-0.127.0/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/config.py` & `qtgql-0.127.0/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.127.0/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.127.0/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/core/template.py` & `qtgql-0.127.0/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/generator.py` & `qtgql-0.127.0/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.127.0/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.127.0/qtgqlcodegen/operation/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/operation/template.py` & `qtgql-0.127.0/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.127.0/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.127.0/qtgqlcodegen/schema/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/schema/template.py` & `qtgql-0.127.0/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.127.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.127.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -6,20 +6,37 @@
 
 {% if field.type.is_queried_object_type  and field.type.is_optional %}
 if (👉 instance_of_concrete 👈){
 👉field.private_name👈 = new 👉field.type_name👈(👉operation_pointer👈, 👉 instance_of_concrete 👈);
 }
 {% elif field.type.is_queried_object_type %}
 👉field.private_name👈 = new 👉field.type_name👈(👉operation_pointer👈, 👉 instance_of_concrete 👈);
-{% elif field.type.is_model and field.type.is_model.of_type.is_queried_object_type %}
-auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.type.of_type.name👈*>>();
-for (const auto & node: 👉 instance_of_concrete 👈){
-init_list_👉 field.name 👈->append(new 👉field.type.of_type.name👈(👉operation_pointer👈, node));
-}
-👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.name 👈>(this, std::move(init_list_👉 field.name 👈));
+{% elif field.type.is_model  %}
+    {% if  field.type.is_model.of_type.is_queried_object_type %}
+    auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.type.of_type.name👈*>>();
+    for (const auto & node: 👉 instance_of_concrete 👈){
+    init_list_👉 field.name 👈->append(new 👉field.type.of_type.name👈(👉operation_pointer👈, node));
+    }
+    👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.name 👈>(this, std::move(init_list_👉 field.name 👈));
+    {% elif field.type.is_model.of_type.is_queried_union %}
+    auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.type.of_type.property_type👈>>();
+    for (const auto & node: 👉 instance_of_concrete 👈){
+        auto 👉field.name👈_typename = node->__typename();
+        {%set type_cond -%}👉field.name👈_typename{% endset -%}
+        {% for choice in field.type.of_type.choices -%}
+        {% set do_on_meets -%}
+        init_list_👉 field.name 👈->append(qobject_cast<👉 field.type.of_type.property_type 👈>(new 👉choice.type_name()👈(👉operation_pointer👈, std::static_pointer_cast<👉 choice.concrete.name 👈>(node))));
+        {% endset -%}
+        👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
+        {% endfor %}
+    }
+    👉field.private_name👈 = new qtgql::bases::ListModelABC<👉 field.type.of_type.type_name() 👈>(this, std::move(init_list_👉 field.name 👈));
+    {% else %}
+    not implemented
+    {% endif %}
 {% elif field.type.is_queried_interface or  field.type.is_queried_union %}
 auto concrete_👉field.name👈 = 👉 instance_of_concrete 👈;
 auto 👉field.name👈_typename = concrete_👉field.name👈->__typename();
 {%set type_cond -%}👉field.name👈_typename{% endset -%}
 {% for choice in field.type.choices -%}
 {% set do_on_meets -%}
 👉field.private_name👈 = qobject_cast<👉 field.type.property_type 👈>(new 👉choice.type_name()👈(👉operation_pointer👈, std::static_pointer_cast<👉 choice.concrete.name 👈>(concrete_👉field.name👈)));
```

### Comparing `qtgql-0.126.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp` & `qtgql-0.127.0/qtgqlcodegen/templates/macros/proxy_type_fields.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.127.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp` & `qtgql-0.127.0/qtgqlcodegen/templates/macros/update_proxy_field.jinja.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,63 @@
 {%- from "macros/iterate_type_condition.jinja.hpp" import  iterate_type_condition -%}
 {% macro update_proxy_field(field, operation) -%}
 {% set new_concrete -%}
 m_inst->👉field.concrete.getter_name👈(👉field.build_variables_tuple_for_field_arguments 👈)
 {%- endset -%}
 auto operation = m_operation;
 {% if field.type.is_model -%}
-    {% if field.type.of_type.is_queried_object_type -%}
-    {#- // the nodes themselves are updated as per normal (via deserializers) and here we only need
-        // to set the nodes at the correct index and append them if they weren't existed so far.
-    -#}
     auto new_data = 👉new_concrete👈;
     auto new_len = new_data.size();
     auto prev_len = 👉field.private_name👈->rowCount();
     if (new_len < prev_len){
         👉field.private_name👈->removeRows(prev_len - 1, prev_len - new_len);
     }
     for (int i = 0; i < new_len; i++){
         auto concrete = new_data.at(i);
+    {% if field.type.of_type.is_queried_object_type -%}
         if (i > prev_len - 1){
             👉field.private_name👈->insert(i, new 👉field.type.of_type.name👈(operation, concrete));
         }
         else {
             auto proxy_to_update = 👉field.private_name👈->get(i);
             if(proxy_to_update){
                 proxy_to_update->qtgql_replace_concrete(concrete);
             }
             else{
                 👉field.private_name👈->insert(i, new 👉field.type.of_type.name👈(operation, concrete));
             }
         }
-    }
+
+    {% elif field.type.of_type.is_queried_union %}
+        auto 👉field.name👈_typename = concrete->__typename();
+        {%set type_cond -%}👉field.name👈_typename{% endset -%}
+        {% for choice in field.type.of_type.choices %}
+        {% set do_on_meets -%}
+        if (i > prev_len - 1){
+            👉field.private_name👈->insert(i, new 👉choice.name👈(operation, std::static_pointer_cast<👉choice.concrete.name👈>(concrete)));
+        }
+        else{
+            auto proxy_to_update = 👉field.private_name👈->get(i);
+            if (proxy_to_update && proxy_to_update->__typename() == "👉choice.concrete.name👈"){
+                qobject_cast<👉choice.property_type👈>(proxy_to_update)->qtgql_replace_concrete(std::static_pointer_cast<👉choice.concrete.name👈>(concrete));
+            }
+            else{
+                delete proxy_to_update; {# // might have been optional or the type_name changed #}
+                👉field.private_name👈->insert(i, new 👉choice.name👈(operation, std::static_pointer_cast<👉choice.concrete.name👈>(concrete)));
+            }
+
+        }
+
+        {% endset %}
+        👉iterate_type_condition(choice,type_cond, do_on_meets, loop)👈
+        {% endfor %}
     {% else %}
     throw qtgql::exceptions::NotImplementedError({"can't update model of 👉field.type.of_type.__class__👈"});
     {% endif %}
+    }
 {% elif field.type.is_queried_object_type -%}
 auto concrete = 👉new_concrete👈;
 if (👉field.private_name👈){
     👉field.private_name👈->qtgql_replace_concrete(concrete);
 }
 else{
     👉field.private_name👈 = new 👉field.type.name👈(operation, concrete);
```

### Comparing `qtgql-0.126.0/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.127.0/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.127.0/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.127.0/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/qtgqlcodegen/types.py` & `qtgql-0.127.0/qtgqlcodegen/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,16 @@
             "models have no valid type for schema concretes, call member_type",
         )
 
     @property
     def property_type(self) -> str:
         if self.of_type.is_queried_object_type:
             return f"qtgql::bases::ListModelABC<{self.of_type.type_name()}> *"
+        if self.of_type.is_queried_union:
+            return f"qtgql::bases::ListModelABC<{self.of_type.is_queried_union.type_name()}> *"
         raise NotImplementedError
 
 
 @define
 class QtGqlUnion(QtGqlTypeABC):
     types: tuple[QtGqlObjectType | QtGqlDeferredType, ...]
```

### Comparing `qtgql-0.126.0/qtgqlcodegen/utils.py` & `qtgql-0.127.0/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.126.0/PKG-INFO` & `qtgql-0.127.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.126.0
+Version: 0.127.0
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

