# Comparing `tmp/ezdxf-1.1.0b4.zip` & `tmp/ezdxf-1.1.0b5.zip`

## zipinfo {}

```diff
@@ -1,843 +1,843 @@
-Zip file size: 2119905 bytes, number of entries: 841
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/LICENSE
--rw-rw-rw-  2.0 fat      302 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/MANIFEST.in
--rw-rw-rw-  2.0 fat   102011 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/NEWS.md
--rw-rw-rw-  2.0 fat    69878 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/PKG-INFO
--rw-rw-rw-  2.0 fat     6142 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/README.md
--rw-rw-rw-  2.0 fat       55 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/requirements.txt
--rw-rw-rw-  2.0 fat       74 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/setup.cfg
--rw-rw-rw-  2.0 fat     5576 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/
--rw-rw-rw-  2.0 fat      567 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_config_file.py
--rw-rw-rw-  2.0 fat      541 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_env_var.py
--rw-rw-rw-  2.0 fat      410 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/conftest.py
--rw-rw-rw-  2.0 fat     1054 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_acad_table.py
--rw-rw-rw-  2.0 fat     4686 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_all_dimline_styles.py
--rw-rw-rw-  2.0 fat     4133 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_all_ellipse_transformations.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_anonymous_blocks.py
--rw-rw-rw-  2.0 fat      871 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_audit_critical_dxf_files.py
--rw-rw-rw-  2.0 fat     1603 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_audit_layouts.py
--rw-rw-rw-  2.0 fat     1726 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_complex_line_type_2.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_create_basic_graphics.py
--rw-rw-rw-  2.0 fat     1921 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_document_guid.py
--rw-rw-rw-  2.0 fat     1832 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_document_page_setup.py
--rw-rw-rw-  2.0 fat      998 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_dxf_info_scanning.py
--rw-rw-rw-  2.0 fat     1558 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_entities_iterator.py
--rw-rw-rw-  2.0 fat      934 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_fix_dulicate_handles.py
--rw-rw-rw-  2.0 fat     1901 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_geo.py
--rw-rw-rw-  2.0 fat     1250 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_groups.py
--rw-rw-rw-  2.0 fat      905 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_hpgl2_addon.py
--rw-rw-rw-  2.0 fat      630 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_ignore_junk_beyond_EOF.py
--rw-rw-rw-  2.0 fat     1155 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_launcher.py
--rw-rw-rw-  2.0 fat      631 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_leica_disto_r12.py
--rw-rw-rw-  2.0 fat      737 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_load_dxf_unicode_notation.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_mapbox_earcut.py
--rw-rw-rw-  2.0 fat     2230 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_mtext_columns.py
--rw-rw-rw-  2.0 fat     2392 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_mtext_explode_addon.py
--rw-rw-rw-  2.0 fat     1846 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_mtext_text_frame.py
--rw-rw-rw-  2.0 fat     1053 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_new_table_entries.py
--rw-rw-rw-  2.0 fat      887 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_none_ascii_read_write.py
--rw-rw-rw-  2.0 fat     3435 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_odafc.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_open_binary_DXF_files.py
--rw-rw-rw-  2.0 fat      751 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_open_coord_order_issue.py
--rw-rw-rw-  2.0 fat     3842 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_open_exotic_dxf_files.py
--rw-rw-rw-  2.0 fat      879 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_open_R13_R14.py
--rw-rw-rw-  2.0 fat     3152 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_polyline_entity.py
--rw-rw-rw-  2.0 fat     1749 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_preserve_binary_data_in_xrecords.py
--rw-rw-rw-  2.0 fat     6944 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_r12export.py
--rw-rw-rw-  2.0 fat     6256 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_r12strict.py
--rw-rw-rw-  2.0 fat     3410 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_r12writer.py
--rw-rw-rw-  2.0 fat      567 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_read_file_without_handles.py
--rw-rw-rw-  2.0 fat     1121 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_read_write_modern_entites.py
--rw-rw-rw-  2.0 fat     5375 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_recover.py
--rw-rw-rw-  2.0 fat     1959 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_redraw_order.py
--rw-rw-rw-  2.0 fat     1819 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_rotated_block_attributes.py
--rw-rw-rw-  2.0 fat      774 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_surface_entities.py
--rw-rw-rw-  2.0 fat      928 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_write_fixed_meta_data.py
--rw-rw-rw-  2.0 fat     1806 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_write_without_handles.py
--rw-rw-rw-  2.0 fat     3638 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_xref_detach.py
--rw-rw-rw-  2.0 fat     3060 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/AC1003_LINE_Example.dxf
--rw-rw-rw-  2.0 fat   179505 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/acad_table_with_blk_ref.dxf
--rw-rw-rw-  2.0 fat     7956 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/ASCII_R12.dxf
--rw-rw-rw-  2.0 fat     3761 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r12.dxf
--rw-rw-rw-  2.0 fat    20914 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r13.dxf
--rw-rw-rw-  2.0 fat    21137 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r14.dxf
--rw-rw-rw-  2.0 fat    11564 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r2000.dxf
--rw-rw-rw-  2.0 fat     6424 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/cc_dxflib.dxf
--rw-rw-rw-  2.0 fat   173753 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/custom_blocks.dxf
--rw-rw-rw-  2.0 fat    32203 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/duplicate_handles.dxf
--rw-rw-rw-  2.0 fat    18554 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/dxf_unicode.dxf
--rw-rw-rw-  2.0 fat     1592 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/empty_handles.dxf
--rw-rw-rw-  2.0 fat    97103 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/groups.dxf
--rw-rw-rw-  2.0 fat     9146 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/Leica_Disto_S910.dxf
--rw-rw-rw-  2.0 fat    17986 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/MODEL.dxf
--rw-rw-rw-  2.0 fat    25799 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2007.dxf
--rw-rw-rw-  2.0 fat    23927 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2018.dxf
--rw-rw-rw-  2.0 fat    98230 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/mtext_framed_columns.dxf
--rw-rw-rw-  2.0 fat   106574 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/mtext_text_frame.dxf
--rw-rw-rw-  2.0 fat    12001 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/no_layouts.dxf
--rw-rw-rw-  2.0 fat    16295 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/PLOTFILE.plt
--rw-rw-rw-  2.0 fat    28788 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/POLI-ALL210_12.DXF
--rw-rw-rw-  2.0 fat      144 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/R12_with_trash_beyond_EOF.dxf
--rw-rw-rw-  2.0 fat   212407 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/recover01.dxf
--rw-rw-rw-  2.0 fat   115423 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/recover02.dxf
--rw-rw-rw-  2.0 fat    21178 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/small_r13.dxf
--rw-rw-rw-  2.0 fat    10326 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/small_r14.dxf
--rw-rw-rw-  2.0 fat    11286 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/XRECORD_0.bin
--rw-rw-rw-  2.0 fat    11662 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/XRECORD_1.bin
--rw-rw-rw-  2.0 fat    15337 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/XRECORD_2.bin
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/
--rw-rw-rw-  2.0 fat     4710 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/appsettings.py
--rw-rw-rw-  2.0 fat    19818 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/audit.py
--rw-rw-rw-  2.0 fat     5324 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/bbox.py
--rw-rw-rw-  2.0 fat     7888 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/blkrefs.py
--rw-rw-rw-  2.0 fat    14858 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/colors.py
--rw-rw-rw-  2.0 fat    31103 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/commands.py
--rw-rw-rw-  2.0 fat     1549 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/comments.py
--rw-rw-rw-  2.0 fat    22100 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/disassemble.py
--rw-rw-rw-  2.0 fat    52708 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/document.py
--rw-rw-rw-  2.0 fat      832 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/dwginfo.py
--rw-rw-rw-  2.0 fat    16248 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entitydb.py
--rw-rw-rw-  2.0 fat     7495 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/enums.py
--rw-rw-rw-  2.0 fat    13948 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/explode.py
--rw-rw-rw-  2.0 fat     1653 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/eztypes.py
--rw-rw-rw-  2.0 fat    10333 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/filemanagement.py
--rw-rw-rw-  2.0 fat    12157 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/gfxattribs.py
--rw-rw-rw-  2.0 fat   107500 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/graphicsfactory.py
--rw-rw-rw-  2.0 fat     3416 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/groupby.py
--rw-rw-rw-  2.0 fat    16588 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/npshapes.py
--rw-rw-rw-  2.0 fat     2743 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/protocols.py
--rw-rw-rw-  2.0 fat    33129 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/proxygraphic.py
--rw-rw-rw-  2.0 fat       95 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/py.typed
--rw-rw-rw-  2.0 fat    22499 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/query.py
--rw-rw-rw-  2.0 fat     2780 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/queryparser.py
--rw-rw-rw-  2.0 fat     9580 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/r12strict.py
--rw-rw-rw-  2.0 fat    30769 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/recover.py
--rw-rw-rw-  2.0 fat     3515 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/reorder.py
--rw-rw-rw-  2.0 fat    10364 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/transform.py
--rw-rw-rw-  2.0 fat     5750 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/units.py
--rw-rw-rw-  2.0 fat     8280 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/upright.py
--rw-rw-rw-  2.0 fat     9875 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/urecord.py
--rw-rw-rw-  2.0 fat     1024 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/version.py
--rw-rw-rw-  2.0 fat    63359 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/xref.py
--rw-rw-rw-  2.0 fat     2853 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/zoom.py
--rw-rw-rw-  2.0 fat    10898 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/_options.py
--rw-rw-rw-  2.0 fat     2566 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/__init__.py
--rw-rw-rw-  2.0 fat     3259 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/__main__.py
--rw-rw-rw-  2.0 fat     6072 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/bezier3p.pyx
--rw-rw-rw-  2.0 fat     9983 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/bezier4p.pyx
--rw-rw-rw-  2.0 fat    12964 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/bspline.pyx
--rw-rw-rw-  2.0 fat       90 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/construct.pxd
--rw-rw-rw-  2.0 fat     6584 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/construct.pyx
--rw-rw-rw-  2.0 fat     3113 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/linetypes.pyx
--rw-rw-rw-  2.0 fat    23989 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/mapbox_earcut.pyx
--rw-rw-rw-  2.0 fat      386 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/matrix44.pxd
--rw-rw-rw-  2.0 fat    23742 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/matrix44.pyx
--rw-rw-rw-  2.0 fat     1688 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/np_support.pyx
--rw-rw-rw-  2.0 fat     2014 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/vector.pxd
--rw-rw-rw-  2.0 fat    23701 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/vector.pyx
--rw-rw-rw-  2.0 fat     1784 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.cpp
--rw-rw-rw-  2.0 fat      599 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.hpp
--rw-rw-rw-  2.0 fat      424 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.pxd
--rw-rw-rw-  2.0 fat      960 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.cpp
--rw-rw-rw-  2.0 fat      464 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.hpp
--rw-rw-rw-  2.0 fat      407 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.pxd
--rw-rw-rw-  2.0 fat     2135 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.hpp
--rw-rw-rw-  2.0 fat      572 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.pxd
--rw-rw-rw-  2.0 fat     1265 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/__init__.py
--rw-rw-rw-  2.0 fat     6393 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/abstract.py
--rw-rw-rw-  2.0 fat      884 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/api.py
--rw-rw-rw-  2.0 fat     5484 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/const.py
--rw-rw-rw-  2.0 fat     6726 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/dbg.py
--rw-rw-rw-  2.0 fat     2980 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/dxf.py
--rw-rw-rw-  2.0 fat    28991 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/entities.py
--rw-rw-rw-  2.0 fat     4088 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/hdr.py
--rw-rw-rw-  2.0 fat    12823 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/mesh.py
--rw-rw-rw-  2.0 fat    18690 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/sab.py
--rw-rw-rw-  2.0 fat    13184 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/sat.py
--rw-rw-rw-  2.0 fat      115 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/
--rw-rw-rw-  2.0 fat    26415 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/acadctb.py
--rw-rw-rw-  2.0 fat    22229 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/binpacking.py
--rw-rw-rw-  2.0 fat    27692 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dimlines.py
--rw-rw-rw-  2.0 fat    31371 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dxf2code.py
--rw-rw-rw-  2.0 fat    22037 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/genetic_algorithm.py
--rw-rw-rw-  2.0 fat    39755 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/geo.py
--rw-rw-rw-  2.0 fat     2674 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/gerber_D6673.py
--rw-rw-rw-  2.0 fat    25472 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/importer.py
--rw-rw-rw-  2.0 fat    17355 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/iterdxf.py
--rw-rw-rw-  2.0 fat     8940 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/menger_sponge.py
--rw-rw-rw-  2.0 fat    24787 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/meshex.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/mixins.py
--rw-rw-rw-  2.0 fat     6203 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/mtextsurrogate.py
--rw-rw-rw-  2.0 fat    13528 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/mtxpl.py
--rw-rw-rw-  2.0 fat    16400 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/odafc.py
--rw-rw-rw-  2.0 fat     9456 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/openscad.py
--rw-rw-rw-  2.0 fat    15878 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/pycsg.py
--rw-rw-rw-  2.0 fat    22496 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/r12export.py
--rw-rw-rw-  2.0 fat    27198 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/r12writer.py
--rw-rw-rw-  2.0 fat     7615 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/sierpinski_pyramid.py
--rw-rw-rw-  2.0 fat    33167 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/tablepainter.py
--rw-rw-rw-  2.0 fat    12786 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/text2path.py
--rw-rw-rw-  2.0 fat     3351 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/xplayer.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/xqt.py
--rw-rw-rw-  2.0 fat      453 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/__init__.py
--rw-rw-rw-  2.0 fat    10023 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/browser.py
--rw-rw-rw-  2.0 fat     1907 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/data.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/__init__.py
--rw-rw-rw-  2.0 fat      820 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/bookmarks.py
--rw-rw-rw-  2.0 fat    29367 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/browser.py
--rw-rw-rw-  2.0 fat    14891 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/data.py
--rw-rw-rw-  2.0 fat    10993 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/find_dialog.py
--rw-rw-rw-  2.0 fat     1281 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/loader.py
--rw-rw-rw-  2.0 fat    21111 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/model.py
--rw-rw-rw-  2.0 fat     2214 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/tags.py
--rw-rw-rw-  2.0 fat     1382 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/views.py
--rw-rw-rw-  2.0 fat      133 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/__init__.py
--rw-rw-rw-  2.0 fat     7419 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/backend.py
--rw-rw-rw-  2.0 fat     4562 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/clipper.py
--rw-rw-rw-  2.0 fat     9824 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/config.py
--rw-rw-rw-  2.0 fat     1570 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_backend.py
--rw-rw-rw-  2.0 fat      514 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_utils.py
--rw-rw-rw-  2.0 fat    18549 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/designer.py
--rw-rw-rw-  2.0 fat     7222 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/dxf.py
--rw-rw-rw-  2.0 fat    34083 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/frontend.py
--rw-rw-rw-  2.0 fat     1823 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/gfxproxy.py
--rw-rw-rw-  2.0 fat    19568 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/hpgl2.py
--rw-rw-rw-  2.0 fat    14662 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/layout.py
--rw-rw-rw-  2.0 fat    11532 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/matplotlib.py
--rw-rw-rw-  2.0 fat     9878 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/mtext_complex.py
--rw-rw-rw-  2.0 fat    38974 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/properties.py
--rw-rw-rw-  2.0 fat    14436 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pymupdf.py
--rw-rw-rw-  2.0 fat    10569 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pyqt.py
--rw-rw-rw-  2.0 fat    22624 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/qtviewer.py
--rw-rw-rw-  2.0 fat    14399 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/recorder.py
--rw-rw-rw-  2.0 fat    14803 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/svg.py
--rw-rw-rw-  2.0 fat    13023 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text.py
--rw-rw-rw-  2.0 fat     1194 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text_renderer.py
--rw-rw-rw-  2.0 fat      314 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/type_hints.py
--rw-rw-rw-  2.0 fat     2559 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/unified_text_renderer.py
--rw-rw-rw-  2.0 fat      171 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/__init__.py
--rw-rw-rw-  2.0 fat     3112 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/classes_section.py
--rw-rw-rw-  2.0 fat      763 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/const.py
--rw-rw-rw-  2.0 fat     6091 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/crc.py
--rw-rw-rw-  2.0 fat     3160 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/fileheader.py
--rw-rw-rw-  2.0 fat    14851 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/header_section.py
--rw-rw-rw-  2.0 fat     2976 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/loader.py
--rw-rw-rw-  2.0 fat      141 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/__init__.py
--rw-rw-rw-  2.0 fat    13459 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/api.py
--rw-rw-rw-  2.0 fat     8570 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/backend.py
--rw-rw-rw-  2.0 fat      561 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/deps.py
--rw-rw-rw-  2.0 fat    16079 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/interpreter.py
--rw-rw-rw-  2.0 fat     4836 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/page.py
--rw-rw-rw-  2.0 fat    11766 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/plotter.py
--rw-rw-rw-  2.0 fat     1698 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/polygon_buffer.py
--rw-rw-rw-  2.0 fat     5615 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/properties.py
--rw-rw-rw-  2.0 fat     6222 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/tokenizer.py
--rw-rw-rw-  2.0 fat    19451 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/viewer.py
--rw-rw-rw-  2.0 fat      164 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/__init__.py
--rw-rw-rw-  2.0 fat     4757 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/acad_proxy_entity.py
--rw-rw-rw-  2.0 fat    18315 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/acad_table.py
--rw-rw-rw-  2.0 fat    25923 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/acis.py
--rw-rw-rw-  2.0 fat     4890 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/appdata.py
--rw-rw-rw-  2.0 fat     1954 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/appid.py
--rw-rw-rw-  2.0 fat     4942 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/arc.py
--rw-rw-rw-  2.0 fat    26138 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/attrib.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/block.py
--rw-rw-rw-  2.0 fat    10536 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/blockrecord.py
--rw-rw-rw-  2.0 fat    50143 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/boundary_paths.py
--rw-rw-rw-  2.0 fat     7961 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/circle.py
--rw-rw-rw-  2.0 fat    23664 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dictionary.py
--rw-rw-rw-  2.0 fat    48743 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dimension.py
--rw-rw-rw-  2.0 fat    35012 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dimstyle.py
--rw-rw-rw-  2.0 fat    23829 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dimstyleoverride.py
--rw-rw-rw-  2.0 fat     4399 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfclass.py
--rw-rw-rw-  2.0 fat    42404 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfentity.py
--rw-rw-rw-  2.0 fat    26923 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfgfx.py
--rw-rw-rw-  2.0 fat    15279 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfgroups.py
--rw-rw-rw-  2.0 fat    23699 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfns.py
--rw-rw-rw-  2.0 fat    13746 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfobj.py
--rw-rw-rw-  2.0 fat    11186 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/ellipse.py
--rw-rw-rw-  2.0 fat     4170 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/factory.py
--rw-rw-rw-  2.0 fat    23785 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/geodata.py
--rw-rw-rw-  2.0 fat     4026 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/gradient.py
--rw-rw-rw-  2.0 fat    12263 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/hatch.py
--rw-rw-rw-  2.0 fat     3944 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/helix.py
--rw-rw-rw-  2.0 fat     4747 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/idbuffer.py
--rw-rw-rw-  2.0 fat    26057 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/image.py
--rw-rw-rw-  2.0 fat    27932 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/insert.py
--rw-rw-rw-  2.0 fat    27834 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/layer.py
--rw-rw-rw-  2.0 fat    14252 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/layout.py
--rw-rw-rw-  2.0 fat    12978 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/leader.py
--rw-rw-rw-  2.0 fat     4718 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/light.py
--rw-rw-rw-  2.0 fat     3718 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/line.py
--rw-rw-rw-  2.0 fat     9677 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/ltype.py
--rw-rw-rw-  2.0 fat    18878 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/lwpolyline.py
--rw-rw-rw-  2.0 fat    19653 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/material.py
--rw-rw-rw-  2.0 fat    18435 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mesh.py
--rw-rw-rw-  2.0 fat    57367 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mleader.py
--rw-rw-rw-  2.0 fat    37144 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mline.py
--rw-rw-rw-  2.0 fat     8385 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mpolygon.py
--rw-rw-rw-  2.0 fat    48153 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mtext.py
--rw-rw-rw-  2.0 fat     4351 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mtext_columns.py
--rw-rw-rw-  2.0 fat     6284 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/objectcollection.py
--rw-rw-rw-  2.0 fat     2111 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/oleframe.py
--rw-rw-rw-  2.0 fat     4332 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/pattern.py
--rw-rw-rw-  2.0 fat     5238 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/point.py
--rw-rw-rw-  2.0 fat    16427 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/polygon.py
--rw-rw-rw-  2.0 fat    40087 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/polyline.py
--rw-rw-rw-  2.0 fat     4822 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/shape.py
--rw-rw-rw-  2.0 fat    10443 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/solid.py
--rw-rw-rw-  2.0 fat    24085 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/spline.py
--rw-rw-rw-  2.0 fat     8246 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/subentity.py
--rw-rw-rw-  2.0 fat     5196 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/sun.py
--rw-rw-rw-  2.0 fat     2449 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/table.py
--rw-rw-rw-  2.0 fat    17602 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/text.py
--rw-rw-rw-  2.0 fat     9035 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/textstyle.py
--rw-rw-rw-  2.0 fat     3597 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/tolerance.py
--rw-rw-rw-  2.0 fat     2703 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/ucs.py
--rw-rw-rw-  2.0 fat    14366 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/underlay.py
--rw-rw-rw-  2.0 fat     6040 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/view.py
--rw-rw-rw-  2.0 fat    28300 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/viewport.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/visualstyle.py
--rw-rw-rw-  2.0 fat     9970 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/vport.py
--rw-rw-rw-  2.0 fat    17024 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/xdata.py
--rw-rw-rw-  2.0 fat     8495 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/xdict.py
--rw-rw-rw-  2.0 fat     3062 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/xline.py
--rw-rw-rw-  2.0 fat     3127 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/__init__.py
--rw-rw-rw-  2.0 fat    25322 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/fonts.py
--rw-rw-rw-  2.0 fat     2242 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/font_face.py
--rw-rw-rw-  2.0 fat    17287 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/font_manager.py
--rw-rw-rw-  2.0 fat     1702 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/font_measurements.py
--rw-rw-rw-  2.0 fat     1175 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/glyphs.py
--rw-rw-rw-  2.0 fat    10763 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/lff.py
--rw-rw-rw-  2.0 fat    35446 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/shapefile.py
--rw-rw-rw-  2.0 fat     7244 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/ttfonts.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/__init__.py
--rw-rw-rw-  2.0 fat    16696 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/base.py
--rw-rw-rw-  2.0 fat     4343 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/blocklayout.py
--rw-rw-rw-  2.0 fat    29785 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/layout.py
--rw-rw-rw-  2.0 fat    15314 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/layouts.py
--rw-rw-rw-  2.0 fat      232 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/__init__.py
--rw-rw-rw-  2.0 fat     8327 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/attributes.py
--rw-rw-rw-  2.0 fat    16500 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/const.py
--rw-rw-rw-  2.0 fat     1614 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/encoding.py
--rw-rw-rw-  2.0 fat    17013 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/extendedtags.py
--rw-rw-rw-  2.0 fat     5363 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/fileindex.py
--rw-rw-rw-  2.0 fat      727 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/hdrvars.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/loader.py
--rw-rw-rw-  2.0 fat     7447 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/packedtags.py
--rw-rw-rw-  2.0 fat     6355 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/repair.py
--rw-rw-rw-  2.0 fat    13058 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/tagger.py
--rw-rw-rw-  2.0 fat    14336 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/tags.py
--rw-rw-rw-  2.0 fat     8952 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/tagwriter.py
--rw-rw-rw-  2.0 fat    12064 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/types.py
--rw-rw-rw-  2.0 fat    17069 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/validator.py
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/__init__.py
--rw-rw-rw-  2.0 fat    19193 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/arc.py
--rw-rw-rw-  2.0 fat    16270 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/bbox.py
--rw-rw-rw-  2.0 fat     9318 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/bezier.py
--rw-rw-rw-  2.0 fat     2452 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/bezier_interpolation.py
--rw-rw-rw-  2.0 fat     8730 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/box.py
--rw-rw-rw-  2.0 fat    52916 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/bspline.py
--rw-rw-rw-  2.0 fat     5608 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/bulge.py
--rw-rw-rw-  2.0 fat     9002 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/circle.py
--rw-rw-rw-  2.0 fat    24220 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/clipping.py
--rw-rw-rw-  2.0 fat     4319 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/clustering.py
--rw-rw-rw-  2.0 fat    12236 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/construct2d.py
--rw-rw-rw-  2.0 fat    26265 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/construct3d.py
--rw-rw-rw-  2.0 fat     1283 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/cspline.py
--rw-rw-rw-  2.0 fat     9114 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/curvetools.py
--rw-rw-rw-  2.0 fat    22048 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/ellipse.py
--rw-rw-rw-  2.0 fat     4406 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/eulerspiral.py
--rw-rw-rw-  2.0 fat    38883 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/linalg.py
--rw-rw-rw-  2.0 fat    10231 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/line.py
--rw-rw-rw-  2.0 fat     3053 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/offset2d.py
--rw-rw-rw-  2.0 fat     8256 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/parametrize.py
--rw-rw-rw-  2.0 fat    15602 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/perlin.py
--rw-rw-rw-  2.0 fat    15921 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/polyline.py
--rw-rw-rw-  2.0 fat    11867 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/rtree.py
--rw-rw-rw-  2.0 fat     3910 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/shape.py
--rw-rw-rw-  2.0 fat     2568 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/surfaces.py
--rw-rw-rw-  2.0 fat    12155 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/transformtools.py
--rw-rw-rw-  2.0 fat     3631 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/triangulation.py
--rw-rw-rw-  2.0 fat    16976 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/ucs.py
--rw-rw-rw-  2.0 fat     7213 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_bezier3p.py
--rw-rw-rw-  2.0 fat    12967 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_bezier4p.py
--rw-rw-rw-  2.0 fat     9440 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_bspline.py
--rw-rw-rw-  2.0 fat     7272 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_construct.py
--rw-rw-rw-  2.0 fat     2261 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_ctypes.py
--rw-rw-rw-  2.0 fat    24954 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    27606 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_matrix44.py
--rw-rw-rw-  2.0 fat    25912 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_vector.py
--rw-rw-rw-  2.0 fat     2003 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/__init__.py
--rw-rw-rw-  2.0 fat     1306 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/commands.py
--rw-rw-rw-  2.0 fat    31244 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/converter.py
--rw-rw-rw-  2.0 fat     5868 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/nesting.py
--rw-rw-rw-  2.0 fat    18249 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/path.py
--rw-rw-rw-  2.0 fat    10140 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/shapes.py
--rw-rw-rw-  2.0 fat    34217 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/tools.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/__init__.py
--rw-rw-rw-  2.0 fat     2987 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.css
--rw-rw-rw-  2.0 fat     1148 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.html
--rw-rw-rw-  2.0 fat    11304 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.js
--rw-rw-rw-  2.0 fat    17144 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.py
--rw-rw-rw-  2.0 fat     3770 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/pprint.py
--rw-rw-rw-  2.0 fat      812 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.css
--rw-rw-rw-  2.0 fat      316 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.html
--rw-rw-rw-  2.0 fat     2545 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.py
--rw-rw-rw-  2.0 fat     6896 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/reflinks.py
--rw-rw-rw-  2.0 fat      123 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/__init__.py
--rw-rw-rw-  2.0 fat    10039 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/abstract_mtext_renderer.py
--rw-rw-rw-  2.0 fat    20495 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/arrows.py
--rw-rw-rw-  2.0 fat    17749 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/curves.py
--rw-rw-rw-  2.0 fat     4041 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dimension.py
--rw-rw-rw-  2.0 fat    52044 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_base.py
--rw-rw-rw-  2.0 fat    35702 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_curved.py
--rw-rw-rw-  2.0 fat     6894 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_diameter.py
--rw-rw-rw-  2.0 fat    24751 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_linear.py
--rw-rw-rw-  2.0 fat     8084 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_ordinate.py
--rw-rw-rw-  2.0 fat    20295 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_radius.py
--rw-rw-rw-  2.0 fat    47170 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/forms.py
--rw-rw-rw-  2.0 fat    24198 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/hatching.py
--rw-rw-rw-  2.0 fat     4728 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/leader.py
--rw-rw-rw-  2.0 fat      664 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/linetypes.py
--rw-rw-rw-  2.0 fat    64121 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/mesh.py
--rw-rw-rw-  2.0 fat    60923 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/mleader.py
--rw-rw-rw-  2.0 fat     8437 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/mline.py
--rw-rw-rw-  2.0 fat     2964 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/point.py
--rw-rw-rw-  2.0 fat     8736 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/polyline.py
--rw-rw-rw-  2.0 fat     7886 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/r12spline.py
--rw-rw-rw-  2.0 fat    22541 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/trace.py
--rw-rw-rw-  2.0 fat     2881 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/_linetypes.py
--rw-rw-rw-  2.0 fat      778 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/__init__.py
--rw-rw-rw-  2.0 fat     1050 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/16x16.png
--rw-rw-rw-  2.0 fat     1420 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/24x24.png
--rw-rw-rw-  2.0 fat    10638 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/256x256.png
--rw-rw-rw-  2.0 fat     1758 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/32x32.png
--rw-rw-rw-  2.0 fat     2335 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/48x48.png
--rw-rw-rw-  2.0 fat     3050 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/64x64.png
--rw-rw-rw-  2.0 fat     2090 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-copy-64px.png
--rw-rw-rw-  2.0 fat     3109 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-find-64px.png
--rw-rw-rw-  2.0 fat     2388 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-bookmark-64px.png
--rw-rw-rw-  2.0 fat     2519 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-handle-64px.png
--rw-rw-rw-  2.0 fat     2409 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-line-64px.png
--rw-rw-rw-  2.0 fat     2231 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-left-arrow-64px.png
--rw-rw-rw-  2.0 fat     2322 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-next-entity-64px.png
--rw-rw-rw-  2.0 fat     2320 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-prev-entity-64px.png
--rw-rw-rw-  2.0 fat     2244 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-right-arrow-64px.png
--rw-rw-rw-  2.0 fat     2553 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-show-in-tree-64px.png
--rw-rw-rw-  2.0 fat     2373 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-store-bookmark-64px.png
--rw-rw-rw-  2.0 fat    10650 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/acdsdata.py
--rw-rw-rw-  2.0 fat    16508 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/blocks.py
--rw-rw-rw-  2.0 fat    11639 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/classes.py
--rw-rw-rw-  2.0 fat     4137 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/entities.py
--rw-rw-rw-  2.0 fat    11953 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/header.py
--rw-rw-rw-  2.0 fat    60696 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/headervars.py
--rw-rw-rw-  2.0 fat    27009 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/objects.py
--rw-rw-rw-  2.0 fat    26581 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/table.py
--rw-rw-rw-  2.0 fat     5270 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/tables.py
--rw-rw-rw-  2.0 fat       67 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/__init__.py
--rw-rw-rw-  2.0 fat    19711 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/analyze.py
--rw-rw-rw-  2.0 fat    20434 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/binarydata.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/codepage.py
--rw-rw-rw-  2.0 fat     7645 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/complex_ltype.py
--rw-rw-rw-  2.0 fat     1782 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/crypt.py
--rw-rw-rw-  2.0 fat     1511 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/debug.py
--rw-rw-rw-  2.0 fat     2341 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/difftags.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/handle.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/indexing.py
--rw-rw-rw-  2.0 fat     2145 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/juliandate.py
--rw-rw-rw-  2.0 fat     6166 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/pattern.py
--rw-rw-rw-  2.0 fat     1256 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/rawloader.py
--rw-rw-rw-  2.0 fat   129174 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/standards.py
--rw-rw-rw-  2.0 fat     6049 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/strip.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/test.py
--rw-rw-rw-  2.0 fat    65523 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/text.py
--rw-rw-rw-  2.0 fat    54234 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/text_layout.py
--rw-rw-rw-  2.0 fat     6893 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/text_size.py
--rw-rw-rw-  2.0 fat     3077 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/zipmanager.py
--rw-rw-rw-  2.0 fat   142734 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/_iso_pattern.py
--rw-rw-rw-  2.0 fat     3564 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       47 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat    69878 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      302 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    31923 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/
--rw-rw-rw-  2.0 fat      410 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/conftest.py
--rw-rw-rw-  2.0 fat     2336 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
--rw-rw-rw-  2.0 fat     2599 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
--rw-rw-rw-  2.0 fat     1124 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
--rw-rw-rw-  2.0 fat     5456 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
--rw-rw-rw-  2.0 fat      582 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_011_codepage.py
--rw-rw-rw-  2.0 fat    11593 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_012_crypt.py
--rw-rw-rw-  2.0 fat     1191 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
--rw-rw-rw-  2.0 fat     1033 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
--rw-rw-rw-  2.0 fat     4792 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
--rw-rw-rw-  2.0 fat      989 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_016_encoding.py
--rw-rw-rw-  2.0 fat     1383 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_018_handle.py
--rw-rw-rw-  2.0 fat     5518 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
--rw-rw-rw-  2.0 fat     8168 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
--rw-rw-rw-  2.0 fat     3787 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
--rw-rw-rw-  2.0 fat      401 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
--rw-rw-rw-  2.0 fat      539 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
--rw-rw-rw-  2.0 fat     2092 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_040_tags.py
--rw-rw-rw-  2.0 fat     3073 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
--rw-rw-rw-  2.0 fat     6419 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
--rw-rw-rw-  2.0 fat     1632 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
--rw-rw-rw-  2.0 fat    11265 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
--rw-rw-rw-  2.0 fat     3363 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
--rw-rw-rw-  2.0 fat     1974 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
--rw-rw-rw-  2.0 fat     2321 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
--rw-rw-rw-  2.0 fat      568 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
--rw-rw-rw-  2.0 fat     8682 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
--rw-rw-rw-  2.0 fat     1051 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
--rw-rw-rw-  2.0 fat     1500 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
--rw-rw-rw-  2.0 fat    11689 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_101_dxfnamespace.py
--rw-rw-rw-  2.0 fat     2893 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_102_appdata.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_103_reactors.py
--rw-rw-rw-  2.0 fat     4001 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_104_extension_dict.py
--rw-rw-rw-  2.0 fat    20860 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_105_xdata.py
--rw-rw-rw-  2.0 fat    14169 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_110_dxfentity.py
--rw-rw-rw-  2.0 fat     2433 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
--rw-rw-rw-  2.0 fat     6781 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112a_dxfgfx.py
--rw-rw-rw-  2.0 fat      695 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112b_dxfobj.py
--rw-rw-rw-  2.0 fat     2431 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_113_dxfclass.py
--rw-rw-rw-  2.0 fat     4044 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_114_factory.py
--rw-rw-rw-  2.0 fat     2256 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
--rw-rw-rw-  2.0 fat    15794 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_116_dictionary.py
--rw-rw-rw-  2.0 fat     4999 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_117_layer_table_entry.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_118_appid_table_entry.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
--rw-rw-rw-  2.0 fat     3003 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_120_style_table_entry.py
--rw-rw-rw-  2.0 fat     2943 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
--rw-rw-rw-  2.0 fat      379 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_122_vport_table_entry.py
--rw-rw-rw-  2.0 fat     1113 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_123_view_table_entry.py
--rw-rw-rw-  2.0 fat     8757 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
--rw-rw-rw-  2.0 fat     1698 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_125_image_def.py
--rw-rw-rw-  2.0 fat     1312 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_126_image_def_reactor.py
--rw-rw-rw-  2.0 fat     1430 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_127_raster_variables.py
--rw-rw-rw-  2.0 fat     1540 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_128_pdf_definition.py
--rw-rw-rw-  2.0 fat     2778 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_129_xrecord.py
--rw-rw-rw-  2.0 fat     2423 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_130_id_buffer.py
--rw-rw-rw-  2.0 fat     2470 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_131_field_list.py
--rw-rw-rw-  2.0 fat     2435 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_132_layer_filter.py
--rw-rw-rw-  2.0 fat     2153 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_133_sun.py
--rw-rw-rw-  2.0 fat      852 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_134_material.py
--rw-rw-rw-  2.0 fat    11497 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_135_geo_data.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_136_vba_project.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_137_sortentstable.py
--rw-rw-rw-  2.0 fat      704 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
--rw-rw-rw-  2.0 fat     7570 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_139_user_record.py
--rw-rw-rw-  2.0 fat      714 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_140_block_record.py
--rw-rw-rw-  2.0 fat     9199 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_141_layer_vp_override.py
--rw-rw-rw-  2.0 fat     2231 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/conftest.py
--rw-rw-rw-  2.0 fat     6532 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_200_line.py
--rw-rw-rw-  2.0 fat     4273 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_201_point.py
--rw-rw-rw-  2.0 fat     6827 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_202_circle.py
--rw-rw-rw-  2.0 fat     8949 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_203_arc.py
--rw-rw-rw-  2.0 fat     2852 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_204_shape.py
--rw-rw-rw-  2.0 fat     8242 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_205_solid.py
--rw-rw-rw-  2.0 fat     8476 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_206_text.py
--rw-rw-rw-  2.0 fat     4947 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_207_attdef.py
--rw-rw-rw-  2.0 fat     6312 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_208_attrib.py
--rw-rw-rw-  2.0 fat     2671 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_209_vertex.py
--rw-rw-rw-  2.0 fat     5930 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_1.py
--rw-rw-rw-  2.0 fat    13489 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_2.py
--rw-rw-rw-  2.0 fat     6650 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_explode.py
--rw-rw-rw-  2.0 fat     1780 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
--rw-rw-rw-  2.0 fat     7847 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_211_viewport.py
--rw-rw-rw-  2.0 fat    12629 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_212_insert.py
--rw-rw-rw-  2.0 fat     6024 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_213_minsert.py
--rw-rw-rw-  2.0 fat     3284 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_214_block.py
--rw-rw-rw-  2.0 fat     6882 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_215_dimension.py
--rw-rw-rw-  2.0 fat     4907 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
--rw-rw-rw-  2.0 fat    13186 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
--rw-rw-rw-  2.0 fat     6471 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
--rw-rw-rw-  2.0 fat     5535 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
--rw-rw-rw-  2.0 fat     3056 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
--rw-rw-rw-  2.0 fat     7181 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
--rw-rw-rw-  2.0 fat     2066 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
--rw-rw-rw-  2.0 fat     3615 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
--rw-rw-rw-  2.0 fat     6919 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_221_ellipse.py
--rw-rw-rw-  2.0 fat     2223 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_222_xline.py
--rw-rw-rw-  2.0 fat     1493 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_223_ray.py
--rw-rw-rw-  2.0 fat     2176 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_224_group.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_225_mtext.py
--rw-rw-rw-  2.0 fat    12020 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline.py
--rw-rw-rw-  2.0 fat     5529 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
--rw-rw-rw-  2.0 fat    10893 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
--rw-rw-rw-  2.0 fat    15116 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_228_mesh.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
--rw-rw-rw-  2.0 fat    21421 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
--rw-rw-rw-  2.0 fat     6587 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
--rw-rw-rw-  2.0 fat     3140 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
--rw-rw-rw-  2.0 fat    12486 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
--rw-rw-rw-  2.0 fat     2274 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay.py
--rw-rw-rw-  2.0 fat     5243 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay_2.py
--rw-rw-rw-  2.0 fat     2294 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis.py
--rw-rw-rw-  2.0 fat     6799 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis_2.py
--rw-rw-rw-  2.0 fat     1854 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_surface.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_233_helix.py
--rw-rw-rw-  2.0 fat     2040 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_234_light.py
--rw-rw-rw-  2.0 fat     3806 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_235_leader.py
--rw-rw-rw-  2.0 fat    20392 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_236_multileader.py
--rw-rw-rw-  2.0 fat    10992 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_237_mline.py
--rw-rw-rw-  2.0 fat     2356 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_238_tolerance.py
--rw-rw-rw-  2.0 fat    27392 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
--rw-rw-rw-  2.0 fat     4347 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_240_arc_dimension.py
--rw-rw-rw-  2.0 fat     1069 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_241_hyperlink.py
--rw-rw-rw-  2.0 fat    11313 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_242_random_transform.py
--rw-rw-rw-  2.0 fat     3725 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_243_replace_entity.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
--rw-rw-rw-  2.0 fat     4456 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_245_wipeout.py
--rw-rw-rw-  2.0 fat     6175 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_246_spline_audit.py
--rw-rw-rw-  2.0 fat     8165 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
--rw-rw-rw-  2.0 fat     6003 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mpolygon.py
--rw-rw-rw-  2.0 fat    13682 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
--rw-rw-rw-  2.0 fat     5713 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_249_boundary_paths.py
--rw-rw-rw-  2.0 fat     8331 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
--rw-rw-rw-  2.0 fat     7331 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_251_upright.py
--rw-rw-rw-  2.0 fat     4795 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
--rw-rw-rw-  2.0 fat     2082 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_253_ole2frame.py
--rw-rw-rw-  2.0 fat      821 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_254_get_font_name.py
--rw-rw-rw-  2.0 fat     5149 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_300_layout.py
--rw-rw-rw-  2.0 fat     4274 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
--rw-rw-rw-  2.0 fat     5582 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_302_block_references.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_303_auto_block_references.py
--rw-rw-rw-  2.0 fat      913 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_304_new_entity_space.py
--rw-rw-rw-  2.0 fat     3279 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
--rw-rw-rw-  2.0 fat     2609 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
--rw-rw-rw-  2.0 fat     2343 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_307_groupby.py
--rw-rw-rw-  2.0 fat    17748 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_308_query.py
--rw-rw-rw-  2.0 fat     6382 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_309_query_parser.py
--rw-rw-rw-  2.0 fat     5031 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
--rw-rw-rw-  2.0 fat     5782 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_312_virtual_layout.py
--rw-rw-rw-  2.0 fat      647 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_313_redraw_order.py
--rw-rw-rw-  2.0 fat     6128 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_401_headersection.py
--rw-rw-rw-  2.0 fat     2750 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_402_classessection.py
--rw-rw-rw-  2.0 fat     5208 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
--rw-rw-rw-  2.0 fat     6795 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404a_tables.py
--rw-rw-rw-  2.0 fat     4981 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
--rw-rw-rw-  2.0 fat     2450 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_405_classes.py
--rw-rw-rw-  2.0 fat     9094 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
--rw-rw-rw-  2.0 fat      848 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
--rw-rw-rw-  2.0 fat     3375 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
--rw-rw-rw-  2.0 fat     1433 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
--rw-rw-rw-  2.0 fat     5736 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_410_table.py
--rw-rw-rw-  2.0 fat     6607 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
--rw-rw-rw-  2.0 fat    18072 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
--rw-rw-rw-  2.0 fat     4638 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
--rw-rw-rw-  2.0 fat    12327 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
--rw-rw-rw-  2.0 fat     6509 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
--rw-rw-rw-  2.0 fat     5656 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_417_bbox.py
--rw-rw-rw-  2.0 fat     5434 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
--rw-rw-rw-  2.0 fat      733 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
--rw-rw-rw-  2.0 fat     1240 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
--rw-rw-rw-  2.0 fat     5007 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
--rw-rw-rw-  2.0 fat      769 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
--rw-rw-rw-  2.0 fat     7289 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_424_audit.py
--rw-rw-rw-  2.0 fat     3737 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
--rw-rw-rw-  2.0 fat     2981 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
--rw-rw-rw-  2.0 fat     2416 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
--rw-rw-rw-  2.0 fat     2533 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
--rw-rw-rw-  2.0 fat   112800 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/conftest.py
--rw-rw-rw-  2.0 fat     5510 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_500_units.py
--rw-rw-rw-  2.0 fat     1052 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_501_truecolor.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_502_raw_color.py
--rw-rw-rw-  2.0 fat     1695 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_503_indexing.py
--rw-rw-rw-  2.0 fat     1442 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_504_suppress_zeros.py
--rw-rw-rw-  2.0 fat      216 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_506_version.py
--rw-rw-rw-  2.0 fat      579 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_507_dxf_pretty_printer.py
--rw-rw-rw-  2.0 fat      657 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_508_read_zip.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_509_comments.py
--rw-rw-rw-  2.0 fat     1185 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_510_byte_stream.py
--rw-rw-rw-  2.0 fat     4239 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_511_bit_stream.py
--rw-rw-rw-  2.0 fat     5595 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_512_pattern.py
--rw-rw-rw-  2.0 fat     2372 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_513_reorder_entities.py
--rw-rw-rw-  2.0 fat    17710 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_514_text.py
--rw-rw-rw-  2.0 fat     9269 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_515a_fonts_truetype.py
--rw-rw-rw-  2.0 fat     4752 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_515b_fonts_shapefiles.py
--rw-rw-rw-  2.0 fat     2469 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_515c_fonts_lff.py
--rw-rw-rw-  2.0 fat     4002 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_516_zoom.py
--rw-rw-rw-  2.0 fat    34209 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_517_text_layout.py
--rw-rw-rw-  2.0 fat      474 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_518_header_guid.py
--rw-rw-rw-  2.0 fat     3716 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_519_mtext_editor.py
--rw-rw-rw-  2.0 fat     3205 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_520_mtext_context.py
--rw-rw-rw-  2.0 fat    24496 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_521_mtext_parser.py
--rw-rw-rw-  2.0 fat     3863 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_522_text_scanner.py
--rw-rw-rw-  2.0 fat     5207 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_523_text_size.py
--rw-rw-rw-  2.0 fat     5063 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_524_block_reference_manager.py
--rw-rw-rw-  2.0 fat      773 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_525_transparency.py
--rw-rw-rw-  2.0 fat     2133 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_526_explode.py
--rw-rw-rw-  2.0 fat    13521 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_527_gfxattribs.py
--rw-rw-rw-  2.0 fat     2748 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_528_difftags.py
--rw-rw-rw-  2.0 fat     6700 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_529_acis_sat.py
--rw-rw-rw-  2.0 fat     2062 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_530_acis_sab.py
--rw-rw-rw-  2.0 fat    12366 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_531_acis_entities.py
--rw-rw-rw-  2.0 fat     7533 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_532_acis_mesh.py
--rw-rw-rw-  2.0 fat    43259 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_533_shapefiles.py
--rw-rw-rw-  2.0 fat     1034 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_534_dwg_info.py
--rw-rw-rw-  2.0 fat    47978 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_535_xref_basic.py
--rw-rw-rw-  2.0 fat    27614 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_536_xref_conflict.py
--rw-rw-rw-  2.0 fat     6887 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_537_transform.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
--rw-rw-rw-  2.0 fat    16358 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_539_npshapes.py
--rw-rw-rw-  2.0 fat     2605 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_540_lff_parser.py
--rw-rw-rw-  2.0 fat     4026 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/conftest.py
--rw-rw-rw-  2.0 fat     7460 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_600_base.py
--rw-rw-rw-  2.0 fat     2098 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_601_bulge.py
--rw-rw-rw-  2.0 fat    14651 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_602_vec3.py
--rw-rw-rw-  2.0 fat     8956 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_603_vec2.py
--rw-rw-rw-  2.0 fat     2801 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_604_banded_matrix.py
--rw-rw-rw-  2.0 fat     9738 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_604_linalg.py
--rw-rw-rw-  2.0 fat    13943 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_605_matrix44.py
--rw-rw-rw-  2.0 fat     5888 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_606_convexhull.py
--rw-rw-rw-  2.0 fat     1010 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_607_perlin_noise.py
--rw-rw-rw-  2.0 fat     3833 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_608_intersection_line_line_2d.py
--rw-rw-rw-  2.0 fat     1676 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_609_point_on_line.py
--rw-rw-rw-  2.0 fat     3171 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_610_ocs.py
--rw-rw-rw-  2.0 fat     7529 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_611_ucs.py
--rw-rw-rw-  2.0 fat     1831 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_612_ucs_pass_trough.py
--rw-rw-rw-  2.0 fat     2586 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_613_point_in_poygon.py
--rw-rw-rw-  2.0 fat    10913 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_614_construct_3d.py
--rw-rw-rw-  2.0 fat      602 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_615_rytz_axis.py
--rw-rw-rw-  2.0 fat     5215 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_616_plane.py
--rw-rw-rw-  2.0 fat      772 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_617_clockwise_orientation.py
--rw-rw-rw-  2.0 fat     6384 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_618_clipping.py
--rw-rw-rw-  2.0 fat    10108 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_619_greiner_hormann.py
--rw-rw-rw-  2.0 fat     2669 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_620_knot.py
--rw-rw-rw-  2.0 fat    18821 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_621_bspline.py
--rw-rw-rw-  2.0 fat     7652 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_622_bsplineu.py
--rw-rw-rw-  2.0 fat    11327 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_623_rbspline.py
--rw-rw-rw-  2.0 fat    10809 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_624_global_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1247 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_626_local_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1967 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_627_bspline_basis.py
--rw-rw-rw-  2.0 fat    10545 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_629_bezier.py
--rw-rw-rw-  2.0 fat    10714 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_630a_bezier4p_base.py
--rw-rw-rw-  2.0 fat    10204 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_630b_bezier4p_functions.py
--rw-rw-rw-  2.0 fat     1683 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_631_euler_spiral.py
--rw-rw-rw-  2.0 fat     4021 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_632_bezier3p.py
--rw-rw-rw-  2.0 fat    19575 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_640_bbox.py
--rw-rw-rw-  2.0 fat     5393 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_641_construction_ray.py
--rw-rw-rw-  2.0 fat     3673 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_642_construction_line.py
--rw-rw-rw-  2.0 fat     9459 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_643_construction_box.py
--rw-rw-rw-  2.0 fat    10941 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_644_construction_circle.py
--rw-rw-rw-  2.0 fat    10988 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_645_construction_arc.py
--rw-rw-rw-  2.0 fat     3422 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_646_offset_vertices_2d.py
--rw-rw-rw-  2.0 fat     7672 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_647_transform_tools.py
--rw-rw-rw-  2.0 fat     8993 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_648_construction_ellipse.py
--rw-rw-rw-  2.0 fat     4243 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_650_elliptic_arc_span.py
--rw-rw-rw-  2.0 fat     9024 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_651_construction_polyline.py
--rw-rw-rw-  2.0 fat     3168 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_652_approx_param_t.py
--rw-rw-rw-  2.0 fat     5806 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_653_polyline_intersection.py
--rw-rw-rw-  2.0 fat     5193 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_654_rtree.py
--rw-rw-rw-  2.0 fat      788 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_655_dbscan.py
--rw-rw-rw-  2.0 fat      834 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_656_k_means.py
--rw-rw-rw-  2.0 fat     4654 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_657_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    11654 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_658_bevel_tools.py
--rw-rw-rw-  2.0 fat     1875 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_659_intersection_line_polygon_3d.py
--rw-rw-rw-  2.0 fat     1428 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
--rw-rw-rw-  2.0 fat     1741 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
--rw-rw-rw-  2.0 fat     3307 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_662_is_convex_polygon_2d.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_701_arrows.py
--rw-rw-rw-  2.0 fat    17245 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_702_render_forms.py
--rw-rw-rw-  2.0 fat    34220 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_703_mesh_builder.py
--rw-rw-rw-  2.0 fat     4459 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_704_render_linear_dimension.py
--rw-rw-rw-  2.0 fat     1345 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_705_shape.py
--rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_706_random_path.py
--rw-rw-rw-  2.0 fat     5603 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_707_trace.py
--rw-rw-rw-  2.0 fat    33999 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708a_path.py
--rw-rw-rw-  2.0 fat    27351 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708b_path_tools.py
--rw-rw-rw-  2.0 fat     2674 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708c_matplotlib_path_tools.py
--rw-rw-rw-  2.0 fat     3261 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708d_qpainter_path_tools.py
--rw-rw-rw-  2.0 fat     4589 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708e_path_shapes.py
--rw-rw-rw-  2.0 fat     4121 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708f_path_nesting.py
--rw-rw-rw-  2.0 fat     1308 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_709_linetype_renderer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_711_points.py
--rw-rw-rw-  2.0 fat     6594 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_712_render_curved_dimension.py
--rw-rw-rw-  2.0 fat     1472 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_713_mleader_builder.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_714_mleader_render_engine.py
--rw-rw-rw-  2.0 fat    11778 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_715_hatching.py
--rw-rw-rw-  2.0 fat     2626 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
--rw-rw-rw-  2.0 fat     4771 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_800_mtext_surrogate.py
--rw-rw-rw-  2.0 fat     1352 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_801_r12spline.py
--rw-rw-rw-  2.0 fat     7881 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_802_table_painter.py
--rw-rw-rw-  2.0 fat    12386 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_803_entities_to_code.py
--rw-rw-rw-  2.0 fat     6844 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_804_importer.py
--rw-rw-rw-  2.0 fat     2362 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_805_pycsg.py
--rw-rw-rw-  2.0 fat    15467 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_806_acadctb.py
--rw-rw-rw-  2.0 fat     4860 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_807_dwg_loader_basics.py
--rw-rw-rw-  2.0 fat    10862 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_810_drawing_properties.py
--rw-rw-rw-  2.0 fat    11597 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_811a_drawing_frontend.py
--rw-rw-rw-  2.0 fat     8684 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_811b_drawing_recorder.py
--rw-rw-rw-  2.0 fat     2898 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_811c_viewport_processing.py
--rw-rw-rw-  2.0 fat     4157 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_812_drawing_graphic_proxy.py
--rw-rw-rw-  2.0 fat    13751 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_813_geo_interface.py
--rw-rw-rw-  2.0 fat    14853 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_814_text2path.py
--rw-rw-rw-  2.0 fat    16239 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_815_dxf_browser.py
--rw-rw-rw-  2.0 fat    11275 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_816_bin_packing.py
--rw-rw-rw-  2.0 fat    12554 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_817_genetic_algorithm.py
--rw-rw-rw-  2.0 fat     9008 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_818_meshex.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_819_menger_sponge.py
--rw-rw-rw-  2.0 fat     4433 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_820_openscad.py
--rw-rw-rw-  2.0 fat    15655 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2.py
--rw-rw-rw-  2.0 fat     1376 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
--rw-rw-rw-  2.0 fat     1028 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_822_clipper.py
--rw-rw-rw-  2.0 fat     5284 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_823_drawing_layout.py
--rw-rw-rw-  2.0 fat     3312 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_824_svg_drawing_backend.py
--rw-rw-rw-  2.0 fat     2014 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
--rw-rw-rw-  2.0 fat     2527 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_901_acc_vec2.py
--rw-rw-rw-  2.0 fat     2199 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_902_acc_vec3.py
--rw-rw-rw-  2.0 fat     2142 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
--rw-rw-rw-  2.0 fat     3158 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
--rw-rw-rw-  2.0 fat     1452 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
--rw-rw-rw-  2.0 fat     4755 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_906_acc_bspline.py
--rw-rw-rw-  2.0 fat     2656 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_414_bbox_calculation.py
--rw-rw-rw-  2.0 fat     1213 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
--rw-rw-rw-  2.0 fat     2268 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_574_flattening_error.py
--rw-rw-rw-  2.0 fat     1754 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
--rw-rw-rw-  2.0 fat      682 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_749_text_layout.py
--rw-rw-rw-  2.0 fat    11094 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
-841 files, 8737649 bytes uncompressed, 1968717 bytes compressed:  77.5%
+Zip file size: 2123041 bytes, number of entries: 841
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/LICENSE
+-rw-rw-rw-  2.0 fat      302 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/MANIFEST.in
+-rw-rw-rw-  2.0 fat   102539 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/NEWS.md
+-rw-rw-rw-  2.0 fat    71110 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/PKG-INFO
+-rw-rw-rw-  2.0 fat     6846 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/README.md
+-rw-rw-rw-  2.0 fat       55 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/requirements.txt
+-rw-rw-rw-  2.0 fat       74 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/setup.cfg
+-rw-rw-rw-  2.0 fat     5576 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/
+-rw-rw-rw-  2.0 fat      567 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/check_disable_c_ext_by_config_file.py
+-rw-rw-rw-  2.0 fat      541 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/check_disable_c_ext_by_env_var.py
+-rw-rw-rw-  2.0 fat      410 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/conftest.py
+-rw-rw-rw-  2.0 fat     1054 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_acad_table.py
+-rw-rw-rw-  2.0 fat     4686 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_all_dimline_styles.py
+-rw-rw-rw-  2.0 fat     4133 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_all_ellipse_transformations.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_anonymous_blocks.py
+-rw-rw-rw-  2.0 fat      871 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_audit_critical_dxf_files.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_audit_layouts.py
+-rw-rw-rw-  2.0 fat     1726 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_complex_line_type_2.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_create_basic_graphics.py
+-rw-rw-rw-  2.0 fat     1921 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_document_guid.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_document_page_setup.py
+-rw-rw-rw-  2.0 fat      998 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_dxf_info_scanning.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_entities_iterator.py
+-rw-rw-rw-  2.0 fat      934 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_fix_dulicate_handles.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_geo.py
+-rw-rw-rw-  2.0 fat     1250 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_groups.py
+-rw-rw-rw-  2.0 fat      905 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_hpgl2_addon.py
+-rw-rw-rw-  2.0 fat      630 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_ignore_junk_beyond_EOF.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_launcher.py
+-rw-rw-rw-  2.0 fat      631 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_leica_disto_r12.py
+-rw-rw-rw-  2.0 fat      737 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_load_dxf_unicode_notation.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_mtext_columns.py
+-rw-rw-rw-  2.0 fat     2392 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_mtext_explode_addon.py
+-rw-rw-rw-  2.0 fat     1846 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_mtext_text_frame.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_new_table_entries.py
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_none_ascii_read_write.py
+-rw-rw-rw-  2.0 fat     3435 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_odafc.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_open_binary_DXF_files.py
+-rw-rw-rw-  2.0 fat      751 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_open_coord_order_issue.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_open_exotic_dxf_files.py
+-rw-rw-rw-  2.0 fat      879 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_open_R13_R14.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_polyline_entity.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_preserve_binary_data_in_xrecords.py
+-rw-rw-rw-  2.0 fat     6944 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_r12export.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_r12strict.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_r12writer.py
+-rw-rw-rw-  2.0 fat      567 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_read_file_without_handles.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_read_write_modern_entites.py
+-rw-rw-rw-  2.0 fat     5375 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_recover.py
+-rw-rw-rw-  2.0 fat     1959 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_redraw_order.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_rotated_block_attributes.py
+-rw-rw-rw-  2.0 fat      774 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_surface_entities.py
+-rw-rw-rw-  2.0 fat      928 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_write_fixed_meta_data.py
+-rw-rw-rw-  2.0 fat     1806 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_write_without_handles.py
+-rw-rw-rw-  2.0 fat     3638 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/test_xref_detach.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/AC1003_LINE_Example.dxf
+-rw-rw-rw-  2.0 fat   179505 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/acad_table_with_blk_ref.dxf
+-rw-rw-rw-  2.0 fat     7956 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/ASCII_R12.dxf
+-rw-rw-rw-  2.0 fat     3761 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r12.dxf
+-rw-rw-rw-  2.0 fat    20914 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r13.dxf
+-rw-rw-rw-  2.0 fat    21137 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r14.dxf
+-rw-rw-rw-  2.0 fat    11564 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r2000.dxf
+-rw-rw-rw-  2.0 fat     6424 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/cc_dxflib.dxf
+-rw-rw-rw-  2.0 fat   173753 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/custom_blocks.dxf
+-rw-rw-rw-  2.0 fat    32203 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/duplicate_handles.dxf
+-rw-rw-rw-  2.0 fat    18554 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/dxf_unicode.dxf
+-rw-rw-rw-  2.0 fat     1592 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/empty_handles.dxf
+-rw-rw-rw-  2.0 fat    97103 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/groups.dxf
+-rw-rw-rw-  2.0 fat     9146 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/Leica_Disto_S910.dxf
+-rw-rw-rw-  2.0 fat    17986 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/MODEL.dxf
+-rw-rw-rw-  2.0 fat    25799 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/mtext_columns_R2007.dxf
+-rw-rw-rw-  2.0 fat    23927 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/mtext_columns_R2018.dxf
+-rw-rw-rw-  2.0 fat    98230 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/mtext_framed_columns.dxf
+-rw-rw-rw-  2.0 fat   106574 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/mtext_text_frame.dxf
+-rw-rw-rw-  2.0 fat    12001 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/no_layouts.dxf
+-rw-rw-rw-  2.0 fat    16295 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/PLOTFILE.plt
+-rw-rw-rw-  2.0 fat    28788 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/POLI-ALL210_12.DXF
+-rw-rw-rw-  2.0 fat      144 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+-rw-rw-rw-  2.0 fat   212407 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/recover01.dxf
+-rw-rw-rw-  2.0 fat   115423 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/recover02.dxf
+-rw-rw-rw-  2.0 fat    21178 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/small_r13.dxf
+-rw-rw-rw-  2.0 fat    10326 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/small_r14.dxf
+-rw-rw-rw-  2.0 fat    11286 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/XRECORD_0.bin
+-rw-rw-rw-  2.0 fat    11662 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/XRECORD_1.bin
+-rw-rw-rw-  2.0 fat    15337 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/integration_tests/data/XRECORD_2.bin
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/fonts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/path/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/
+-rw-rw-rw-  2.0 fat     4710 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/appsettings.py
+-rw-rw-rw-  2.0 fat    19849 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/audit.py
+-rw-rw-rw-  2.0 fat     5324 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/bbox.py
+-rw-rw-rw-  2.0 fat     7888 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/blkrefs.py
+-rw-rw-rw-  2.0 fat    14858 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/colors.py
+-rw-rw-rw-  2.0 fat    31103 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/commands.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/comments.py
+-rw-rw-rw-  2.0 fat    22100 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/disassemble.py
+-rw-rw-rw-  2.0 fat    52708 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/document.py
+-rw-rw-rw-  2.0 fat      832 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/dwginfo.py
+-rw-rw-rw-  2.0 fat    16248 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entitydb.py
+-rw-rw-rw-  2.0 fat     7495 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/enums.py
+-rw-rw-rw-  2.0 fat    13948 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/explode.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/eztypes.py
+-rw-rw-rw-  2.0 fat    10333 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/filemanagement.py
+-rw-rw-rw-  2.0 fat    12157 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/gfxattribs.py
+-rw-rw-rw-  2.0 fat   107500 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/graphicsfactory.py
+-rw-rw-rw-  2.0 fat     3416 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/groupby.py
+-rw-rw-rw-  2.0 fat    16588 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/npshapes.py
+-rw-rw-rw-  2.0 fat     2743 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/protocols.py
+-rw-rw-rw-  2.0 fat    33805 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/proxygraphic.py
+-rw-rw-rw-  2.0 fat       95 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/py.typed
+-rw-rw-rw-  2.0 fat    22499 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/query.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/queryparser.py
+-rw-rw-rw-  2.0 fat     9580 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/r12strict.py
+-rw-rw-rw-  2.0 fat    30769 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/recover.py
+-rw-rw-rw-  2.0 fat     3515 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/reorder.py
+-rw-rw-rw-  2.0 fat    10364 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/transform.py
+-rw-rw-rw-  2.0 fat     5750 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/units.py
+-rw-rw-rw-  2.0 fat     8280 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/upright.py
+-rw-rw-rw-  2.0 fat     9875 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/urecord.py
+-rw-rw-rw-  2.0 fat     1024 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/version.py
+-rw-rw-rw-  2.0 fat    64359 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/xref.py
+-rw-rw-rw-  2.0 fat     2853 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/zoom.py
+-rw-rw-rw-  2.0 fat    10898 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/_options.py
+-rw-rw-rw-  2.0 fat     2566 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/__init__.py
+-rw-rw-rw-  2.0 fat     3259 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/__main__.py
+-rw-rw-rw-  2.0 fat     6072 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/bezier3p.pyx
+-rw-rw-rw-  2.0 fat     9983 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/bezier4p.pyx
+-rw-rw-rw-  2.0 fat    12964 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/bspline.pyx
+-rw-rw-rw-  2.0 fat       90 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/construct.pxd
+-rw-rw-rw-  2.0 fat     6584 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/construct.pyx
+-rw-rw-rw-  2.0 fat     3113 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/linetypes.pyx
+-rw-rw-rw-  2.0 fat    23989 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/mapbox_earcut.pyx
+-rw-rw-rw-  2.0 fat      386 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/matrix44.pxd
+-rw-rw-rw-  2.0 fat    23742 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/matrix44.pyx
+-rw-rw-rw-  2.0 fat     1688 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/np_support.pyx
+-rw-rw-rw-  2.0 fat     2014 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/vector.pxd
+-rw-rw-rw-  2.0 fat    23701 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/vector.pyx
+-rw-rw-rw-  2.0 fat     1784 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+-rw-rw-rw-  2.0 fat      599 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+-rw-rw-rw-  2.0 fat      424 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+-rw-rw-rw-  2.0 fat      960 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_quad_bezier.cpp
+-rw-rw-rw-  2.0 fat      464 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_quad_bezier.hpp
+-rw-rw-rw-  2.0 fat      407 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_quad_bezier.pxd
+-rw-rw-rw-  2.0 fat     2135 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_vec3.hpp
+-rw-rw-rw-  2.0 fat      572 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_vec3.pxd
+-rw-rw-rw-  2.0 fat     1265 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acc/__init__.py
+-rw-rw-rw-  2.0 fat     6393 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/abstract.py
+-rw-rw-rw-  2.0 fat      884 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/api.py
+-rw-rw-rw-  2.0 fat     5484 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/const.py
+-rw-rw-rw-  2.0 fat     6726 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/dbg.py
+-rw-rw-rw-  2.0 fat     2980 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/dxf.py
+-rw-rw-rw-  2.0 fat    28991 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/entities.py
+-rw-rw-rw-  2.0 fat     4088 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/hdr.py
+-rw-rw-rw-  2.0 fat    12823 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/mesh.py
+-rw-rw-rw-  2.0 fat    18690 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/sab.py
+-rw-rw-rw-  2.0 fat    13184 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/sat.py
+-rw-rw-rw-  2.0 fat      115 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/acis/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/acisbrowser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/browser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/dwg/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/
+-rw-rw-rw-  2.0 fat    26415 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/acadctb.py
+-rw-rw-rw-  2.0 fat    22229 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/binpacking.py
+-rw-rw-rw-  2.0 fat    27692 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/dimlines.py
+-rw-rw-rw-  2.0 fat    31371 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/dxf2code.py
+-rw-rw-rw-  2.0 fat    22037 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/genetic_algorithm.py
+-rw-rw-rw-  2.0 fat    39755 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/geo.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/gerber_D6673.py
+-rw-rw-rw-  2.0 fat    25472 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/importer.py
+-rw-rw-rw-  2.0 fat    17355 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/iterdxf.py
+-rw-rw-rw-  2.0 fat     8940 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/menger_sponge.py
+-rw-rw-rw-  2.0 fat    24787 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/meshex.py
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/mixins.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/mtextsurrogate.py
+-rw-rw-rw-  2.0 fat    13528 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/mtxpl.py
+-rw-rw-rw-  2.0 fat    16400 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/odafc.py
+-rw-rw-rw-  2.0 fat     9456 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/openscad.py
+-rw-rw-rw-  2.0 fat    15878 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/pycsg.py
+-rw-rw-rw-  2.0 fat    22317 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/r12export.py
+-rw-rw-rw-  2.0 fat    27198 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/r12writer.py
+-rw-rw-rw-  2.0 fat     7615 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/sierpinski_pyramid.py
+-rw-rw-rw-  2.0 fat    33167 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/tablepainter.py
+-rw-rw-rw-  2.0 fat    12786 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/text2path.py
+-rw-rw-rw-  2.0 fat     3351 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/xplayer.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/xqt.py
+-rw-rw-rw-  2.0 fat      453 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/__init__.py
+-rw-rw-rw-  2.0 fat    10023 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/acisbrowser/browser.py
+-rw-rw-rw-  2.0 fat     1907 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/acisbrowser/data.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/acisbrowser/__init__.py
+-rw-rw-rw-  2.0 fat      820 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/browser/bookmarks.py
+-rw-rw-rw-  2.0 fat    29367 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/browser/browser.py
+-rw-rw-rw-  2.0 fat    14891 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/browser/data.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/browser/find_dialog.py
+-rw-rw-rw-  2.0 fat     1281 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/browser/loader.py
+-rw-rw-rw-  2.0 fat    21111 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/browser/model.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/browser/tags.py
+-rw-rw-rw-  2.0 fat     1382 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/browser/views.py
+-rw-rw-rw-  2.0 fat      133 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/browser/__init__.py
+-rw-rw-rw-  2.0 fat     7419 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/backend.py
+-rw-rw-rw-  2.0 fat     4562 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/clipper.py
+-rw-rw-rw-  2.0 fat     9824 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/config.py
+-rw-rw-rw-  2.0 fat     1570 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/debug_backend.py
+-rw-rw-rw-  2.0 fat      514 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/debug_utils.py
+-rw-rw-rw-  2.0 fat    18549 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/designer.py
+-rw-rw-rw-  2.0 fat     7222 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/dxf.py
+-rw-rw-rw-  2.0 fat    34083 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/frontend.py
+-rw-rw-rw-  2.0 fat     1823 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/gfxproxy.py
+-rw-rw-rw-  2.0 fat    19568 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/hpgl2.py
+-rw-rw-rw-  2.0 fat    14662 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/layout.py
+-rw-rw-rw-  2.0 fat    11532 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/matplotlib.py
+-rw-rw-rw-  2.0 fat     9878 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/mtext_complex.py
+-rw-rw-rw-  2.0 fat    38974 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/properties.py
+-rw-rw-rw-  2.0 fat    14436 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/pymupdf.py
+-rw-rw-rw-  2.0 fat    10569 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/pyqt.py
+-rw-rw-rw-  2.0 fat    22624 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/qtviewer.py
+-rw-rw-rw-  2.0 fat    14399 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/recorder.py
+-rw-rw-rw-  2.0 fat    14803 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/svg.py
+-rw-rw-rw-  2.0 fat    13023 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/text.py
+-rw-rw-rw-  2.0 fat     1194 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/text_renderer.py
+-rw-rw-rw-  2.0 fat      314 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/type_hints.py
+-rw-rw-rw-  2.0 fat     2559 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/unified_text_renderer.py
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/drawing/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/dwg/classes_section.py
+-rw-rw-rw-  2.0 fat      763 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/dwg/const.py
+-rw-rw-rw-  2.0 fat     6091 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/dwg/crc.py
+-rw-rw-rw-  2.0 fat     3160 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/dwg/fileheader.py
+-rw-rw-rw-  2.0 fat    14851 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/dwg/header_section.py
+-rw-rw-rw-  2.0 fat     2976 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/dwg/loader.py
+-rw-rw-rw-  2.0 fat      141 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/dwg/__init__.py
+-rw-rw-rw-  2.0 fat    13459 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/api.py
+-rw-rw-rw-  2.0 fat     8570 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/backend.py
+-rw-rw-rw-  2.0 fat      561 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/deps.py
+-rw-rw-rw-  2.0 fat    16079 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/interpreter.py
+-rw-rw-rw-  2.0 fat     4836 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/page.py
+-rw-rw-rw-  2.0 fat    11766 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/plotter.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/polygon_buffer.py
+-rw-rw-rw-  2.0 fat     5615 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/properties.py
+-rw-rw-rw-  2.0 fat     6222 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/tokenizer.py
+-rw-rw-rw-  2.0 fat    19451 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/viewer.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/__init__.py
+-rw-rw-rw-  2.0 fat     5920 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat    19466 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/acad_table.py
+-rw-rw-rw-  2.0 fat    25923 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/acis.py
+-rw-rw-rw-  2.0 fat     4890 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/appdata.py
+-rw-rw-rw-  2.0 fat     1954 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/appid.py
+-rw-rw-rw-  2.0 fat     4942 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/arc.py
+-rw-rw-rw-  2.0 fat    26657 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/attrib.py
+-rw-rw-rw-  2.0 fat     8850 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/block.py
+-rw-rw-rw-  2.0 fat    10400 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/blockrecord.py
+-rw-rw-rw-  2.0 fat    50143 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/boundary_paths.py
+-rw-rw-rw-  2.0 fat     7961 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/circle.py
+-rw-rw-rw-  2.0 fat    23664 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/dictionary.py
+-rw-rw-rw-  2.0 fat    48743 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/dimension.py
+-rw-rw-rw-  2.0 fat    35012 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/dimstyle.py
+-rw-rw-rw-  2.0 fat    23829 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/dimstyleoverride.py
+-rw-rw-rw-  2.0 fat     4399 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/dxfclass.py
+-rw-rw-rw-  2.0 fat    42404 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/dxfentity.py
+-rw-rw-rw-  2.0 fat    26923 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/dxfgfx.py
+-rw-rw-rw-  2.0 fat    15279 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/dxfgroups.py
+-rw-rw-rw-  2.0 fat    23699 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/dxfns.py
+-rw-rw-rw-  2.0 fat    13746 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/dxfobj.py
+-rw-rw-rw-  2.0 fat    11186 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/ellipse.py
+-rw-rw-rw-  2.0 fat     4170 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/factory.py
+-rw-rw-rw-  2.0 fat    23785 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/geodata.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/gradient.py
+-rw-rw-rw-  2.0 fat    12263 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/hatch.py
+-rw-rw-rw-  2.0 fat     3944 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/helix.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/idbuffer.py
+-rw-rw-rw-  2.0 fat    26057 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/image.py
+-rw-rw-rw-  2.0 fat    27931 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/insert.py
+-rw-rw-rw-  2.0 fat    27834 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/layer.py
+-rw-rw-rw-  2.0 fat    14252 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/layout.py
+-rw-rw-rw-  2.0 fat    12978 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/leader.py
+-rw-rw-rw-  2.0 fat     4718 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/light.py
+-rw-rw-rw-  2.0 fat     3718 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/line.py
+-rw-rw-rw-  2.0 fat     9677 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/ltype.py
+-rw-rw-rw-  2.0 fat    18878 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/lwpolyline.py
+-rw-rw-rw-  2.0 fat    19653 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/material.py
+-rw-rw-rw-  2.0 fat    18435 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/mesh.py
+-rw-rw-rw-  2.0 fat    57367 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/mleader.py
+-rw-rw-rw-  2.0 fat    37144 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/mline.py
+-rw-rw-rw-  2.0 fat     8385 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/mpolygon.py
+-rw-rw-rw-  2.0 fat    48153 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/mtext.py
+-rw-rw-rw-  2.0 fat     4351 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/mtext_columns.py
+-rw-rw-rw-  2.0 fat     6284 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/objectcollection.py
+-rw-rw-rw-  2.0 fat     2111 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/oleframe.py
+-rw-rw-rw-  2.0 fat     4332 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/pattern.py
+-rw-rw-rw-  2.0 fat     5238 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/point.py
+-rw-rw-rw-  2.0 fat    16427 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/polygon.py
+-rw-rw-rw-  2.0 fat    40087 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/polyline.py
+-rw-rw-rw-  2.0 fat     4822 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/shape.py
+-rw-rw-rw-  2.0 fat    10443 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/solid.py
+-rw-rw-rw-  2.0 fat    24085 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/spline.py
+-rw-rw-rw-  2.0 fat     8246 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/subentity.py
+-rw-rw-rw-  2.0 fat     5196 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/sun.py
+-rw-rw-rw-  2.0 fat     2449 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/table.py
+-rw-rw-rw-  2.0 fat    17602 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/text.py
+-rw-rw-rw-  2.0 fat     9035 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/textstyle.py
+-rw-rw-rw-  2.0 fat     3597 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/tolerance.py
+-rw-rw-rw-  2.0 fat     2703 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/ucs.py
+-rw-rw-rw-  2.0 fat    14366 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/underlay.py
+-rw-rw-rw-  2.0 fat     6040 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/view.py
+-rw-rw-rw-  2.0 fat    28300 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/viewport.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/visualstyle.py
+-rw-rw-rw-  2.0 fat     9970 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/vport.py
+-rw-rw-rw-  2.0 fat    17024 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/xdata.py
+-rw-rw-rw-  2.0 fat     8495 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/xdict.py
+-rw-rw-rw-  2.0 fat     3062 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/xline.py
+-rw-rw-rw-  2.0 fat     3148 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/entities/__init__.py
+-rw-rw-rw-  2.0 fat    25322 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/fonts/fonts.py
+-rw-rw-rw-  2.0 fat     2242 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/fonts/font_face.py
+-rw-rw-rw-  2.0 fat    17287 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/fonts/font_manager.py
+-rw-rw-rw-  2.0 fat     1702 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/fonts/font_measurements.py
+-rw-rw-rw-  2.0 fat     1175 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/fonts/glyphs.py
+-rw-rw-rw-  2.0 fat    10763 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/fonts/lff.py
+-rw-rw-rw-  2.0 fat    35446 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/fonts/shapefile.py
+-rw-rw-rw-  2.0 fat     7244 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/fonts/ttfonts.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/fonts/__init__.py
+-rw-rw-rw-  2.0 fat    16696 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/layouts/base.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/layouts/blocklayout.py
+-rw-rw-rw-  2.0 fat    29785 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/layouts/layout.py
+-rw-rw-rw-  2.0 fat    15314 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/layouts/layouts.py
+-rw-rw-rw-  2.0 fat      232 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/layouts/__init__.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/attributes.py
+-rw-rw-rw-  2.0 fat    16500 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/const.py
+-rw-rw-rw-  2.0 fat     1614 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/encoding.py
+-rw-rw-rw-  2.0 fat    17013 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/extendedtags.py
+-rw-rw-rw-  2.0 fat     5363 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/fileindex.py
+-rw-rw-rw-  2.0 fat      727 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/hdrvars.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/loader.py
+-rw-rw-rw-  2.0 fat     7447 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/packedtags.py
+-rw-rw-rw-  2.0 fat     6355 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/repair.py
+-rw-rw-rw-  2.0 fat    13058 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/tagger.py
+-rw-rw-rw-  2.0 fat    14336 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/tags.py
+-rw-rw-rw-  2.0 fat     8952 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/tagwriter.py
+-rw-rw-rw-  2.0 fat    12064 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/types.py
+-rw-rw-rw-  2.0 fat    17069 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/validator.py
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/lldxf/__init__.py
+-rw-rw-rw-  2.0 fat    19193 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/arc.py
+-rw-rw-rw-  2.0 fat    16270 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/bbox.py
+-rw-rw-rw-  2.0 fat     9318 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/bezier.py
+-rw-rw-rw-  2.0 fat     2452 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/bezier_interpolation.py
+-rw-rw-rw-  2.0 fat     8730 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/box.py
+-rw-rw-rw-  2.0 fat    52916 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/bspline.py
+-rw-rw-rw-  2.0 fat     5608 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/bulge.py
+-rw-rw-rw-  2.0 fat     9002 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/circle.py
+-rw-rw-rw-  2.0 fat    24220 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/clipping.py
+-rw-rw-rw-  2.0 fat     4319 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/clustering.py
+-rw-rw-rw-  2.0 fat    12236 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/construct2d.py
+-rw-rw-rw-  2.0 fat    26265 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/construct3d.py
+-rw-rw-rw-  2.0 fat     1283 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/cspline.py
+-rw-rw-rw-  2.0 fat     9114 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/curvetools.py
+-rw-rw-rw-  2.0 fat    22048 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/ellipse.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/eulerspiral.py
+-rw-rw-rw-  2.0 fat    38883 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/linalg.py
+-rw-rw-rw-  2.0 fat    10231 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/line.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/offset2d.py
+-rw-rw-rw-  2.0 fat     8256 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/parametrize.py
+-rw-rw-rw-  2.0 fat    15602 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/perlin.py
+-rw-rw-rw-  2.0 fat    15921 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/polyline.py
+-rw-rw-rw-  2.0 fat    11867 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/rtree.py
+-rw-rw-rw-  2.0 fat     3910 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/shape.py
+-rw-rw-rw-  2.0 fat     2568 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/surfaces.py
+-rw-rw-rw-  2.0 fat    12155 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/transformtools.py
+-rw-rw-rw-  2.0 fat     3631 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/triangulation.py
+-rw-rw-rw-  2.0 fat    16976 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/ucs.py
+-rw-rw-rw-  2.0 fat     7213 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/_bezier3p.py
+-rw-rw-rw-  2.0 fat    12967 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/_bezier4p.py
+-rw-rw-rw-  2.0 fat     9440 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/_bspline.py
+-rw-rw-rw-  2.0 fat     7272 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/_construct.py
+-rw-rw-rw-  2.0 fat     2261 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/_ctypes.py
+-rw-rw-rw-  2.0 fat    24954 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    27606 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/_matrix44.py
+-rw-rw-rw-  2.0 fat    25912 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/_vector.py
+-rw-rw-rw-  2.0 fat     2003 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/math/__init__.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/path/commands.py
+-rw-rw-rw-  2.0 fat    31244 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/path/converter.py
+-rw-rw-rw-  2.0 fat     5868 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/path/nesting.py
+-rw-rw-rw-  2.0 fat    18249 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/path/path.py
+-rw-rw-rw-  2.0 fat    10140 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/path/shapes.py
+-rw-rw-rw-  2.0 fat    34217 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/path/tools.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/path/__init__.py
+-rw-rw-rw-  2.0 fat     2987 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.css
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.html
+-rw-rw-rw-  2.0 fat    11304 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.js
+-rw-rw-rw-  2.0 fat    17144 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.py
+-rw-rw-rw-  2.0 fat     3770 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/pprint.py
+-rw-rw-rw-  2.0 fat      812 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/rawpp.css
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/rawpp.html
+-rw-rw-rw-  2.0 fat     2545 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/rawpp.py
+-rw-rw-rw-  2.0 fat     6896 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/reflinks.py
+-rw-rw-rw-  2.0 fat      123 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/pp/__init__.py
+-rw-rw-rw-  2.0 fat    10039 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/abstract_mtext_renderer.py
+-rw-rw-rw-  2.0 fat    20495 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/arrows.py
+-rw-rw-rw-  2.0 fat    17749 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/curves.py
+-rw-rw-rw-  2.0 fat     4041 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/dimension.py
+-rw-rw-rw-  2.0 fat    52044 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/dim_base.py
+-rw-rw-rw-  2.0 fat    35702 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/dim_curved.py
+-rw-rw-rw-  2.0 fat     6894 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/dim_diameter.py
+-rw-rw-rw-  2.0 fat    24751 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/dim_linear.py
+-rw-rw-rw-  2.0 fat     8084 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/dim_ordinate.py
+-rw-rw-rw-  2.0 fat    20295 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/dim_radius.py
+-rw-rw-rw-  2.0 fat    47170 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/forms.py
+-rw-rw-rw-  2.0 fat    24198 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/hatching.py
+-rw-rw-rw-  2.0 fat     4728 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/leader.py
+-rw-rw-rw-  2.0 fat      664 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/linetypes.py
+-rw-rw-rw-  2.0 fat    64121 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/mesh.py
+-rw-rw-rw-  2.0 fat    60923 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/mleader.py
+-rw-rw-rw-  2.0 fat     8437 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/mline.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/point.py
+-rw-rw-rw-  2.0 fat     8736 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/polyline.py
+-rw-rw-rw-  2.0 fat     7886 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/r12spline.py
+-rw-rw-rw-  2.0 fat    22541 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/trace.py
+-rw-rw-rw-  2.0 fat     2881 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/_linetypes.py
+-rw-rw-rw-  2.0 fat      778 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/render/__init__.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/16x16.png
+-rw-rw-rw-  2.0 fat     1420 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/24x24.png
+-rw-rw-rw-  2.0 fat    10638 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/256x256.png
+-rw-rw-rw-  2.0 fat     1758 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/32x32.png
+-rw-rw-rw-  2.0 fat     2335 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/48x48.png
+-rw-rw-rw-  2.0 fat     3050 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/64x64.png
+-rw-rw-rw-  2.0 fat     2090 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-copy-64px.png
+-rw-rw-rw-  2.0 fat     3109 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-find-64px.png
+-rw-rw-rw-  2.0 fat     2388 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-goto-bookmark-64px.png
+-rw-rw-rw-  2.0 fat     2519 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-goto-handle-64px.png
+-rw-rw-rw-  2.0 fat     2409 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-goto-line-64px.png
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-left-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2322 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-next-entity-64px.png
+-rw-rw-rw-  2.0 fat     2320 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-prev-entity-64px.png
+-rw-rw-rw-  2.0 fat     2244 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-right-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2553 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-show-in-tree-64px.png
+-rw-rw-rw-  2.0 fat     2373 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/resources/icon-store-bookmark-64px.png
+-rw-rw-rw-  2.0 fat    10650 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/acdsdata.py
+-rw-rw-rw-  2.0 fat    16508 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/blocks.py
+-rw-rw-rw-  2.0 fat    11639 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/classes.py
+-rw-rw-rw-  2.0 fat     4137 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/entities.py
+-rw-rw-rw-  2.0 fat    11953 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/header.py
+-rw-rw-rw-  2.0 fat    60696 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/headervars.py
+-rw-rw-rw-  2.0 fat    27009 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/objects.py
+-rw-rw-rw-  2.0 fat    26581 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/table.py
+-rw-rw-rw-  2.0 fat     5270 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/tables.py
+-rw-rw-rw-  2.0 fat       67 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/sections/__init__.py
+-rw-rw-rw-  2.0 fat    19711 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/analyze.py
+-rw-rw-rw-  2.0 fat    20434 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/binarydata.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/codepage.py
+-rw-rw-rw-  2.0 fat     7645 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/complex_ltype.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/crypt.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/debug.py
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/difftags.py
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/handle.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/indexing.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/juliandate.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/pattern.py
+-rw-rw-rw-  2.0 fat     1256 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/rawloader.py
+-rw-rw-rw-  2.0 fat   129174 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/standards.py
+-rw-rw-rw-  2.0 fat     6049 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/strip.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/test.py
+-rw-rw-rw-  2.0 fat    65523 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/text.py
+-rw-rw-rw-  2.0 fat    54234 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/text_layout.py
+-rw-rw-rw-  2.0 fat     6893 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/text_size.py
+-rw-rw-rw-  2.0 fat     3077 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/zipmanager.py
+-rw-rw-rw-  2.0 fat   142734 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/_iso_pattern.py
+-rw-rw-rw-  2.0 fat     3564 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat    71110 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      302 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    31923 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/src/ezdxf.egg-info/top_level.txt
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_09_cython_acceleration/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_10_issues/
+-rw-rw-rw-  2.0 fat      410 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/conftest.py
+-rw-rw-rw-  2.0 fat     2336 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+-rw-rw-rw-  2.0 fat     1124 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+-rw-rw-rw-  2.0 fat     5456 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+-rw-rw-rw-  2.0 fat      582 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+-rw-rw-rw-  2.0 fat    11593 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+-rw-rw-rw-  2.0 fat     1191 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+-rw-rw-rw-  2.0 fat     4792 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+-rw-rw-rw-  2.0 fat      989 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_018_handle.py
+-rw-rw-rw-  2.0 fat     5518 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+-rw-rw-rw-  2.0 fat     8168 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+-rw-rw-rw-  2.0 fat      401 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+-rw-rw-rw-  2.0 fat      539 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+-rw-rw-rw-  2.0 fat     2092 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_040_tags.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+-rw-rw-rw-  2.0 fat     6419 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+-rw-rw-rw-  2.0 fat    11265 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+-rw-rw-rw-  2.0 fat     1974 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+-rw-rw-rw-  2.0 fat     2321 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+-rw-rw-rw-  2.0 fat      568 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+-rw-rw-rw-  2.0 fat     8682 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+-rw-rw-rw-  2.0 fat     1051 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+-rw-rw-rw-  2.0 fat    11689 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+-rw-rw-rw-  2.0 fat     2893 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_102_appdata.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_103_reactors.py
+-rw-rw-rw-  2.0 fat     4001 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_104_extension_dict.py
+-rw-rw-rw-  2.0 fat    20860 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_105_xdata.py
+-rw-rw-rw-  2.0 fat    14169 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_110_dxfentity.py
+-rw-rw-rw-  2.0 fat     2433 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+-rw-rw-rw-  2.0 fat     6781 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+-rw-rw-rw-  2.0 fat      695 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_112b_dxfobj.py
+-rw-rw-rw-  2.0 fat     2431 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_113_dxfclass.py
+-rw-rw-rw-  2.0 fat     4044 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_114_factory.py
+-rw-rw-rw-  2.0 fat     2256 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+-rw-rw-rw-  2.0 fat    15794 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_116_dictionary.py
+-rw-rw-rw-  2.0 fat     4999 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+-rw-rw-rw-  2.0 fat     3003 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_120_style_table_entry.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+-rw-rw-rw-  2.0 fat      379 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_123_view_table_entry.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_125_image_def.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_127_raster_variables.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_128_pdf_definition.py
+-rw-rw-rw-  2.0 fat     2778 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_129_xrecord.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_130_id_buffer.py
+-rw-rw-rw-  2.0 fat     2470 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_131_field_list.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_132_layer_filter.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_133_sun.py
+-rw-rw-rw-  2.0 fat      852 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_134_material.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_135_geo_data.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_136_vba_project.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_137_sortentstable.py
+-rw-rw-rw-  2.0 fat      704 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_139_user_record.py
+-rw-rw-rw-  2.0 fat      714 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_140_block_record.py
+-rw-rw-rw-  2.0 fat     9199 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/conftest.py
+-rw-rw-rw-  2.0 fat     6532 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_200_line.py
+-rw-rw-rw-  2.0 fat     4273 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_201_point.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_202_circle.py
+-rw-rw-rw-  2.0 fat     8949 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_203_arc.py
+-rw-rw-rw-  2.0 fat     2852 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_204_shape.py
+-rw-rw-rw-  2.0 fat     8242 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_205_solid.py
+-rw-rw-rw-  2.0 fat     8476 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_206_text.py
+-rw-rw-rw-  2.0 fat     6487 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_207_attdef.py
+-rw-rw-rw-  2.0 fat     7922 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_208_attrib.py
+-rw-rw-rw-  2.0 fat     2671 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_209_vertex.py
+-rw-rw-rw-  2.0 fat     5930 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_1.py
+-rw-rw-rw-  2.0 fat    13489 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_2.py
+-rw-rw-rw-  2.0 fat     6650 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+-rw-rw-rw-  2.0 fat     1780 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+-rw-rw-rw-  2.0 fat     7847 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_211_viewport.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_212_insert.py
+-rw-rw-rw-  2.0 fat     6024 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_213_minsert.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_214_block.py
+-rw-rw-rw-  2.0 fat     6882 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_215_dimension.py
+-rw-rw-rw-  2.0 fat     4907 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+-rw-rw-rw-  2.0 fat     6471 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+-rw-rw-rw-  2.0 fat     5535 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+-rw-rw-rw-  2.0 fat     7181 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+-rw-rw-rw-  2.0 fat     3615 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+-rw-rw-rw-  2.0 fat     6919 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_221_ellipse.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_222_xline.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_223_ray.py
+-rw-rw-rw-  2.0 fat     2176 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_224_group.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_225_mtext.py
+-rw-rw-rw-  2.0 fat    12020 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_226_spline.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+-rw-rw-rw-  2.0 fat    10893 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+-rw-rw-rw-  2.0 fat    15116 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_228_mesh.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+-rw-rw-rw-  2.0 fat    21421 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+-rw-rw-rw-  2.0 fat     6587 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+-rw-rw-rw-  2.0 fat    12486 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+-rw-rw-rw-  2.0 fat     2274 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_231_underlay.py
+-rw-rw-rw-  2.0 fat     5243 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_231_underlay_2.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_232_acis.py
+-rw-rw-rw-  2.0 fat     6799 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_232_acis_2.py
+-rw-rw-rw-  2.0 fat     1854 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_232_surface.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_233_helix.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_234_light.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_235_leader.py
+-rw-rw-rw-  2.0 fat    20392 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_236_multileader.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_237_mline.py
+-rw-rw-rw-  2.0 fat     2356 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_238_tolerance.py
+-rw-rw-rw-  2.0 fat    27392 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+-rw-rw-rw-  2.0 fat     4347 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_241_hyperlink.py
+-rw-rw-rw-  2.0 fat    11313 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_242_random_transform.py
+-rw-rw-rw-  2.0 fat     3725 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_243_replace_entity.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+-rw-rw-rw-  2.0 fat     4456 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_245_wipeout.py
+-rw-rw-rw-  2.0 fat     6175 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_246_spline_audit.py
+-rw-rw-rw-  2.0 fat     8165 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+-rw-rw-rw-  2.0 fat     6003 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_248_mpolygon.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+-rw-rw-rw-  2.0 fat     5713 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+-rw-rw-rw-  2.0 fat     7331 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_251_upright.py
+-rw-rw-rw-  2.0 fat     4795 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat     2082 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_253_ole2frame.py
+-rw-rw-rw-  2.0 fat      821 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_254_get_font_name.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_300_layout.py
+-rw-rw-rw-  2.0 fat     4274 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_302_block_references.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+-rw-rw-rw-  2.0 fat      913 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+-rw-rw-rw-  2.0 fat     3279 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_307_groupby.py
+-rw-rw-rw-  2.0 fat    17748 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_308_query.py
+-rw-rw-rw-  2.0 fat     6382 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_309_query_parser.py
+-rw-rw-rw-  2.0 fat     5031 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+-rw-rw-rw-  2.0 fat     5782 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+-rw-rw-rw-  2.0 fat      647 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_313_redraw_order.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+-rw-rw-rw-  2.0 fat     5208 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+-rw-rw-rw-  2.0 fat     6795 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+-rw-rw-rw-  2.0 fat     4981 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+-rw-rw-rw-  2.0 fat     2450 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_405_classes.py
+-rw-rw-rw-  2.0 fat     9094 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+-rw-rw-rw-  2.0 fat      848 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+-rw-rw-rw-  2.0 fat     3375 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+-rw-rw-rw-  2.0 fat     1433 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+-rw-rw-rw-  2.0 fat     5736 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_410_table.py
+-rw-rw-rw-  2.0 fat     6607 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+-rw-rw-rw-  2.0 fat    18072 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+-rw-rw-rw-  2.0 fat    12327 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+-rw-rw-rw-  2.0 fat     6509 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+-rw-rw-rw-  2.0 fat     5656 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+-rw-rw-rw-  2.0 fat     5434 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+-rw-rw-rw-  2.0 fat      733 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+-rw-rw-rw-  2.0 fat     1240 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+-rw-rw-rw-  2.0 fat     5007 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+-rw-rw-rw-  2.0 fat      769 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+-rw-rw-rw-  2.0 fat     7289 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_424_audit.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+-rw-rw-rw-  2.0 fat     2981 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+-rw-rw-rw-  2.0 fat     2416 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+-rw-rw-rw-  2.0 fat     2533 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+-rw-rw-rw-  2.0 fat   112800 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/conftest.py
+-rw-rw-rw-  2.0 fat     5510 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_500_units.py
+-rw-rw-rw-  2.0 fat     1052 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_501_truecolor.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_502_raw_color.py
+-rw-rw-rw-  2.0 fat     1695 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_503_indexing.py
+-rw-rw-rw-  2.0 fat     1442 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_504_suppress_zeros.py
+-rw-rw-rw-  2.0 fat      216 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_506_version.py
+-rw-rw-rw-  2.0 fat      579 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_507_dxf_pretty_printer.py
+-rw-rw-rw-  2.0 fat      657 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_508_read_zip.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_509_comments.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_510_byte_stream.py
+-rw-rw-rw-  2.0 fat     4239 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_511_bit_stream.py
+-rw-rw-rw-  2.0 fat     5595 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_512_pattern.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_513_reorder_entities.py
+-rw-rw-rw-  2.0 fat    17710 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_514_text.py
+-rw-rw-rw-  2.0 fat     9269 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_515a_fonts_truetype.py
+-rw-rw-rw-  2.0 fat     4752 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_515b_fonts_shapefiles.py
+-rw-rw-rw-  2.0 fat     2469 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_515c_fonts_lff.py
+-rw-rw-rw-  2.0 fat     4002 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_516_zoom.py
+-rw-rw-rw-  2.0 fat    34209 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_517_text_layout.py
+-rw-rw-rw-  2.0 fat      474 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_518_header_guid.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_519_mtext_editor.py
+-rw-rw-rw-  2.0 fat     3205 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_520_mtext_context.py
+-rw-rw-rw-  2.0 fat    24496 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_521_mtext_parser.py
+-rw-rw-rw-  2.0 fat     3863 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_522_text_scanner.py
+-rw-rw-rw-  2.0 fat     5207 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_523_text_size.py
+-rw-rw-rw-  2.0 fat     5063 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_524_block_reference_manager.py
+-rw-rw-rw-  2.0 fat      773 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_525_transparency.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_526_explode.py
+-rw-rw-rw-  2.0 fat    13521 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_527_gfxattribs.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_528_difftags.py
+-rw-rw-rw-  2.0 fat     6700 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_529_acis_sat.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_530_acis_sab.py
+-rw-rw-rw-  2.0 fat    12366 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_531_acis_entities.py
+-rw-rw-rw-  2.0 fat     7533 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_532_acis_mesh.py
+-rw-rw-rw-  2.0 fat    43259 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_533_shapefiles.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_534_dwg_info.py
+-rw-rw-rw-  2.0 fat    48174 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_535_xref_basic.py
+-rw-rw-rw-  2.0 fat    27614 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_536_xref_conflict.py
+-rw-rw-rw-  2.0 fat     6887 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_537_transform.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+-rw-rw-rw-  2.0 fat    16358 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_539_npshapes.py
+-rw-rw-rw-  2.0 fat     2605 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_05_tools/test_540_lff_parser.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/conftest.py
+-rw-rw-rw-  2.0 fat     7460 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_600_base.py
+-rw-rw-rw-  2.0 fat     2098 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_601_bulge.py
+-rw-rw-rw-  2.0 fat    14651 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_602_vec3.py
+-rw-rw-rw-  2.0 fat     8956 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_603_vec2.py
+-rw-rw-rw-  2.0 fat     2801 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_604_banded_matrix.py
+-rw-rw-rw-  2.0 fat     9738 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_604_linalg.py
+-rw-rw-rw-  2.0 fat    13943 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_605_matrix44.py
+-rw-rw-rw-  2.0 fat     5888 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_606_convexhull.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_607_perlin_noise.py
+-rw-rw-rw-  2.0 fat     3833 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_608_intersection_line_line_2d.py
+-rw-rw-rw-  2.0 fat     1676 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_609_point_on_line.py
+-rw-rw-rw-  2.0 fat     3171 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_610_ocs.py
+-rw-rw-rw-  2.0 fat     7529 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_611_ucs.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_612_ucs_pass_trough.py
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_613_point_in_poygon.py
+-rw-rw-rw-  2.0 fat    10913 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_614_construct_3d.py
+-rw-rw-rw-  2.0 fat      602 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_615_rytz_axis.py
+-rw-rw-rw-  2.0 fat     5215 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_616_plane.py
+-rw-rw-rw-  2.0 fat      772 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_617_clockwise_orientation.py
+-rw-rw-rw-  2.0 fat     6384 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_618_clipping.py
+-rw-rw-rw-  2.0 fat    10108 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_619_greiner_hormann.py
+-rw-rw-rw-  2.0 fat     2669 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_620_knot.py
+-rw-rw-rw-  2.0 fat    18821 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_621_bspline.py
+-rw-rw-rw-  2.0 fat     7652 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_622_bsplineu.py
+-rw-rw-rw-  2.0 fat    11327 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_623_rbspline.py
+-rw-rw-rw-  2.0 fat    10809 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_624_global_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_626_local_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_627_bspline_basis.py
+-rw-rw-rw-  2.0 fat    10545 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_629_bezier.py
+-rw-rw-rw-  2.0 fat    10714 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_630a_bezier4p_base.py
+-rw-rw-rw-  2.0 fat    10204 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_630b_bezier4p_functions.py
+-rw-rw-rw-  2.0 fat     1683 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_631_euler_spiral.py
+-rw-rw-rw-  2.0 fat     4021 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_632_bezier3p.py
+-rw-rw-rw-  2.0 fat    19575 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_640_bbox.py
+-rw-rw-rw-  2.0 fat     5393 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_641_construction_ray.py
+-rw-rw-rw-  2.0 fat     3673 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_642_construction_line.py
+-rw-rw-rw-  2.0 fat     9459 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_643_construction_box.py
+-rw-rw-rw-  2.0 fat    10941 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_644_construction_circle.py
+-rw-rw-rw-  2.0 fat    10988 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_645_construction_arc.py
+-rw-rw-rw-  2.0 fat     3422 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_646_offset_vertices_2d.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_647_transform_tools.py
+-rw-rw-rw-  2.0 fat     8993 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_648_construction_ellipse.py
+-rw-rw-rw-  2.0 fat     4243 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_650_elliptic_arc_span.py
+-rw-rw-rw-  2.0 fat     9024 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_651_construction_polyline.py
+-rw-rw-rw-  2.0 fat     3168 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_652_approx_param_t.py
+-rw-rw-rw-  2.0 fat     5806 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_653_polyline_intersection.py
+-rw-rw-rw-  2.0 fat     5193 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_654_rtree.py
+-rw-rw-rw-  2.0 fat      788 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_655_dbscan.py
+-rw-rw-rw-  2.0 fat      834 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_656_k_means.py
+-rw-rw-rw-  2.0 fat     4654 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_657_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    11654 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_658_bevel_tools.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1428 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+-rw-rw-rw-  2.0 fat     3307 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_06_math/test_662_is_convex_polygon_2d.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_701_arrows.py
+-rw-rw-rw-  2.0 fat    17245 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_702_render_forms.py
+-rw-rw-rw-  2.0 fat    34220 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_703_mesh_builder.py
+-rw-rw-rw-  2.0 fat     4459 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_704_render_linear_dimension.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_705_shape.py
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_706_random_path.py
+-rw-rw-rw-  2.0 fat     5603 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_707_trace.py
+-rw-rw-rw-  2.0 fat    33999 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_708a_path.py
+-rw-rw-rw-  2.0 fat    27351 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_708b_path_tools.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_708c_matplotlib_path_tools.py
+-rw-rw-rw-  2.0 fat     3261 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_708d_qpainter_path_tools.py
+-rw-rw-rw-  2.0 fat     4589 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_708e_path_shapes.py
+-rw-rw-rw-  2.0 fat     4121 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_708f_path_nesting.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_709_linetype_renderer.py
+-rw-rw-rw-  2.0 fat     2815 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_711_points.py
+-rw-rw-rw-  2.0 fat     6594 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_712_render_curved_dimension.py
+-rw-rw-rw-  2.0 fat     1472 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_713_mleader_builder.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_714_mleader_render_engine.py
+-rw-rw-rw-  2.0 fat    11778 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_715_hatching.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_800_mtext_surrogate.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_801_r12spline.py
+-rw-rw-rw-  2.0 fat     7881 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_802_table_painter.py
+-rw-rw-rw-  2.0 fat    12386 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_803_entities_to_code.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_804_importer.py
+-rw-rw-rw-  2.0 fat     2362 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_805_pycsg.py
+-rw-rw-rw-  2.0 fat    15467 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_806_acadctb.py
+-rw-rw-rw-  2.0 fat     4860 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_807_dwg_loader_basics.py
+-rw-rw-rw-  2.0 fat    10862 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_810_drawing_properties.py
+-rw-rw-rw-  2.0 fat    11597 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_811a_drawing_frontend.py
+-rw-rw-rw-  2.0 fat     8684 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_811b_drawing_recorder.py
+-rw-rw-rw-  2.0 fat     2898 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_811c_viewport_processing.py
+-rw-rw-rw-  2.0 fat     4157 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+-rw-rw-rw-  2.0 fat    13751 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_813_geo_interface.py
+-rw-rw-rw-  2.0 fat    14853 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_814_text2path.py
+-rw-rw-rw-  2.0 fat    16239 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_815_dxf_browser.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_816_bin_packing.py
+-rw-rw-rw-  2.0 fat    12554 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_817_genetic_algorithm.py
+-rw-rw-rw-  2.0 fat     9008 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_818_meshex.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_819_menger_sponge.py
+-rw-rw-rw-  2.0 fat     4433 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_820_openscad.py
+-rw-rw-rw-  2.0 fat    15655 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_821_hpgl2.py
+-rw-rw-rw-  2.0 fat     1376 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+-rw-rw-rw-  2.0 fat     1028 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_822_clipper.py
+-rw-rw-rw-  2.0 fat     5284 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_823_drawing_layout.py
+-rw-rw-rw-  2.0 fat     3312 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_824_svg_drawing_backend.py
+-rw-rw-rw-  2.0 fat     2014 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+-rw-rw-rw-  2.0 fat     2527 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+-rw-rw-rw-  2.0 fat     2199 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+-rw-rw-rw-  2.0 fat     2142 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+-rw-rw-rw-  2.0 fat     1452 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+-rw-rw-rw-  2.0 fat     4755 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_10_issues/test_issue_414_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     1213 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_10_issues/test_issue_574_flattening_error.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+-rw-rw-rw-  2.0 fat      682 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_10_issues/test_issue_749_text_layout.py
+-rw-rw-rw-  2.0 fat    11094 b- defN 23-Jul-09 08:08 ezdxf-1.1.0b5/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+841 files, 8749919 bytes uncompressed, 1971853 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -1,2524 +1,2524 @@
-Filename: ezdxf-1.1.0b4/
+Filename: ezdxf-1.1.0b5/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/
+Filename: ezdxf-1.1.0b5/integration_tests/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/
+Filename: ezdxf-1.1.0b5/src/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/
+Filename: ezdxf-1.1.0b5/tests/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/LICENSE
+Filename: ezdxf-1.1.0b5/LICENSE
 Comment: 
 
-Filename: ezdxf-1.1.0b4/MANIFEST.in
+Filename: ezdxf-1.1.0b5/MANIFEST.in
 Comment: 
 
-Filename: ezdxf-1.1.0b4/NEWS.md
+Filename: ezdxf-1.1.0b5/NEWS.md
 Comment: 
 
-Filename: ezdxf-1.1.0b4/PKG-INFO
+Filename: ezdxf-1.1.0b5/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.1.0b4/README.md
+Filename: ezdxf-1.1.0b5/README.md
 Comment: 
 
-Filename: ezdxf-1.1.0b4/requirements.txt
+Filename: ezdxf-1.1.0b5/requirements.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b4/setup.cfg
+Filename: ezdxf-1.1.0b5/setup.cfg
 Comment: 
 
-Filename: ezdxf-1.1.0b4/setup.py
+Filename: ezdxf-1.1.0b5/setup.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/
+Filename: ezdxf-1.1.0b5/integration_tests/data/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_config_file.py
+Filename: ezdxf-1.1.0b5/integration_tests/check_disable_c_ext_by_config_file.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_env_var.py
+Filename: ezdxf-1.1.0b5/integration_tests/check_disable_c_ext_by_env_var.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/conftest.py
+Filename: ezdxf-1.1.0b5/integration_tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_acad_table.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_acad_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_all_dimline_styles.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_all_dimline_styles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_all_ellipse_transformations.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_all_ellipse_transformations.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_anonymous_blocks.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_anonymous_blocks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_audit_critical_dxf_files.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_audit_critical_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_audit_layouts.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_audit_layouts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_complex_line_type_2.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_complex_line_type_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_create_basic_graphics.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_create_basic_graphics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_document_guid.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_document_guid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_document_page_setup.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_document_page_setup.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_dxf_info_scanning.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_dxf_info_scanning.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_entities_iterator.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_entities_iterator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_fix_dulicate_handles.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_fix_dulicate_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_geo.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_geo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_groups.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_groups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_hpgl2_addon.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_hpgl2_addon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_ignore_junk_beyond_EOF.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_ignore_junk_beyond_EOF.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_launcher.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_launcher.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_leica_disto_r12.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_leica_disto_r12.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_load_dxf_unicode_notation.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_load_dxf_unicode_notation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_mapbox_earcut.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_mtext_columns.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_mtext_explode_addon.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_mtext_explode_addon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_mtext_text_frame.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_mtext_text_frame.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_new_table_entries.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_new_table_entries.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_none_ascii_read_write.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_none_ascii_read_write.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_odafc.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_odafc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_open_binary_DXF_files.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_open_binary_DXF_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_open_coord_order_issue.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_open_coord_order_issue.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_open_exotic_dxf_files.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_open_exotic_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_open_R13_R14.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_open_R13_R14.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_polyline_entity.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_polyline_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_preserve_binary_data_in_xrecords.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_preserve_binary_data_in_xrecords.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_r12export.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_r12export.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_r12strict.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_r12strict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_r12writer.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_r12writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_read_file_without_handles.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_read_file_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_read_write_modern_entites.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_read_write_modern_entites.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_recover.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_recover.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_redraw_order.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_rotated_block_attributes.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_rotated_block_attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_surface_entities.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_surface_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_write_fixed_meta_data.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_write_fixed_meta_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_write_without_handles.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_write_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/test_xref_detach.py
+Filename: ezdxf-1.1.0b5/integration_tests/test_xref_detach.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/AC1003_LINE_Example.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/AC1003_LINE_Example.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/acad_table_with_blk_ref.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/acad_table_with_blk_ref.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/ASCII_R12.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/ASCII_R12.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r12.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r12.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r13.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r14.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r2000.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r2000.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/cc_dxflib.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/cc_dxflib.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/custom_blocks.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/custom_blocks.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/duplicate_handles.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/duplicate_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/dxf_unicode.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/dxf_unicode.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/empty_handles.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/empty_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/groups.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/groups.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/Leica_Disto_S910.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/Leica_Disto_S910.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/MODEL.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/MODEL.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2007.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/mtext_columns_R2007.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2018.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/mtext_columns_R2018.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/mtext_framed_columns.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/mtext_framed_columns.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/mtext_text_frame.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/mtext_text_frame.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/no_layouts.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/no_layouts.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/PLOTFILE.plt
+Filename: ezdxf-1.1.0b5/integration_tests/data/PLOTFILE.plt
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/POLI-ALL210_12.DXF
+Filename: ezdxf-1.1.0b5/integration_tests/data/POLI-ALL210_12.DXF
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/R12_with_trash_beyond_EOF.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/recover01.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/recover01.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/recover02.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/recover02.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/small_r13.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/small_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/small_r14.dxf
+Filename: ezdxf-1.1.0b5/integration_tests/data/small_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/XRECORD_0.bin
+Filename: ezdxf-1.1.0b5/integration_tests/data/XRECORD_0.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/XRECORD_1.bin
+Filename: ezdxf-1.1.0b5/integration_tests/data/XRECORD_1.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b4/integration_tests/data/XRECORD_2.bin
+Filename: ezdxf-1.1.0b5/integration_tests/data/XRECORD_2.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/
+Filename: ezdxf-1.1.0b5/src/ezdxf/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/
+Filename: ezdxf-1.1.0b5/src/ezdxf.egg-info/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/
+Filename: ezdxf-1.1.0b5/src/ezdxf/fonts/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/
+Filename: ezdxf-1.1.0b5/src/ezdxf/layouts/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/path/
+Filename: ezdxf-1.1.0b5/src/ezdxf/path/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/appsettings.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/appsettings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/audit.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/bbox.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/blkrefs.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/blkrefs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/colors.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/colors.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/commands.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/comments.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/comments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/disassemble.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/disassemble.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/document.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/document.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/dwginfo.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/dwginfo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entitydb.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entitydb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/enums.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/enums.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/explode.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/eztypes.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/eztypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/filemanagement.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/filemanagement.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/gfxattribs.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/graphicsfactory.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/graphicsfactory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/groupby.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/groupby.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/npshapes.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/npshapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/protocols.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/protocols.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/proxygraphic.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/proxygraphic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/py.typed
+Filename: ezdxf-1.1.0b5/src/ezdxf/py.typed
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/query.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/query.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/queryparser.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/queryparser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/r12strict.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/r12strict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/recover.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/recover.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/reorder.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/reorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/transform.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/units.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/units.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/upright.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/upright.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/urecord.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/urecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/version.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/version.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/xref.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/xref.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/zoom.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/zoom.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/_options.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/_options.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/__main__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/__main__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/bezier3p.pyx
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/bezier3p.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/bezier4p.pyx
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/bezier4p.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/bspline.pyx
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/bspline.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/construct.pxd
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/construct.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/construct.pyx
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/construct.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/linetypes.pyx
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/linetypes.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/mapbox_earcut.pyx
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/mapbox_earcut.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/matrix44.pxd
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/matrix44.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/matrix44.pyx
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/matrix44.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/np_support.pyx
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/np_support.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/vector.pxd
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/vector.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/vector.pyx
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/vector.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_cubic_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_cubic_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_cubic_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.cpp
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_quad_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.hpp
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_quad_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.pxd
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_quad_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.hpp
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_vec3.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.pxd
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_vec3.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acc/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acc/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/abstract.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/abstract.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/api.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/api.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/const.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/dbg.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/dbg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/dxf.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/dxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/entities.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/hdr.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/hdr.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/mesh.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/sab.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/sab.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/sat.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/sat.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/acis/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/acis/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/acisbrowser/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/browser/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/dwg/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/acadctb.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/acadctb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/binpacking.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/binpacking.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dimlines.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/dimlines.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dxf2code.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/dxf2code.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/genetic_algorithm.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/geo.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/geo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/gerber_D6673.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/gerber_D6673.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/importer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/importer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/iterdxf.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/iterdxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/menger_sponge.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/meshex.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/meshex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/mixins.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/mixins.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/mtextsurrogate.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/mtextsurrogate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/mtxpl.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/mtxpl.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/odafc.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/odafc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/openscad.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/openscad.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/pycsg.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/pycsg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/r12export.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/r12export.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/r12writer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/r12writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/sierpinski_pyramid.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/sierpinski_pyramid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/tablepainter.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/tablepainter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/text2path.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/text2path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/xplayer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/xplayer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/xqt.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/xqt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/browser.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/acisbrowser/browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/data.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/acisbrowser/data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/acisbrowser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/bookmarks.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/browser/bookmarks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/browser.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/browser/browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/data.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/browser/data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/find_dialog.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/browser/find_dialog.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/loader.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/browser/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/model.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/browser/model.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/tags.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/browser/tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/views.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/browser/views.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/browser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/backend.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/clipper.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/clipper.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/config.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/config.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_backend.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/debug_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_utils.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/debug_utils.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/designer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/designer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/dxf.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/dxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/frontend.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/frontend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/gfxproxy.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/gfxproxy.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/hpgl2.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/layout.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/matplotlib.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/matplotlib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/mtext_complex.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/mtext_complex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/properties.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pymupdf.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/pymupdf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pyqt.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/pyqt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/qtviewer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/qtviewer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/recorder.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/recorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/svg.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/svg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text_renderer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/type_hints.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/unified_text_renderer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/unified_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/drawing/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/classes_section.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/dwg/classes_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/const.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/dwg/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/crc.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/dwg/crc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/fileheader.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/dwg/fileheader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/header_section.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/dwg/header_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/loader.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/dwg/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/dwg/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/api.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/api.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/backend.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/deps.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/deps.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/interpreter.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/interpreter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/page.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/page.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/plotter.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/plotter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/polygon_buffer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/polygon_buffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/properties.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/tokenizer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/tokenizer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/viewer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/viewer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/acad_proxy_entity.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/acad_table.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/acad_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/acis.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/acis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/appdata.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/appdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/appid.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/appid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/arc.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/attrib.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/attrib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/block.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/block.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/blockrecord.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/blockrecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/boundary_paths.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/circle.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dictionary.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/dictionary.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dimension.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dimstyle.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/dimstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dimstyleoverride.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/dimstyleoverride.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfclass.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfentity.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfgfx.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfgroups.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfns.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/dxfns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfobj.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/ellipse.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/factory.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/factory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/geodata.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/geodata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/gradient.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/gradient.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/hatch.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/hatch.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/helix.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/helix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/idbuffer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/idbuffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/image.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/image.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/insert.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/insert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/layer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/layer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/layout.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/leader.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/light.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/light.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/line.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/ltype.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/ltype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/lwpolyline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/lwpolyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/material.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/material.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mesh.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mleader.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/mleader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mpolygon.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mtext.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/mtext.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mtext_columns.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/objectcollection.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/objectcollection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/oleframe.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/oleframe.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/pattern.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/point.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/polygon.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/polygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/polyline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/shape.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/solid.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/solid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/spline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/subentity.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/subentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/sun.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/sun.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/table.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/text.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/textstyle.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/textstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/tolerance.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/tolerance.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/ucs.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/underlay.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/underlay.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/view.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/view.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/viewport.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/viewport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/visualstyle.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/visualstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/vport.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/vport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/xdata.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/xdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/xdict.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/xdict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/xline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/xline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/entities/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/entities/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/fonts.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/fonts/fonts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/font_face.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/fonts/font_face.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/font_manager.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/fonts/font_manager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/font_measurements.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/fonts/font_measurements.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/glyphs.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/fonts/glyphs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/lff.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/fonts/lff.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/shapefile.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/fonts/shapefile.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/ttfonts.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/fonts/ttfonts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/fonts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/base.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/layouts/base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/blocklayout.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/layouts/blocklayout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/layout.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/layouts/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/layouts.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/layouts/layouts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/layouts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/attributes.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/const.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/encoding.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/encoding.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/extendedtags.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/extendedtags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/fileindex.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/fileindex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/hdrvars.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/hdrvars.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/loader.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/packedtags.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/packedtags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/repair.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/repair.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/tagger.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/tagger.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/tags.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/tagwriter.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/tagwriter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/types.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/types.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/validator.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/validator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/lldxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/arc.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/bbox.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/bezier.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/bezier.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/bezier_interpolation.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/bezier_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/box.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/box.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/bspline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/bulge.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/bulge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/circle.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/clipping.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/clipping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/clustering.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/clustering.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/construct2d.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/construct2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/construct3d.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/construct3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/cspline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/cspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/curvetools.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/curvetools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/ellipse.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/eulerspiral.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/eulerspiral.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/linalg.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/linalg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/line.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/offset2d.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/offset2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/parametrize.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/parametrize.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/perlin.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/perlin.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/polyline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/rtree.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/rtree.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/shape.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/surfaces.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/surfaces.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/transformtools.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/transformtools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/triangulation.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/triangulation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/ucs.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/_bezier3p.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/_bezier4p.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/_bspline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/_construct.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/_construct.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/_ctypes.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/_ctypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/_mapbox_earcut.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/_matrix44.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/_vector.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/_vector.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/math/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/math/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/path/commands.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/path/commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/path/converter.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/path/converter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/path/nesting.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/path/nesting.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/path/path.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/path/path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/path/shapes.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/path/shapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/path/tools.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/path/tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/path/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/path/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.css
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.css
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.html
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.html
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.js
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.js
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/pprint.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/pprint.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.css
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/rawpp.css
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.html
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/rawpp.html
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/rawpp.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/reflinks.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/reflinks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/pp/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/pp/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/abstract_mtext_renderer.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/abstract_mtext_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/arrows.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/arrows.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/curves.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/curves.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/dimension.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_base.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/dim_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_curved.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/dim_curved.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_diameter.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/dim_diameter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_linear.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/dim_linear.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_ordinate.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/dim_ordinate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_radius.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/dim_radius.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/forms.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/forms.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/hatching.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/hatching.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/leader.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/linetypes.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/linetypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/mesh.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/mleader.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/mleader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/mline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/point.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/polyline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/r12spline.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/r12spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/trace.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/trace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/_linetypes.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/_linetypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/render/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/render/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/16x16.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/16x16.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/24x24.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/24x24.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/256x256.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/256x256.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/32x32.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/32x32.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/48x48.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/48x48.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/64x64.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/64x64.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-copy-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-copy-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-find-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-find-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-bookmark-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-goto-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-handle-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-goto-handle-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-line-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-goto-line-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-left-arrow-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-left-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-next-entity-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-next-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-prev-entity-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-prev-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-right-arrow-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-right-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-show-in-tree-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-show-in-tree-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-store-bookmark-64px.png
+Filename: ezdxf-1.1.0b5/src/ezdxf/resources/icon-store-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/acdsdata.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/acdsdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/blocks.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/blocks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/classes.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/classes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/entities.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/header.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/header.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/headervars.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/headervars.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/objects.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/objects.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/table.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/tables.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/tables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/sections/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/sections/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/analyze.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/analyze.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/binarydata.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/binarydata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/codepage.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/codepage.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/complex_ltype.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/complex_ltype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/crypt.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/crypt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/debug.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/debug.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/difftags.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/difftags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/handle.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/handle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/indexing.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/indexing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/juliandate.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/juliandate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/pattern.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/rawloader.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/rawloader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/standards.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/standards.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/strip.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/strip.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/test.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/test.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/text.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/text_layout.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/text_size.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/text_size.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/zipmanager.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/zipmanager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/_iso_pattern.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/_iso_pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf/tools/__init__.py
+Filename: ezdxf-1.1.0b5/src/ezdxf/tools/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/dependency_links.txt
+Filename: ezdxf-1.1.0b5/src/ezdxf.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/entry_points.txt
+Filename: ezdxf-1.1.0b5/src/ezdxf.egg-info/entry_points.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/not-zip-safe
+Filename: ezdxf-1.1.0b5/src/ezdxf.egg-info/not-zip-safe
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/PKG-INFO
+Filename: ezdxf-1.1.0b5/src/ezdxf.egg-info/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/requires.txt
+Filename: ezdxf-1.1.0b5/src/ezdxf.egg-info/requires.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/SOURCES.txt
+Filename: ezdxf-1.1.0b5/src/ezdxf.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/top_level.txt
+Filename: ezdxf-1.1.0b5/src/ezdxf.egg-info/top_level.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/
+Filename: ezdxf-1.1.0b5/tests/test_06_math/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/
+Filename: ezdxf-1.1.0b5/tests/test_07_render/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/
+Filename: ezdxf-1.1.0b5/tests/test_09_cython_acceleration/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_10_issues/
+Filename: ezdxf-1.1.0b5/tests/test_10_issues/
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/conftest.py
+Filename: ezdxf-1.1.0b5/tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_011_codepage.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_012_crypt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_016_encoding.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_018_handle.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_018_handle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_040_tags.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_040_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+Filename: ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_101_dxfnamespace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_102_appdata.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_102_appdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_103_reactors.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_103_reactors.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_104_extension_dict.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_104_extension_dict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_105_xdata.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_105_xdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_110_dxfentity.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_110_dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_112a_dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112b_dxfobj.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_112b_dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_113_dxfclass.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_113_dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_114_factory.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_114_factory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_116_dictionary.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_116_dictionary.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_117_layer_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_118_appid_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_120_style_table_entry.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_120_style_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_122_vport_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_123_view_table_entry.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_123_view_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_125_image_def.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_125_image_def.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_126_image_def_reactor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_127_raster_variables.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_127_raster_variables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_128_pdf_definition.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_128_pdf_definition.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_129_xrecord.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_129_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_130_id_buffer.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_130_id_buffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_131_field_list.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_131_field_list.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_132_layer_filter.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_132_layer_filter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_133_sun.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_133_sun.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_134_material.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_134_material.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_135_geo_data.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_135_geo_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_136_vba_project.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_136_vba_project.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_137_sortentstable.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_137_sortentstable.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_139_user_record.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_139_user_record.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_140_block_record.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_140_block_record.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+Filename: ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_141_layer_vp_override.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/conftest.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_200_line.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_200_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_201_point.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_201_point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_202_circle.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_202_circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_203_arc.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_203_arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_204_shape.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_204_shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_205_solid.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_205_solid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_206_text.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_206_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_207_attdef.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_207_attdef.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_208_attrib.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_208_attrib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_209_vertex.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_209_vertex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_1.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_1.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_2.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_211_viewport.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_211_viewport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_212_insert.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_212_insert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_213_minsert.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_213_minsert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_214_block.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_214_block.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_215_dimension.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_215_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_221_ellipse.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_221_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_222_xline.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_222_xline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_223_ray.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_223_ray.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_224_group.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_224_group.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_225_mtext.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_225_mtext.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_226_spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_228_mesh.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_228_mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_231_underlay.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay_2.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_231_underlay_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_232_acis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis_2.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_232_acis_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_surface.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_232_surface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_233_helix.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_233_helix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_234_light.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_234_light.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_235_leader.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_235_leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_236_multileader.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_236_multileader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_237_mline.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_237_mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_238_tolerance.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_238_tolerance.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_240_arc_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_241_hyperlink.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_241_hyperlink.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_242_random_transform.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_242_random_transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_243_replace_entity.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_243_replace_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_245_wipeout.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_245_wipeout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_246_spline_audit.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_246_spline_audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mpolygon.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_248_mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_249_boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_251_upright.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_251_upright.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_253_ole2frame.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_253_ole2frame.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_254_get_font_name.py
+Filename: ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_254_get_font_name.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_300_layout.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_300_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_302_block_references.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_302_block_references.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_303_auto_block_references.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_304_new_entity_space.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_307_groupby.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_307_groupby.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_308_query.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_308_query.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_309_query_parser.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_309_query_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_312_virtual_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_313_redraw_order.py
+Filename: ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_313_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_401_headersection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_402_classessection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_404a_tables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_405_classes.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_405_classes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_410_table.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_410_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_417_bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_424_audit.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_424_audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+Filename: ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/conftest.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_500_units.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_500_units.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_501_truecolor.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_501_truecolor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_502_raw_color.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_502_raw_color.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_503_indexing.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_503_indexing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_504_suppress_zeros.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_504_suppress_zeros.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_506_version.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_506_version.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_507_dxf_pretty_printer.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_507_dxf_pretty_printer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_508_read_zip.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_508_read_zip.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_509_comments.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_509_comments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_510_byte_stream.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_510_byte_stream.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_511_bit_stream.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_511_bit_stream.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_512_pattern.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_512_pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_513_reorder_entities.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_513_reorder_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_514_text.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_514_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_515a_fonts_truetype.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_515a_fonts_truetype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_515b_fonts_shapefiles.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_515b_fonts_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_515c_fonts_lff.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_515c_fonts_lff.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_516_zoom.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_516_zoom.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_517_text_layout.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_517_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_518_header_guid.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_518_header_guid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_519_mtext_editor.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_519_mtext_editor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_520_mtext_context.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_520_mtext_context.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_521_mtext_parser.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_521_mtext_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_522_text_scanner.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_522_text_scanner.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_523_text_size.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_523_text_size.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_524_block_reference_manager.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_524_block_reference_manager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_525_transparency.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_525_transparency.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_526_explode.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_526_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_527_gfxattribs.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_527_gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_528_difftags.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_528_difftags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_529_acis_sat.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_529_acis_sat.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_530_acis_sab.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_530_acis_sab.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_531_acis_entities.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_531_acis_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_532_acis_mesh.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_532_acis_mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_533_shapefiles.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_533_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_534_dwg_info.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_534_dwg_info.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_535_xref_basic.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_535_xref_basic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_536_xref_conflict.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_536_xref_conflict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_537_transform.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_537_transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_539_npshapes.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_539_npshapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_540_lff_parser.py
+Filename: ezdxf-1.1.0b5/tests/test_05_tools/test_540_lff_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/conftest.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_600_base.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_600_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_601_bulge.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_601_bulge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_602_vec3.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_602_vec3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_603_vec2.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_603_vec2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_604_banded_matrix.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_604_banded_matrix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_604_linalg.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_604_linalg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_605_matrix44.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_605_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_606_convexhull.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_606_convexhull.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_607_perlin_noise.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_607_perlin_noise.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_608_intersection_line_line_2d.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_608_intersection_line_line_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_609_point_on_line.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_609_point_on_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_610_ocs.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_610_ocs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_611_ucs.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_611_ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_612_ucs_pass_trough.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_612_ucs_pass_trough.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_613_point_in_poygon.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_613_point_in_poygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_614_construct_3d.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_614_construct_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_615_rytz_axis.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_615_rytz_axis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_616_plane.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_616_plane.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_617_clockwise_orientation.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_617_clockwise_orientation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_618_clipping.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_618_clipping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_619_greiner_hormann.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_619_greiner_hormann.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_620_knot.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_620_knot.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_621_bspline.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_621_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_622_bsplineu.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_622_bsplineu.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_623_rbspline.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_623_rbspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_624_global_bspline_interpolation.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_624_global_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_626_local_bspline_interpolation.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_626_local_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_627_bspline_basis.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_627_bspline_basis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_629_bezier.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_629_bezier.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_630a_bezier4p_base.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_630a_bezier4p_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_630b_bezier4p_functions.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_630b_bezier4p_functions.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_631_euler_spiral.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_631_euler_spiral.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_632_bezier3p.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_632_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_640_bbox.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_640_bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_641_construction_ray.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_641_construction_ray.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_642_construction_line.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_642_construction_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_643_construction_box.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_643_construction_box.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_644_construction_circle.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_644_construction_circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_645_construction_arc.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_645_construction_arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_646_offset_vertices_2d.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_646_offset_vertices_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_647_transform_tools.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_647_transform_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_648_construction_ellipse.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_648_construction_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_650_elliptic_arc_span.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_650_elliptic_arc_span.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_651_construction_polyline.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_651_construction_polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_652_approx_param_t.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_652_approx_param_t.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_653_polyline_intersection.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_653_polyline_intersection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_654_rtree.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_654_rtree.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_655_dbscan.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_655_dbscan.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_656_k_means.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_656_k_means.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_657_mapbox_earcut.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_657_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_658_bevel_tools.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_658_bevel_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_659_intersection_line_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_06_math/test_662_is_convex_polygon_2d.py
+Filename: ezdxf-1.1.0b5/tests/test_06_math/test_662_is_convex_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_701_arrows.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_701_arrows.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_702_render_forms.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_702_render_forms.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_703_mesh_builder.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_703_mesh_builder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_704_render_linear_dimension.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_704_render_linear_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_705_shape.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_705_shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_706_random_path.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_706_random_path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_707_trace.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_707_trace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708a_path.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_708a_path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708b_path_tools.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_708b_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708c_matplotlib_path_tools.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_708c_matplotlib_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708d_qpainter_path_tools.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_708d_qpainter_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708e_path_shapes.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_708e_path_shapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708f_path_nesting.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_708f_path_nesting.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_709_linetype_renderer.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_709_linetype_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_711_points.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_711_points.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_712_render_curved_dimension.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_712_render_curved_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_713_mleader_builder.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_713_mleader_builder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_714_mleader_render_engine.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_714_mleader_render_engine.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_715_hatching.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_715_hatching.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+Filename: ezdxf-1.1.0b5/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_800_mtext_surrogate.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_800_mtext_surrogate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_801_r12spline.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_801_r12spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_802_table_painter.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_802_table_painter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_803_entities_to_code.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_803_entities_to_code.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_804_importer.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_804_importer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_805_pycsg.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_805_pycsg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_806_acadctb.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_806_acadctb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_807_dwg_loader_basics.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_807_dwg_loader_basics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_810_drawing_properties.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_810_drawing_properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_811a_drawing_frontend.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_811a_drawing_frontend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_811b_drawing_recorder.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_811b_drawing_recorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_811c_viewport_processing.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_811c_viewport_processing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_812_drawing_graphic_proxy.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_813_geo_interface.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_813_geo_interface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_814_text2path.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_814_text2path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_815_dxf_browser.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_815_dxf_browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_816_bin_packing.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_816_bin_packing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_817_genetic_algorithm.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_817_genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_818_meshex.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_818_meshex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_819_menger_sponge.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_819_menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_820_openscad.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_820_openscad.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_821_hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_822_clipper.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_822_clipper.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_823_drawing_layout.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_823_drawing_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_824_svg_drawing_backend.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_824_svg_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+Filename: ezdxf-1.1.0b5/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Filename: ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_901_acc_vec2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Filename: ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_902_acc_vec3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Filename: ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Filename: ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Filename: ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Filename: ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_906_acc_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Filename: ezdxf-1.1.0b5/tests/test_10_issues/test_issue_414_bbox_calculation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Filename: ezdxf-1.1.0b5/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_574_flattening_error.py
+Filename: ezdxf-1.1.0b5/tests/test_10_issues/test_issue_574_flattening_error.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Filename: ezdxf-1.1.0b5/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_749_text_layout.py
+Filename: ezdxf-1.1.0b5/tests/test_10_issues/test_issue_749_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+Filename: ezdxf-1.1.0b5/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ezdxf-1.1.0b4/LICENSE` & `ezdxf-1.1.0b5/LICENSE`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/NEWS.md` & `ezdxf-1.1.0b5/NEWS.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 - NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
   add-on to change/override foreground- and background color by the frontend 
 - NEW: `TextPolicy` configuration settings for the `drawing` add-on, render text as 
   solid filling, outline path, replace text by (filled) rectangles or ignore text at all 
 - NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
   stroke fonts included in CAD applications
 - NEW: added setter to `BlockLayout.base_point` property
+- NEW: `ezdxf.entities.acad_table_to_block()` function, converts a `ACAD_TABLE` entity 
+  to an `INSERT` entity
+- NEW: `ACADProxyEntity.explode()` method, to explode `ACAD_PROXY_ENTITY` into proxy 
+  graphic entities
 - CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
   including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
 - REMOVED: configuration option `use_matplotlib` - is not needed anymore
 - REMOVED: configuration option `font_cache_directory` - is not needed anymore
@@ -39,15 +43,20 @@
 - REMOVED: Matplotlib/Qt path converters from `ezdxf.path.converter`
 - REMOVED: `Pillow` backend and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
 - BUGFIX: [#898](https://github.com/mozman/ezdxf/issues/898)
-  use `dimclrd` color for dimension arrow blocks 
+  use `dimclrd` color for dimension arrow blocks
+- BUGFIX: [#906](https://github.com/mozman/ezdxf/issues/906)
+  linetype and fill flag parsing for proxy graphics 
+- BUGFIX: [#907](https://github.com/mozman/ezdxf/issues/907)
+  fix ATTRIB and ATTDEF handling of version- and lock_position tags which share the 
+  same group code 280 in the same subclass
 
 Version 1.0.3 - 2023-03-26
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing
```

## Comparing `ezdxf-1.1.0b4/PKG-INFO` & `ezdxf-1.1.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.1.0b4
+Version: 1.1.0b5
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -66,14 +66,15 @@
 - read/write/new support for DXF versions: R12, R2000, R2004, R2007, R2010, R2013 and R2018
 - additional read-only support for DXF versions R13/R14 (upgraded to R2000)
 - additional read-only support for older DXF versions than R12 (upgraded to R12)
 - read/write support for ASCII DXF and Binary DXF
 - retains third-party DXF content
 - optional C-extensions for CPython are included in the binary wheels, available 
   on [PyPI](https://pypi.org/project/ezdxf/) for Windows, Linux and macOS
+- command line script `ezdxf` to display, convert and inspect DXF files
 
 Included Extensions
 -------------------
 
 Additional packages required for these add-ons are not automatically installed 
 during the *basic* setup, for more information about the setup & dependencies 
 visit the [documentation](https://ezdxf.mozman.at/docs/setup.html).
@@ -159,14 +160,48 @@
 drawing add-on:
 
     pip install ezdxf[draw]
 
 For more information about the setup & dependencies visit the 
 [documentation](https://ezdxf.mozman.at/docs/setup.html).
 
+Command Line
+------------
+
+Use `python -m ezdxf ...` if your shell can't find the `ezdxf` script.
+
+Get additional help for a sub-command:
+
+    ezdxf <cmd> -h
+
+Preview DXF files in a graphical window:
+
+    ezdxf view <file.dxf>
+
+Export the modelspace of DXF files as PNG|SVG|PDF:
+
+    ezdxf draw -o file.<png|svg|pdf> <file.dxf>
+
+Print basic information about DXF files:
+
+    ezdxf info <file.dxf>
+
+Show detailed information and structures of DXF files:
+
+    ezdxf browse <file.dxf>
+
+Audit DXF files:
+
+    ezdxf audit <file.dxf>
+
+Preview and convert HPGL/2 plot files:
+
+    ezdxf hpgl <file.plt>
+
+
 Website
 -------
 
 https://ezdxf.mozman.at/
 
 Documentation
 -------------
@@ -233,14 +268,18 @@
 - NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
   add-on to change/override foreground- and background color by the frontend 
 - NEW: `TextPolicy` configuration settings for the `drawing` add-on, render text as 
   solid filling, outline path, replace text by (filled) rectangles or ignore text at all 
 - NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
   stroke fonts included in CAD applications
 - NEW: added setter to `BlockLayout.base_point` property
+- NEW: `ezdxf.entities.acad_table_to_block()` function, converts a `ACAD_TABLE` entity 
+  to an `INSERT` entity
+- NEW: `ACADProxyEntity.explode()` method, to explode `ACAD_PROXY_ENTITY` into proxy 
+  graphic entities
 - CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
   including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
 - REMOVED: configuration option `use_matplotlib` - is not needed anymore
 - REMOVED: configuration option `font_cache_directory` - is not needed anymore
@@ -252,15 +291,20 @@
 - REMOVED: Matplotlib/Qt path converters from `ezdxf.path.converter`
 - REMOVED: `Pillow` backend and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
 - BUGFIX: [#898](https://github.com/mozman/ezdxf/issues/898)
-  use `dimclrd` color for dimension arrow blocks 
+  use `dimclrd` color for dimension arrow blocks
+- BUGFIX: [#906](https://github.com/mozman/ezdxf/issues/906)
+  linetype and fill flag parsing for proxy graphics 
+- BUGFIX: [#907](https://github.com/mozman/ezdxf/issues/907)
+  fix ATTRIB and ATTDEF handling of version- and lock_position tags which share the 
+  same group code 280 in the same subclass
 
 Version 1.0.3 - 2023-03-26
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing
```

## Comparing `ezdxf-1.1.0b4/README.md` & `ezdxf-1.1.0b5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 - read/write/new support for DXF versions: R12, R2000, R2004, R2007, R2010, R2013 and R2018
 - additional read-only support for DXF versions R13/R14 (upgraded to R2000)
 - additional read-only support for older DXF versions than R12 (upgraded to R12)
 - read/write support for ASCII DXF and Binary DXF
 - retains third-party DXF content
 - optional C-extensions for CPython are included in the binary wheels, available 
   on [PyPI](https://pypi.org/project/ezdxf/) for Windows, Linux and macOS
+- command line script `ezdxf` to display, convert and inspect DXF files
 
 Included Extensions
 -------------------
 
 Additional packages required for these add-ons are not automatically installed 
 during the *basic* setup, for more information about the setup & dependencies 
 visit the [documentation](https://ezdxf.mozman.at/docs/setup.html).
@@ -124,14 +125,48 @@
 drawing add-on:
 
     pip install ezdxf[draw]
 
 For more information about the setup & dependencies visit the 
 [documentation](https://ezdxf.mozman.at/docs/setup.html).
 
+Command Line
+------------
+
+Use `python -m ezdxf ...` if your shell can't find the `ezdxf` script.
+
+Get additional help for a sub-command:
+
+    ezdxf <cmd> -h
+
+Preview DXF files in a graphical window:
+
+    ezdxf view <file.dxf>
+
+Export the modelspace of DXF files as PNG|SVG|PDF:
+
+    ezdxf draw -o file.<png|svg|pdf> <file.dxf>
+
+Print basic information about DXF files:
+
+    ezdxf info <file.dxf>
+
+Show detailed information and structures of DXF files:
+
+    ezdxf browse <file.dxf>
+
+Audit DXF files:
+
+    ezdxf audit <file.dxf>
+
+Preview and convert HPGL/2 plot files:
+
+    ezdxf hpgl <file.plt>
+
+
 Website
 -------
 
 https://ezdxf.mozman.at/
 
 Documentation
 -------------
```

## Comparing `ezdxf-1.1.0b4/setup.py` & `ezdxf-1.1.0b5/setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_config_file.py` & `ezdxf-1.1.0b5/integration_tests/check_disable_c_ext_by_config_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_env_var.py` & `ezdxf-1.1.0b5/integration_tests/check_disable_c_ext_by_env_var.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_acad_table.py` & `ezdxf-1.1.0b5/integration_tests/test_acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_all_dimline_styles.py` & `ezdxf-1.1.0b5/integration_tests/test_all_dimline_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_all_ellipse_transformations.py` & `ezdxf-1.1.0b5/integration_tests/test_all_ellipse_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_anonymous_blocks.py` & `ezdxf-1.1.0b5/integration_tests/test_anonymous_blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_audit_critical_dxf_files.py` & `ezdxf-1.1.0b5/integration_tests/test_audit_critical_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_audit_layouts.py` & `ezdxf-1.1.0b5/integration_tests/test_audit_layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_complex_line_type_2.py` & `ezdxf-1.1.0b5/integration_tests/test_complex_line_type_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_create_basic_graphics.py` & `ezdxf-1.1.0b5/integration_tests/test_create_basic_graphics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_document_guid.py` & `ezdxf-1.1.0b5/integration_tests/test_document_guid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_document_page_setup.py` & `ezdxf-1.1.0b5/integration_tests/test_document_page_setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_dxf_info_scanning.py` & `ezdxf-1.1.0b5/integration_tests/test_dxf_info_scanning.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_entities_iterator.py` & `ezdxf-1.1.0b5/integration_tests/test_entities_iterator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_fix_dulicate_handles.py` & `ezdxf-1.1.0b5/integration_tests/test_fix_dulicate_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_geo.py` & `ezdxf-1.1.0b5/integration_tests/test_geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_groups.py` & `ezdxf-1.1.0b5/integration_tests/test_groups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_hpgl2_addon.py` & `ezdxf-1.1.0b5/integration_tests/test_hpgl2_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_ignore_junk_beyond_EOF.py` & `ezdxf-1.1.0b5/integration_tests/test_ignore_junk_beyond_EOF.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_launcher.py` & `ezdxf-1.1.0b5/integration_tests/test_launcher.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_leica_disto_r12.py` & `ezdxf-1.1.0b5/integration_tests/test_leica_disto_r12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_load_dxf_unicode_notation.py` & `ezdxf-1.1.0b5/integration_tests/test_load_dxf_unicode_notation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_mapbox_earcut.py` & `ezdxf-1.1.0b5/integration_tests/test_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_mtext_columns.py` & `ezdxf-1.1.0b5/integration_tests/test_mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_mtext_explode_addon.py` & `ezdxf-1.1.0b5/integration_tests/test_mtext_explode_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_mtext_text_frame.py` & `ezdxf-1.1.0b5/integration_tests/test_mtext_text_frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_new_table_entries.py` & `ezdxf-1.1.0b5/integration_tests/test_new_table_entries.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_none_ascii_read_write.py` & `ezdxf-1.1.0b5/integration_tests/test_none_ascii_read_write.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_odafc.py` & `ezdxf-1.1.0b5/integration_tests/test_odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_open_binary_DXF_files.py` & `ezdxf-1.1.0b5/integration_tests/test_open_binary_DXF_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_open_coord_order_issue.py` & `ezdxf-1.1.0b5/integration_tests/test_open_coord_order_issue.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_open_exotic_dxf_files.py` & `ezdxf-1.1.0b5/integration_tests/test_open_exotic_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_open_R13_R14.py` & `ezdxf-1.1.0b5/integration_tests/test_open_R13_R14.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_polyline_entity.py` & `ezdxf-1.1.0b5/integration_tests/test_polyline_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_preserve_binary_data_in_xrecords.py` & `ezdxf-1.1.0b5/integration_tests/test_preserve_binary_data_in_xrecords.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_r12export.py` & `ezdxf-1.1.0b5/integration_tests/test_r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_r12strict.py` & `ezdxf-1.1.0b5/integration_tests/test_r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_r12writer.py` & `ezdxf-1.1.0b5/integration_tests/test_r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_read_file_without_handles.py` & `ezdxf-1.1.0b5/integration_tests/test_read_file_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_read_write_modern_entites.py` & `ezdxf-1.1.0b5/integration_tests/test_read_write_modern_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_recover.py` & `ezdxf-1.1.0b5/integration_tests/test_recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_redraw_order.py` & `ezdxf-1.1.0b5/integration_tests/test_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_rotated_block_attributes.py` & `ezdxf-1.1.0b5/integration_tests/test_rotated_block_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_surface_entities.py` & `ezdxf-1.1.0b5/integration_tests/test_surface_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_write_fixed_meta_data.py` & `ezdxf-1.1.0b5/integration_tests/test_write_fixed_meta_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_write_without_handles.py` & `ezdxf-1.1.0b5/integration_tests/test_write_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/test_xref_detach.py` & `ezdxf-1.1.0b5/integration_tests/test_xref_detach.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/AC1003_LINE_Example.dxf` & `ezdxf-1.1.0b5/integration_tests/data/AC1003_LINE_Example.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/acad_table_with_blk_ref.dxf` & `ezdxf-1.1.0b5/integration_tests/data/acad_table_with_blk_ref.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/ASCII_R12.dxf` & `ezdxf-1.1.0b5/integration_tests/data/ASCII_R12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r12.dxf` & `ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r13.dxf` & `ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r14.dxf` & `ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r2000.dxf` & `ezdxf-1.1.0b5/integration_tests/data/bin_dxf_r2000.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/cc_dxflib.dxf` & `ezdxf-1.1.0b5/integration_tests/data/cc_dxflib.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/custom_blocks.dxf` & `ezdxf-1.1.0b5/integration_tests/data/custom_blocks.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/duplicate_handles.dxf` & `ezdxf-1.1.0b5/integration_tests/data/duplicate_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/dxf_unicode.dxf` & `ezdxf-1.1.0b5/integration_tests/data/dxf_unicode.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/empty_handles.dxf` & `ezdxf-1.1.0b5/integration_tests/data/empty_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/groups.dxf` & `ezdxf-1.1.0b5/integration_tests/data/groups.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/Leica_Disto_S910.dxf` & `ezdxf-1.1.0b5/integration_tests/data/Leica_Disto_S910.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/MODEL.dxf` & `ezdxf-1.1.0b5/integration_tests/data/MODEL.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2007.dxf` & `ezdxf-1.1.0b5/integration_tests/data/mtext_columns_R2007.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2018.dxf` & `ezdxf-1.1.0b5/integration_tests/data/mtext_columns_R2018.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/mtext_framed_columns.dxf` & `ezdxf-1.1.0b5/integration_tests/data/mtext_framed_columns.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/mtext_text_frame.dxf` & `ezdxf-1.1.0b5/integration_tests/data/mtext_text_frame.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/no_layouts.dxf` & `ezdxf-1.1.0b5/integration_tests/data/no_layouts.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/PLOTFILE.plt` & `ezdxf-1.1.0b5/integration_tests/data/PLOTFILE.plt`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/POLI-ALL210_12.DXF` & `ezdxf-1.1.0b5/integration_tests/data/POLI-ALL210_12.DXF`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/recover01.dxf` & `ezdxf-1.1.0b5/integration_tests/data/recover01.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/recover02.dxf` & `ezdxf-1.1.0b5/integration_tests/data/recover02.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/small_r13.dxf` & `ezdxf-1.1.0b5/integration_tests/data/small_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/small_r14.dxf` & `ezdxf-1.1.0b5/integration_tests/data/small_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/XRECORD_0.bin` & `ezdxf-1.1.0b5/integration_tests/data/XRECORD_0.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/XRECORD_1.bin` & `ezdxf-1.1.0b5/integration_tests/data/XRECORD_1.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/integration_tests/data/XRECORD_2.bin` & `ezdxf-1.1.0b5/integration_tests/data/XRECORD_2.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/appsettings.py` & `ezdxf-1.1.0b5/src/ezdxf/appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/audit.py` & `ezdxf-1.1.0b5/src/ezdxf/audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     CREATED_MISSING_OBJECT = 112
     RESET_MLINE_STYLE = 113
     INVALID_GROUP_ENTITIES = 114
     UNDEFINED_BLOCK_NAME = 115
     INVALID_INTEGER_VALUE = 116
     INVALID_FLOATING_POINT_VALUE = 117
     MISSING_PERSISTENT_REACTOR = 118
+    BLOCK_NAME_MISMATCH = 119
 
     # DXF entity property errors:
     INVALID_ENTITY_HANDLE = 201
     INVALID_OWNER_HANDLE = 202
     INVALID_LAYER_NAME = 203
     INVALID_COLOR_INDEX = 204
     INVALID_LINEWEIGHT = 205
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/bbox.py` & `ezdxf-1.1.0b5/src/ezdxf/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/blkrefs.py` & `ezdxf-1.1.0b5/src/ezdxf/blkrefs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/colors.py` & `ezdxf-1.1.0b5/src/ezdxf/colors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/commands.py` & `ezdxf-1.1.0b5/src/ezdxf/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/comments.py` & `ezdxf-1.1.0b5/src/ezdxf/comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/disassemble.py` & `ezdxf-1.1.0b5/src/ezdxf/disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/document.py` & `ezdxf-1.1.0b5/src/ezdxf/document.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/dwginfo.py` & `ezdxf-1.1.0b5/src/ezdxf/dwginfo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entitydb.py` & `ezdxf-1.1.0b5/src/ezdxf/entitydb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/enums.py` & `ezdxf-1.1.0b5/src/ezdxf/enums.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/explode.py` & `ezdxf-1.1.0b5/src/ezdxf/explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/eztypes.py` & `ezdxf-1.1.0b5/src/ezdxf/eztypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/filemanagement.py` & `ezdxf-1.1.0b5/src/ezdxf/filemanagement.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/gfxattribs.py` & `ezdxf-1.1.0b5/src/ezdxf/gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/graphicsfactory.py` & `ezdxf-1.1.0b5/src/ezdxf/graphicsfactory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/groupby.py` & `ezdxf-1.1.0b5/src/ezdxf/groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/npshapes.py` & `ezdxf-1.1.0b5/src/ezdxf/npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/protocols.py` & `ezdxf-1.1.0b5/src/ezdxf/protocols.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/proxygraphic.py` & `ezdxf-1.1.0b5/src/ezdxf/proxygraphic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# Copyright (c) 2020-2022, Manfred Moitzi
+# Copyright (c) 2020-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
     Optional,
     Iterable,
     Iterator,
     cast,
     Sequence,
     Any,
 )
 import sys
 import struct
 import math
-import os
 from enum import IntEnum
 from itertools import repeat
 from ezdxf.lldxf import const
 from ezdxf.tools.binarydata import bytes_to_hexstr, ByteStream, BitStream
 from ezdxf import colors
 from ezdxf.math import (
     Vec3,
@@ -360,16 +359,22 @@
             index = struct.unpack("<L", data)[0]
             if index < len(self.layers):
                 self.layer = self.layers[index]
 
     def attribute_linetype(self, data: bytes):
         if self._doc:
             index = struct.unpack("<L", data)[0]
-            if index < len(self.linetypes):
-                self.linetype = self.linetypes[index]
+            try:
+                # first two entries ByLayer and ByBlock are not included in CAD applications:
+                self.linetype = self.linetypes[index + 2]
+            except IndexError:
+                if index == 32766:
+                    self.linetype = "BYBLOCK"
+                else:  # index is 32767 or invalid
+                    self.linetype = "BYLAYER"
 
     def attribute_marker(self, data: bytes):
         self.marker_index = struct.unpack("<L", data)[0]
 
     def attribute_fill(self, data: bytes):
         self.fill = bool(struct.unpack("<L", data)[0])
 
@@ -494,47 +499,49 @@
         hatch = cast("Hatch", self._factory("HATCH", dxfattribs=attribs))
         elevation = _get_elevation(vertices)
         hatch.paths.add_polyline_path(Vec2.generate(vertices), is_closed=True)
         if elevation:
             hatch.dxf.elevation = Vec3(0, 0, elevation)
         return hatch
 
-    def _polyline(self, vertices, *, close=False, normal=Z_AXIS):
+    def _polyline(self, vertices: list[Vec3], *, close=False, normal=Z_AXIS):
         # Polyline without bulge values!
         # Current implementation ignores the normal vector!
+        # Polyline ignores the filled flag, see #906
         attribs = self._build_dxf_attribs()
         count = len(vertices)
         if count == 1 or (count == 2 and vertices[0].isclose(vertices[1])):
             attribs["location"] = vertices[0]
             return self._factory("POINT", dxfattribs=attribs)
-
-        if self.fill and count > 2:
-            polyline = self._filled_polygon(vertices, attribs)
-        else:
+        if not is_2d_polyline(vertices):
             attribs["flags"] = const.POLYLINE_3D_POLYLINE
-            polyline = cast("Polyline", self._factory("POLYLINE", dxfattribs=attribs))
-            polyline.append_vertices(vertices)
-            if close:
-                polyline.close()
-            polyline.new_seqend()
+        polyline = cast("Polyline", self._factory("POLYLINE", dxfattribs=attribs))
+        polyline.append_vertices(vertices)
+        if close:
+            polyline.close()
+        polyline.new_seqend()
         return polyline
 
     def polyline_with_normals(self, data: bytes):
         # Polyline without bulge values!
+        # Polyline ignores the filled flag, see #906
         vertices, normal = self._load_vertices(data, load_normal=True)
         return self._polyline(vertices, normal=normal)
 
     def polyline(self, data: bytes):
         # Polyline without bulge values!
+        # Polyline ignores the filled flag, see #906
         vertices, normal = self._load_vertices(data, load_normal=False)
         return self._polyline(vertices)
 
     def polygon(self, data: bytes):
         # Polyline without bulge values!
         vertices, normal = self._load_vertices(data, load_normal=False)
+        if self.fill:
+            return self._filled_polygon(vertices, self._build_dxf_attribs())
         return self._polyline(vertices, close=True)
 
     def lwpolyline(self, data: bytes):
         # OpenDesign Specs LWPLINE: 20.4.85 Page 211
         attribs = self._build_dxf_attribs()
         num_bulges = 0
         num_vertex_ids = 0
@@ -790,15 +797,16 @@
             if self._doc and not self._doc.styles.has_entry(style):
                 self._doc.styles.new(
                     font, dxfattribs={"font": font, "bigfont": bigfont}
                 )
                 self.textstyles[font] = style
         return style
 
-    def _load_vertices(self, data: bytes, load_normal=False):
+    @staticmethod
+    def _load_vertices(data: bytes, load_normal=False) -> tuple[list[Vec3], bool]:
         normal = Z_AXIS
         bs = ByteStream(data)
         count = bs.read_long()
         if load_normal:
             count += 1
         vertices: list[Vec3] = []
         while count > 0:
@@ -917,7 +925,14 @@
                 return
 
 
 def _get_elevation(vertices) -> float:
     if vertices:
         return vertices[0].z
     return 0.0
+
+
+def is_2d_polyline(vertices: list[Vec3]) -> bool:
+    if len(vertices) < 1:
+        return True
+    z = vertices[0].z
+    return all(math.isclose(z, v.z) for v in vertices)
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/query.py` & `ezdxf-1.1.0b5/src/ezdxf/query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/queryparser.py` & `ezdxf-1.1.0b5/src/ezdxf/queryparser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/r12strict.py` & `ezdxf-1.1.0b5/src/ezdxf/r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/recover.py` & `ezdxf-1.1.0b5/src/ezdxf/recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/reorder.py` & `ezdxf-1.1.0b5/src/ezdxf/reorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/transform.py` & `ezdxf-1.1.0b5/src/ezdxf/transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/units.py` & `ezdxf-1.1.0b5/src/ezdxf/units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/upright.py` & `ezdxf-1.1.0b5/src/ezdxf/upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/urecord.py` & `ezdxf-1.1.0b5/src/ezdxf/urecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/version.py` & `ezdxf-1.1.0b5/src/ezdxf/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # examples:
 #   major pre-release alpha 2: VERSION = "0.9.0a2"; version = (0, 9, 0, 'a2')
 #   major release candidate 0: VERSION = "0.9.0rc0"; version = (0, 9, 0, 'rc0')
 #   major release: VERSION = "0.9.0"; version = (0, 9, 0, 'release')
 #   1. bug fix release beta0: VERSION = "0.9.1b0"; version = (0, 9, 1, 'b0')
 #   2. bug fix release: VERSION = "0.9.2"; version = (0, 9, 2, 'release')
 
-version = (1, 1, 0, "b4")
-__version__ = "1.1.0b4"
+version = (1, 1, 0, "b5")
+__version__ = "1.1.0b5"
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/xref.py` & `ezdxf-1.1.0b5/src/ezdxf/xref.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,23 +100,33 @@
 
 
 class InternalError(XrefError):
     pass
 
 
 class ConflictPolicy(enum.Enum):
-    # What to do when a name conflict of existing and loaded resources occur:
-    # keep existing resource <name> and ignore loaded resource
-    KEEP = enum.auto()
+    """These conflict policies define how to handle resource name conflicts.
 
-    # ALWAYS rename imported resources to <xref>$0$<name>
-    # This is the default behavior of BricsCAD when binding an external reference.
-    XREF_PREFIX = enum.auto()
+    .. versionadded:: 1.1
+
+    Attributes:
+        KEEP: Keeps the existing resource name of the target document and ignore the
+            resource from the source document.
+        XREF_PREFIX: This policy handles the resource import like CAD applications by
+            **always** renaming the loaded resources to `<xref>$0$<name>`, where `xref`
+            is the name of source document, the `$0$` part is a number to create a
+            unique resource name and `<name>` is the name of the resource itself.
+        NUM_PREFIX: This policy renames the loaded resources to `$0$<name>` only if the
+            resource `<name>` already exists. The `$0$` prefix is a number to create a
+            unique resource name and `<name>` is the name of the resource itself.
 
-    # rename loaded resource to $0$<name> if the loaded resource <name> already exist
+    """
+
+    KEEP = enum.auto()
+    XREF_PREFIX = enum.auto()
     NUM_PREFIX = enum.auto()
 
 
 def dxf_info(filename: str | os.PathLike) -> DXFInfo:
     """Scans the HEADER section of a DXF document and returns a :class:`DXFInfo`
     object, which contains information about the DXF version, text encoding, drawing
     units and insertion base point.
@@ -249,15 +259,15 @@
     insert: UVec = (0, 0, 0),
     scale: float = 1.0,
     rotation: float = 0.0,
     overlay=False,
 ) -> Insert:
     """Attach the file `filename` to the host document as external reference (XREF) and
     creates a default block reference for the XREF in the modelspace of the document.
-    The function raises a :class:`ValueError` exception if the block definition
+    The function raises an :class:`XrefDefinitionError` exception if the block definition
     already exist, but an XREF can be inserted multiple times by adding additional block
     references::
 
         msp.add_blockref(block_name, insert=another_location)
 
     .. important::
 
@@ -303,14 +313,16 @@
 def find_xref(xref_filename: str, search_paths: Sequence[pathlib.Path]) -> pathlib.Path:
     """Returns the path of the XREF file.
 
     Args:
         xref_filename: filename of the XREF, absolute or relative path
         search_paths: search paths where to look for the XREF file
 
+    .. versionadded:: 1.1
+
     """
     filepath = pathlib.Path(xref_filename)
     # 1. check absolute xref_filename
     if filepath.exists():
         return filepath
 
     name = filepath.name
@@ -415,14 +427,18 @@
         xref_doc = xref.detach(my_block, "my_block.dwg")
         odafc.export_dwg(xref_doc, "my_block.dwg")
 
     It's recommended to clean up the entity database of the host document afterwards::
 
         doc.entitydb.purge()
 
+    The function does not create any block references. These references should already
+    exist and do not need to be changed since references to blocks and XREFs are the
+    same.
+
     Args:
         block: block definition to detach
         xref_filename: name of the external referenced file
         overlay: creates an XREF overlay if ``True`` and an XREF attachment otherwise
 
     .. versionadded:: 1.1
 
@@ -499,14 +515,16 @@
 
     Args:
         sdoc: source document
         tdoc: target document
         filter_fn: optional function to filter entities from the source modelspace
         conflict_policy: how to resolve name conflicts
 
+    .. versionadded:: 1.1
+
     """
     loader = Loader(sdoc, tdoc, conflict_policy=conflict_policy)
     loader.load_modelspace(filter_fn=filter_fn)
     loader.execute()
 
 
 def load_paperspace(
@@ -521,14 +539,16 @@
 
     Args:
         psp: paperspace layout to load
         tdoc: target document
         filter_fn: optional function to filter entities from the source paperspace layout
         conflict_policy: how to resolve name conflicts
 
+    .. versionadded:: 1.1
+
     """
     if psp.doc is tdoc:
         raise LayoutError("Source paperspace layout cannot be from target document.")
     loader = Loader(psp.doc, tdoc, conflict_policy=conflict_policy)
     loader.load_paperspace_layout(psp, filter_fn=filter_fn)
     loader.execute()
 
@@ -624,15 +644,18 @@
         for e in self.entities:
             registry.add_entity(e, block_key=e.dxf.owner)
 
     def execute(self, transfer: _Transfer) -> None:
         target_layout = self.target_layout
         for entity in self.entities:
             clone = transfer.get_entity_copy(entity)
-            if clone and is_graphic_entity(clone):
+            if clone is None:
+                transfer.debug(f"xref:cannot copy {str(entity)}")
+                continue
+            if is_graphic_entity(clone):
                 target_layout.add_entity(clone)  # type: ignore
             else:
                 transfer.debug(
                     f"found non-graphic entity {str(clone)} as layout content"
                 )
         if isinstance(target_layout, Paperspace):
             _reorganize_paperspace_viewports(target_layout)
@@ -913,24 +936,22 @@
             cmd.register_resources(registry)
 
         if debug:
             _log_debug_messages(registry.debug_messages)
 
         cpm = CopyMachine(self.tdoc)
 
-        if debug:
-            _log_debug_messages(cpm.debug_messages)
-
         cpm.copy_blocks(registry.source_blocks)
         transfer = _Transfer(
             registry=registry,
             copies=cpm.copies,
             objects=cpm.objects,
             handle_mapping=cpm.handle_mapping,
             conflict_policy=self.conflict_policy,
+            copy_errors=cpm.copy_errors,
         )
         if xref_prefix:
             transfer.xref_prefix = str(xref_prefix)
         transfer.add_object_copies(cpm.objects)
         transfer.register_classes(cpm.classes)
         transfer.register_table_resources()
         transfer.register_object_resources()
@@ -1061,19 +1082,21 @@
         self,
         registry: _Registry,
         copies: dict[str, dict[str, DXFEntity]],
         objects: dict[str, DXFEntity],
         handle_mapping: dict[str, str],
         *,
         conflict_policy=ConflictPolicy.KEEP,
+        copy_errors: set[str],
     ) -> None:
         self.registry = registry
         # entry NO_BLOCK (layout key "0") contains table entries
         self.copied_blocks = copies
         self.copied_objects = objects
+        self.copy_errors = copy_errors
         self.conflict_policy = conflict_policy
         self.xref_prefix = get_xref_name(registry.source_doc)
         self.layer_mapping: dict[str, str] = {}
         self.linetype_mapping: dict[str, str] = {}
         self.text_style_mapping: dict[str, str] = {}
         self.dim_style_mapping: dict[str, str] = {}
         self.block_name_mapping: dict[str, str] = {}
@@ -1116,14 +1139,16 @@
             pass
         return None
 
     def map_resources_of_copy(self, entity: DXFEntity) -> None:
         clone = self.get_entity_copy(entity)
         if clone:
             entity.map_resources(clone, self)
+        elif entity.dxf.handle in self.copy_errors:
+            pass
         else:
             raise InternalError(f"copy of {entity} not found")
 
     def map_pointers(self, tags: Tags, new_owner_handle: str = "") -> None:
         for index, tag in enumerate(tags):
             if types.is_translatable_pointer(tag):
                 handle = self.get_handle(tag.value, default="0")
@@ -1516,14 +1541,16 @@
         tdoc.objects.set_wipeout_variables(
             frame=sdoc.objects.get_wipeout_frame_setting()
         )
 
     def finalize(self) -> None:
         # remove replaced entities:
         self.registry.target_doc.entitydb.purge()
+        for msg in self.debug_messages:
+            logger.log(logging.INFO, msg)
 
 
 def get_xref_name(doc: Drawing) -> str:
     if doc.filename:
         return pathlib.Path(doc.filename).stem
     return ""
 
@@ -1552,21 +1579,18 @@
 
 class CopyMachine:
     def __init__(self, tdoc: Drawing) -> None:
         self.target_doc = tdoc
         self.copies: dict[str, dict[str, DXFEntity]] = {}
         self.classes: list[DXFClass] = []
         self.objects: dict[str, DXFEntity] = {}
+        self.copy_errors: set[str] = set()
 
         # mapping from the source entity handle to the handle of the copied entity
         self.handle_mapping: dict[str, str] = {}
-        self.debug_messages: list[str] = []
-
-    def debug(self, msg: str) -> None:
-        self.debug_messages.append(msg)
 
     def copy_blocks(self, blocks: dict[str, dict[str, DXFEntity]]) -> None:
         for handle, block in blocks.items():
             self.copies[handle] = self.copy_block(block)
 
     def copy_block(self, block: dict[str, DXFEntity]) -> dict[str, DXFEntity]:
         copies: dict[str, DXFEntity] = {}
@@ -1592,12 +1616,12 @@
                 copies[handle] = clone
         return copies
 
     def copy_entity(self, entity: DXFEntity) -> Optional[DXFEntity]:
         try:
             return entity.copy_external()
         except const.DXFError:
-            self.debug(f"cannot copy entity {str(entity)}")
+            self.copy_errors.add(entity.dxf.handle)
         return None
 
     def copy_dxf_class(self, cls: DXFClass) -> None:
         self.classes.append(cls.copy())
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/zoom.py` & `ezdxf-1.1.0b5/src/ezdxf/zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/_options.py` & `ezdxf-1.1.0b5/src/ezdxf/_options.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/__init__.py` & `ezdxf-1.1.0b5/src/ezdxf/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/__main__.py` & `ezdxf-1.1.0b5/src/ezdxf/__main__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/bezier3p.pyx` & `ezdxf-1.1.0b5/src/ezdxf/acc/bezier3p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/bezier4p.pyx` & `ezdxf-1.1.0b5/src/ezdxf/acc/bezier4p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/bspline.pyx` & `ezdxf-1.1.0b5/src/ezdxf/acc/bspline.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/construct.pyx` & `ezdxf-1.1.0b5/src/ezdxf/acc/construct.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/linetypes.pyx` & `ezdxf-1.1.0b5/src/ezdxf/acc/linetypes.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/mapbox_earcut.pyx` & `ezdxf-1.1.0b5/src/ezdxf/acc/mapbox_earcut.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/matrix44.pyx` & `ezdxf-1.1.0b5/src/ezdxf/acc/matrix44.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/np_support.pyx` & `ezdxf-1.1.0b5/src/ezdxf/acc/np_support.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/vector.pxd` & `ezdxf-1.1.0b5/src/ezdxf/acc/vector.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/vector.pyx` & `ezdxf-1.1.0b5/src/ezdxf/acc/vector.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.cpp` & `ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_cubic_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.hpp` & `ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_cubic_bezier.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.cpp` & `ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_quad_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.hpp` & `ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_vec3.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.pxd` & `ezdxf-1.1.0b5/src/ezdxf/acc/_cpp_vec3.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acc/__init__.py` & `ezdxf-1.1.0b5/src/ezdxf/acc/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acis/abstract.py` & `ezdxf-1.1.0b5/src/ezdxf/acis/abstract.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acis/api.py` & `ezdxf-1.1.0b5/src/ezdxf/acis/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acis/const.py` & `ezdxf-1.1.0b5/src/ezdxf/acis/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acis/dbg.py` & `ezdxf-1.1.0b5/src/ezdxf/acis/dbg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acis/dxf.py` & `ezdxf-1.1.0b5/src/ezdxf/acis/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acis/entities.py` & `ezdxf-1.1.0b5/src/ezdxf/acis/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acis/hdr.py` & `ezdxf-1.1.0b5/src/ezdxf/acis/hdr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acis/mesh.py` & `ezdxf-1.1.0b5/src/ezdxf/acis/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acis/sab.py` & `ezdxf-1.1.0b5/src/ezdxf/acis/sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/acis/sat.py` & `ezdxf-1.1.0b5/src/ezdxf/acis/sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/acadctb.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/binpacking.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/binpacking.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/dimlines.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/dimlines.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/dxf2code.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/dxf2code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/genetic_algorithm.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/geo.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/gerber_D6673.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/gerber_D6673.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/importer.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/iterdxf.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/iterdxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/menger_sponge.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/meshex.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/mtextsurrogate.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/mtextsurrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/mtxpl.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/mtxpl.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/odafc.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/openscad.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/pycsg.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/r12export.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/r12export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 """
 Module to export any DXF document as DXF version R12 without modifying the source
 document.
 
----------------------------------------------------------
-WARNING: THIS MODULE IS IN PLANNING STATE, DO NOT USE IT!
----------------------------------------------------------
-
 .. versionadded:: 1.1
 
 To get the best result use the ODA File Converter add-on::
 
     from ezdxf.addons import odafc
 
     odafc.convert("any.dxf", "r12.dxf", version="R12")
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/r12writer.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/sierpinski_pyramid.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/sierpinski_pyramid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/tablepainter.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/tablepainter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/text2path.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/xplayer.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/xplayer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/xqt.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/xqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/browser.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/acisbrowser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/data.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/acisbrowser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/browser/bookmarks.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/browser/bookmarks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/browser/browser.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/browser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/browser/data.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/browser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/browser/find_dialog.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/browser/find_dialog.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/browser/loader.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/browser/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/browser/model.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/browser/model.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/browser/tags.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/browser/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/browser/views.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/browser/views.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/backend.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/clipper.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/clipper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/config.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/config.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_backend.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/debug_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_utils.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/debug_utils.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/designer.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/designer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/dxf.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/frontend.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/frontend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/gfxproxy.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/gfxproxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/hpgl2.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/layout.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/matplotlib.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/matplotlib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/mtext_complex.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/mtext_complex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/properties.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pymupdf.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/pymupdf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pyqt.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/pyqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/qtviewer.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/qtviewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/recorder.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/recorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/svg.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/svg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text_renderer.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/unified_text_renderer.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/drawing/unified_text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/classes_section.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/dwg/classes_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/const.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/dwg/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/crc.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/dwg/crc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/fileheader.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/dwg/fileheader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/header_section.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/dwg/header_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/loader.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/dwg/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/api.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/backend.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/deps.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/deps.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/interpreter.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/interpreter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/page.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/page.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/plotter.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/plotter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/polygon_buffer.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/polygon_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/properties.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/tokenizer.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/tokenizer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/viewer.py` & `ezdxf-1.1.0b5/src/ezdxf/addons/hpgl2/viewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/acad_proxy_entity.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/acad_proxy_entity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #  Copyright (c) 2021-2022, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, Iterator
 from ezdxf.lldxf import const
 from ezdxf.lldxf.tags import Tags
+from ezdxf.query import EntityQuery
 from .dxfentity import SubclassProcessor
 from .dxfgfx import DXFGraphic
 from . import factory
 
 if TYPE_CHECKING:
     from ezdxf.lldxf.tagwriter import AbstractTagWriter
     from ezdxf.entities import DXFNamespace
+    from ezdxf.layouts import BaseLayout
 
 
 # Group Codes of AcDbProxyEntity
 # https://help.autodesk.com/view/OARX/2018/ENU/?guid=GUID-89A690F9-E859-4D57-89EA-750F3FB76C6B
 # 100 AcDbProxyEntity
 # 90  Proxy entity class ID (always 498)
 # 91  Application entity's class ID. Class IDs are based on the order of
@@ -89,25 +91,49 @@
         # XDATA export is done by the parent class
 
     def __virtual_entities__(self) -> Iterator[DXFGraphic]:
         """Implements the SupportsVirtualEntities protocol."""
         from ezdxf.proxygraphic import ProxyGraphic
 
         if self.proxy_graphic:
-            for e in ProxyGraphic(
-                self.proxy_graphic, self.doc
-            ).virtual_entities():
+            for e in ProxyGraphic(self.proxy_graphic, doc=self.doc).virtual_entities():
                 e.set_source_of_copy(self)
                 yield e
         return []
 
     def virtual_entities(self) -> Iterator[DXFGraphic]:
         """Yields proxy graphic as "virtual" entities."""
         return self.__virtual_entities__()
 
+    def explode(self, target_layout: Optional[BaseLayout] = None) -> EntityQuery:
+        """Explodes the proxy graphic for the ACAD_PROXY_ENTITY into the target layout,
+        if target layout is ``None``, the layout of the ACAD_PROXY_ENTITY will be used.
+        This method destroys the source ACAD_PROXY_ENTITY entity.
+
+        Args:
+            target_layout: target layout for exploded entities, ``None`` for
+                same layout as the source ACAD_PROXY_ENTITY.
+
+        Returns:
+            :class:`~ezdxf.query.EntityQuery` container referencing all exploded
+            DXF entities.
+
+        """
+        if target_layout is None:
+            target_layout = self.get_layout()
+            if target_layout is None:
+                raise const.DXFStructureError(
+                    "ACAD_PROXY_ENTITY without layout assignment, specify target layout"
+                )
+        entities: list[DXFGraphic] = list(self.__virtual_entities__())
+        for e in entities:
+            target_layout.add_entity(e)
+        self.destroy()
+        return EntityQuery(entities)
+
 
 def load_proxy_data(
     tags: Tags, length_code: int, data_code: int = 310
 ) -> Optional[bytes]:
     try:
         index = tags.tag_index(length_code)
     except const.DXFValueError:
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/acad_table.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/acad_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,61 +20,15 @@
 from .objectcollection import ObjectCollection
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFNamespace
     from ezdxf.lldxf.tagwriter import AbstractTagWriter
     from ezdxf.document import Drawing
 
-__all__ = ["AcadTable", "AcadTableBlockContent"]
-
-
-@factory.register_entity
-class AcadTableBlockContent(DXFTagStorage):
-    DXFTYPE = "ACAD_TABLE"
-
-    def proxy_graphic_content(self) -> Iterable[DXFGraphic]:
-        return super().__virtual_entities__()
-
-    def _block_content(self) -> Iterator[DXFGraphic]:
-        block_name: str = self.get_block_name()
-        return self.doc.blocks.get(block_name, [])  # type: ignore
-
-    def _block_reference_tags(self) -> Tags:
-        try:
-            return self.xtags.get_subclass("AcDbBlockReference")
-        except const.DXFKeyError:
-            return Tags()
-
-    def get_block_name(self) -> str:
-        tags = self._block_reference_tags()
-        return tags.get_first_value(2, "")
-
-    def get_insert_location(self) -> Vec3:
-        return self._block_reference_tags().get_first_value(10, Vec3())
-
-    def __virtual_entities__(self) -> Iterator[DXFGraphic]:
-        """Implements the SupportsVirtualEntities protocol."""
-        insert: Vec3 = Vec3(self.get_insert_location())
-        m: Optional[Matrix44] = None
-        if insert:
-            # TODO: OCS transformation (extrusion) is ignored yet
-            m = Matrix44.translate(insert.x, insert.y, insert.z)
-
-        for entity in self._block_content():
-            try:
-                clone = entity.copy()
-            except const.DXFTypeError:
-                continue
-            if m is not None:
-                # noinspection PyUnboundLocalVariable
-                try:
-                    clone.transform(m)
-                except:  # skip entity at any transformation issue
-                    continue
-            yield clone
+__all__ = ["AcadTable", "AcadTableBlockContent", "acad_table_to_block"]
 
 
 acdb_block_reference = DefSubclass(
     "AcDbBlockReference",
     {
         # Block name: an anonymous block begins with a *T value
         "geometry": DXFAttr(2),
@@ -381,10 +335,91 @@
     DXFTYPE = "TABLESTYLE"
     DXFATTRIBS = DXFAttributes(base_class, acdb_table_style)
     MIN_DXF_VERSION_FOR_EXPORT = const.DXF2007
 
 
 class TableStyleManager(ObjectCollection[TableStyle]):
     def __init__(self, doc: Drawing):
-        super().__init__(
-            doc, dict_name="ACAD_TABLESTYLE", object_type="TABLESTYLE"
-        )
+        super().__init__(doc, dict_name="ACAD_TABLESTYLE", object_type="TABLESTYLE")
+
+
+@factory.register_entity
+class AcadTableBlockContent(DXFTagStorage):
+    DXFTYPE = "ACAD_TABLE"
+    DXFATTRIBS = DXFAttributes(
+        base_class, acdb_entity, acdb_block_reference, acdb_table
+    )
+
+    def load_dxf_attribs(
+        self, processor: Optional[SubclassProcessor] = None
+    ) -> DXFNamespace:
+        dxf = super().load_dxf_attribs(processor)
+        if processor:
+            processor.fast_load_dxfattribs(
+                dxf, acdb_block_reference_group_codes, subclass=2
+            )
+            processor.fast_load_dxfattribs(
+                dxf, acdb_table_group_codes, subclass=3, log=False
+            )
+        return dxf
+
+    def proxy_graphic_content(self) -> Iterable[DXFGraphic]:
+        return super().__virtual_entities__()
+
+    def _block_content(self) -> Iterator[DXFGraphic]:
+        block_name: str = self.get_block_name()
+        return self.doc.blocks.get(block_name, [])  # type: ignore
+
+    def get_block_name(self) -> str:
+        return self.dxf.get("geometry", "")
+
+    def get_insert_location(self) -> Vec3:
+        return self.dxf.get("insert", Vec3())
+
+    def __virtual_entities__(self) -> Iterator[DXFGraphic]:
+        """Implements the SupportsVirtualEntities protocol."""
+        insert: Vec3 = Vec3(self.get_insert_location())
+        m: Optional[Matrix44] = None
+        if insert:
+            # TODO: OCS transformation (extrusion) is ignored yet
+            m = Matrix44.translate(insert.x, insert.y, insert.z)
+
+        for entity in self._block_content():
+            try:
+                clone = entity.copy()
+            except const.DXFTypeError:
+                continue
+            if m is not None:
+                # noinspection PyUnboundLocalVariable
+                try:
+                    clone.transform(m)
+                except:  # skip entity at any transformation issue
+                    continue
+            yield clone
+
+
+def acad_table_to_block(table: DXFEntity) -> None:
+    """Converts the given ACAD_TABLE entity to a block references (INSERT entity).
+
+    The original ACAD_TABLE entity will be destroyed.
+
+    .. versionadded:: 1.1
+
+    """
+    if not isinstance(table, AcadTableBlockContent):
+        return
+    doc = table.doc
+    owner = table.dxf.owner
+    block_name = table.get_block_name()
+    if doc is None or block_name == "" or owner is None:
+        return
+    try:
+        layout = doc.layouts.get_layout_by_key(owner)
+    except const.DXFKeyError:
+        return
+    # replace ACAD_TABLE entity by INSERT entity
+    layout.add_blockref(
+        block_name,
+        insert=table.get_insert_location(),
+        dxfattribs={"layer": table.dxf.get("layer", "0")},
+    )
+    layout.delete_entity(table)  # type: ignore
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/acis.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/appdata.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/appid.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/appid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/arc.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/attrib.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/attrib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2022 Manfred Moitzi
+# Copyright (c) 2019-2023 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
 import copy
 from ezdxf.lldxf import validator
 from ezdxf.math import NULLVEC, Vec3, Z_AXIS, OCS
 from ezdxf.lldxf.attributes import (
@@ -67,16 +67,21 @@
 #        paper space can not be used as XREF.
 
 # DXF Reference for ATTRIB is a total mess and incorrect, the AcDbText subclass
 # for the ATTRIB entity is the same as for the TEXT entity, but the valign field
 # from the 2nd AcDbText subclass of the TEXT entity is stored in the
 # AcDbAttribute subclass:
 attrib_fields = {
+    # "version": DXFAttr(280, default=0, dxfversion=const.DXF2010),
+    # The "version" tag has the same group code as the lock_position tag!!!!!
     # Version number: 0 = 2010
-    "version": DXFAttr(280, default=0, dxfversion=const.DXF2010),
+    # This tag is not really used (at least by BricsCAD) but there exists DXF files
+    # which do use this tag: "dxftest\attrib\attrib_with_mtext_R2018.dxf"
+    # ezdxf stores the last group code 280 as "lock_position" attribute and does
+    # not export a version tag for any DXF version.
     # Tag string (cannot contain spaces):
     "tag": DXFAttr(
         2,
         default="",
         validator=validator.is_valid_attrib_tag,
         fixer=validator.fix_attrib_tag,
     ),
@@ -96,15 +101,15 @@
         fixer=RETURN_DEFAULT,
     ),
     # Lock position flag. Locks the position of the attribute within the block
     # reference, example of double use of group codes in one sub class
     "lock_position": DXFAttr(
         280,
         default=0,
-        dxfversion=const.DXF2010,
+        dxfversion=const.DXF2007,  # tested with BricsCAD 2023/TrueView 2023
         optional=True,
         validator=validator.is_integer_bool,
         fixer=RETURN_DEFAULT,
     ),
     # Attribute type:
     # 1 = single line
     # 2 = multiline ATTRIB
@@ -445,15 +450,15 @@
 
     def export_acdb_attdef(self, tagwriter: AbstractTagWriter) -> None:
         if tagwriter.dxfversion > const.DXF12:
             tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_attdef.name)
         self.dxf.export_dxf_attribs(
             tagwriter,
             [
-                "version",
+                # write version tag (280, 0) here, if required in the future
                 "prompt",
                 "tag",
                 "flags",
                 "field_length",
                 "valign",
                 "lock_position",
             ],
@@ -519,15 +524,15 @@
 
     def export_acdb_attrib(self, tagwriter: AbstractTagWriter) -> None:
         if tagwriter.dxfversion > const.DXF12:
             tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_attrib.name)
         self.dxf.export_dxf_attribs(
             tagwriter,
             [
-                "version",
+                # write version tag (280, 0) here, if required in the future
                 "tag",
                 "flags",
                 "field_length",
                 "valign",
                 "lock_position",
             ],
         )
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/block.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/block.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,28 @@
     PAPER_SPACE_R12,
     MODEL_SPACE_R2000,
     PAPER_SPACE_R2000,
 )
 from ezdxf.math import NULLVEC
 from .dxfentity import base_class, SubclassProcessor, DXFEntity
 from .factory import register_entity
+from ezdxf.audit import Auditor, AuditError
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFNamespace
     from ezdxf.lldxf.tagwriter import AbstractTagWriter
+    from ezdxf import xref
 
 __all__ = ["Block", "EndBlk"]
 
 acdb_entity = DefSubclass(
     "AcDbEntity",
     {
         # No auto fix for invalid layer names!
-        "layer": DXFAttr(
-            8, default="0", validator=validator.is_valid_layer_name
-        ),
+        "layer": DXFAttr(8, default="0", validator=validator.is_valid_layer_name),
         "paperspace": DXFAttr(
             67,
             default=0,
             optional=True,
             validator=validator.is_integer_bool,
             fixer=RETURN_DEFAULT,
         ),
@@ -160,17 +160,15 @@
 
     @property
     def is_layout_block(self) -> bool:
         """Returns ``True`` if this is a :class:`~ezdxf.layouts.Modelspace` or
         :class:`~ezdxf.layouts.Paperspace` block definition.
         """
         name = self.dxf.name.lower()
-        return name.startswith("*model_space") or name.startswith(
-            "*paper_space"
-        )
+        return name.startswith("*model_space") or name.startswith("*paper_space")
 
     @property
     def is_anonymous(self) -> bool:
         """Returns ``True`` if this is an anonymous block generated by
         hatching, associative dimensioning, other internal operations, or an
         application.
 
@@ -183,14 +181,35 @@
         return self.get_flag_state(Block.XREF)
 
     @property
     def is_xref_overlay(self) -> bool:
         """Returns ``True`` if bock is an external referenced overlay file."""
         return self.get_flag_state(Block.XREF_OVERLAY)
 
+    def audit(self, auditor: Auditor):
+        owner_handle = self.dxf.get("owner")
+        if owner_handle is None:  # invalid owner handle - IGNORE
+            return
+        owner = auditor.entitydb.get(owner_handle)
+        if owner is None:  # invalid owner entity - IGNORE
+            return
+        owner_name = owner.dxf.get("name", "").upper()
+        block_name = self.dxf.get("name", "").upper()
+        if owner_name != block_name:
+            auditor.add_error(
+                AuditError.BLOCK_NAME_MISMATCH,
+                f"{str(self)} name '{block_name}' and {str(owner)} name '{owner_name}' mismatch",
+            )
+
+    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+        """Translate resources from self to the copied entity."""
+        assert isinstance(clone, Block)
+        super().map_resources(clone, mapping)
+        clone.dxf.name = mapping.get_block_name(self.dxf.name)
+
 
 acdb_block_end = DefSubclass("AcDbBlockEnd", {})
 
 
 @register_entity
 class EndBlk(DXFEntity):
     """DXF ENDBLK entity"""
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/blockrecord.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/blockrecord.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Copyright (c) 2019-2022, Manfred Moitzi
+# Copyright (c) 2019-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
 import logging
-from ezdxf.audit import AuditError
+
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     RETURN_DEFAULT,
     group_code_mapping,
@@ -175,30 +175,28 @@
             registry.add_entity(self.endblk, block_key=key)
         else:
             raise DXFInternalEzdxfError(
                 f"ENDBLK entity in BLOCK_RECORD #{key} is invalid"
             )
         for e in self.entity_space:
             registry.add_entity(e, block_key=key)
-        # todo: Modelspace and Paperspace layouts
 
     def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, BlockRecord)
         super().map_resources(clone, mapping)
 
         assert self.block is not None
         mapping.map_resources_of_copy(self.block)
 
         assert self.endblk is not None
         mapping.map_resources_of_copy(self.endblk)
 
         for entity in self.entity_space:
             mapping.map_resources_of_copy(entity)
-        # todo: Modelspace and Paperspace layouts
 
     def destroy(self):
         """Destroy associated data:
 
             - BLOCK
             - ENDBLK
             - all entities stored in this block definition
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/boundary_paths.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/circle.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/dictionary.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/dimension.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/dimstyle.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/dimstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/dimstyleoverride.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/dimstyleoverride.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/dxfclass.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/dxfentity.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/dxfgfx.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/dxfgroups.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/dxfns.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/dxfns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/dxfobj.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/ellipse.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/factory.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/geodata.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/geodata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/gradient.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/gradient.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/hatch.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/hatch.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/helix.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/idbuffer.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/idbuffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/image.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/image.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/insert.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/insert.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,15 +578,15 @@
             DXF entities.
 
         """
         if target_layout is None:
             target_layout = self.get_layout()
             if target_layout is None:
                 raise DXFStructureError(
-                    "INSERT without layout assignment, specify target layout."
+                    "INSERT without layout assignment, specify target layout"
                 )
         return explode_block_reference(
             self, target_layout=target_layout, redraw_order=redraw_order
         )
 
     def __virtual_entities__(self) -> Iterator[DXFGraphic]:
         """Implements the SupportsVirtualEntities protocol.
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/layer.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/layout.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/leader.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/light.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/line.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/ltype.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/lwpolyline.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/lwpolyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/material.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/mesh.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/mleader.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/mline.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/mpolygon.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/mtext.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/mtext_columns.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/objectcollection.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/objectcollection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/oleframe.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/oleframe.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/pattern.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/point.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/polygon.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/polyline.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/shape.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/solid.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/spline.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/subentity.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/subentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/sun.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/table.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/text.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/textstyle.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/textstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/tolerance.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/ucs.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/underlay.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/view.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/view.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/viewport.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/visualstyle.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/visualstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/vport.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/vport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/xdata.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/xdict.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/xdict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/xline.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/entities/__init__.py` & `ezdxf-1.1.0b5/src/ezdxf/entities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 from .mleader import MLeader, MLeaderStyle, MLeaderStyleCollection, MultiLeader
 
 # register graphical entities R2004
 
 # register graphical entities R2007
 
 from .light import Light
-from .acad_table import AcadTableBlockContent
+from .acad_table import AcadTableBlockContent, acad_table_to_block
 
 # register graphical entities R2010
 
 from .geodata import GeoData
 
 # register graphical entities R2013
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf/fonts/fonts.py` & `ezdxf-1.1.0b5/src/ezdxf/fonts/fonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/fonts/font_face.py` & `ezdxf-1.1.0b5/src/ezdxf/fonts/font_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/fonts/font_manager.py` & `ezdxf-1.1.0b5/src/ezdxf/fonts/font_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/fonts/font_measurements.py` & `ezdxf-1.1.0b5/src/ezdxf/fonts/font_measurements.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/fonts/glyphs.py` & `ezdxf-1.1.0b5/src/ezdxf/fonts/glyphs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/fonts/lff.py` & `ezdxf-1.1.0b5/src/ezdxf/fonts/lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/fonts/shapefile.py` & `ezdxf-1.1.0b5/src/ezdxf/fonts/shapefile.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/fonts/ttfonts.py` & `ezdxf-1.1.0b5/src/ezdxf/fonts/ttfonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/layouts/base.py` & `ezdxf-1.1.0b5/src/ezdxf/layouts/base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/layouts/blocklayout.py` & `ezdxf-1.1.0b5/src/ezdxf/layouts/blocklayout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/layouts/layout.py` & `ezdxf-1.1.0b5/src/ezdxf/layouts/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/layouts/layouts.py` & `ezdxf-1.1.0b5/src/ezdxf/layouts/layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/attributes.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/const.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/encoding.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/extendedtags.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/extendedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/fileindex.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/fileindex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/hdrvars.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/hdrvars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/loader.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/packedtags.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/packedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/repair.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/repair.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/tagger.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/tagger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/tags.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/tagwriter.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/tagwriter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/types.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/lldxf/validator.py` & `ezdxf-1.1.0b5/src/ezdxf/lldxf/validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/arc.py` & `ezdxf-1.1.0b5/src/ezdxf/math/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/bbox.py` & `ezdxf-1.1.0b5/src/ezdxf/math/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/bezier.py` & `ezdxf-1.1.0b5/src/ezdxf/math/bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/bezier_interpolation.py` & `ezdxf-1.1.0b5/src/ezdxf/math/bezier_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/box.py` & `ezdxf-1.1.0b5/src/ezdxf/math/box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/bspline.py` & `ezdxf-1.1.0b5/src/ezdxf/math/bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/bulge.py` & `ezdxf-1.1.0b5/src/ezdxf/math/bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/circle.py` & `ezdxf-1.1.0b5/src/ezdxf/math/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/clipping.py` & `ezdxf-1.1.0b5/src/ezdxf/math/clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/clustering.py` & `ezdxf-1.1.0b5/src/ezdxf/math/clustering.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/construct2d.py` & `ezdxf-1.1.0b5/src/ezdxf/math/construct2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/construct3d.py` & `ezdxf-1.1.0b5/src/ezdxf/math/construct3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/cspline.py` & `ezdxf-1.1.0b5/src/ezdxf/math/cspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/curvetools.py` & `ezdxf-1.1.0b5/src/ezdxf/math/curvetools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/ellipse.py` & `ezdxf-1.1.0b5/src/ezdxf/math/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/eulerspiral.py` & `ezdxf-1.1.0b5/src/ezdxf/math/eulerspiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/linalg.py` & `ezdxf-1.1.0b5/src/ezdxf/math/linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/line.py` & `ezdxf-1.1.0b5/src/ezdxf/math/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/offset2d.py` & `ezdxf-1.1.0b5/src/ezdxf/math/offset2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/parametrize.py` & `ezdxf-1.1.0b5/src/ezdxf/math/parametrize.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/perlin.py` & `ezdxf-1.1.0b5/src/ezdxf/math/perlin.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/polyline.py` & `ezdxf-1.1.0b5/src/ezdxf/math/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/rtree.py` & `ezdxf-1.1.0b5/src/ezdxf/math/rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/shape.py` & `ezdxf-1.1.0b5/src/ezdxf/math/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/surfaces.py` & `ezdxf-1.1.0b5/src/ezdxf/math/surfaces.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/transformtools.py` & `ezdxf-1.1.0b5/src/ezdxf/math/transformtools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/triangulation.py` & `ezdxf-1.1.0b5/src/ezdxf/math/triangulation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/ucs.py` & `ezdxf-1.1.0b5/src/ezdxf/math/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/_bezier3p.py` & `ezdxf-1.1.0b5/src/ezdxf/math/_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/_bezier4p.py` & `ezdxf-1.1.0b5/src/ezdxf/math/_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/_bspline.py` & `ezdxf-1.1.0b5/src/ezdxf/math/_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/_construct.py` & `ezdxf-1.1.0b5/src/ezdxf/math/_construct.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/_ctypes.py` & `ezdxf-1.1.0b5/src/ezdxf/math/_ctypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/_mapbox_earcut.py` & `ezdxf-1.1.0b5/src/ezdxf/math/_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/_matrix44.py` & `ezdxf-1.1.0b5/src/ezdxf/math/_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/_vector.py` & `ezdxf-1.1.0b5/src/ezdxf/math/_vector.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/math/__init__.py` & `ezdxf-1.1.0b5/src/ezdxf/math/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/path/commands.py` & `ezdxf-1.1.0b5/src/ezdxf/path/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/path/converter.py` & `ezdxf-1.1.0b5/src/ezdxf/path/converter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/path/nesting.py` & `ezdxf-1.1.0b5/src/ezdxf/path/nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/path/path.py` & `ezdxf-1.1.0b5/src/ezdxf/path/path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/path/shapes.py` & `ezdxf-1.1.0b5/src/ezdxf/path/shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/path/tools.py` & `ezdxf-1.1.0b5/src/ezdxf/path/tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.css` & `ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.html` & `ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.html`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.js` & `ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.js`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.py` & `ezdxf-1.1.0b5/src/ezdxf/pp/dxfpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/pp/pprint.py` & `ezdxf-1.1.0b5/src/ezdxf/pp/pprint.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.css` & `ezdxf-1.1.0b5/src/ezdxf/pp/rawpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.py` & `ezdxf-1.1.0b5/src/ezdxf/pp/rawpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/pp/reflinks.py` & `ezdxf-1.1.0b5/src/ezdxf/pp/reflinks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/abstract_mtext_renderer.py` & `ezdxf-1.1.0b5/src/ezdxf/render/abstract_mtext_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/arrows.py` & `ezdxf-1.1.0b5/src/ezdxf/render/arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/curves.py` & `ezdxf-1.1.0b5/src/ezdxf/render/curves.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/dimension.py` & `ezdxf-1.1.0b5/src/ezdxf/render/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/dim_base.py` & `ezdxf-1.1.0b5/src/ezdxf/render/dim_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/dim_curved.py` & `ezdxf-1.1.0b5/src/ezdxf/render/dim_curved.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/dim_diameter.py` & `ezdxf-1.1.0b5/src/ezdxf/render/dim_diameter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/dim_linear.py` & `ezdxf-1.1.0b5/src/ezdxf/render/dim_linear.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/dim_ordinate.py` & `ezdxf-1.1.0b5/src/ezdxf/render/dim_ordinate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/dim_radius.py` & `ezdxf-1.1.0b5/src/ezdxf/render/dim_radius.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/forms.py` & `ezdxf-1.1.0b5/src/ezdxf/render/forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/hatching.py` & `ezdxf-1.1.0b5/src/ezdxf/render/hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/leader.py` & `ezdxf-1.1.0b5/src/ezdxf/render/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/linetypes.py` & `ezdxf-1.1.0b5/src/ezdxf/render/linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/mesh.py` & `ezdxf-1.1.0b5/src/ezdxf/render/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/mleader.py` & `ezdxf-1.1.0b5/src/ezdxf/render/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/mline.py` & `ezdxf-1.1.0b5/src/ezdxf/render/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/point.py` & `ezdxf-1.1.0b5/src/ezdxf/render/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/polyline.py` & `ezdxf-1.1.0b5/src/ezdxf/render/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/r12spline.py` & `ezdxf-1.1.0b5/src/ezdxf/render/r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/trace.py` & `ezdxf-1.1.0b5/src/ezdxf/render/trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/_linetypes.py` & `ezdxf-1.1.0b5/src/ezdxf/render/_linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/render/__init__.py` & `ezdxf-1.1.0b5/src/ezdxf/render/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/16x16.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/16x16.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/24x24.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/24x24.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/256x256.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/256x256.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/32x32.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/32x32.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/48x48.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/48x48.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/64x64.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/64x64.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-copy-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-copy-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-find-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-find-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-bookmark-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-goto-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-handle-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-goto-handle-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-line-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-goto-line-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-left-arrow-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-left-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-next-entity-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-next-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-prev-entity-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-prev-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-right-arrow-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-right-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-show-in-tree-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-show-in-tree-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/resources/icon-store-bookmark-64px.png` & `ezdxf-1.1.0b5/src/ezdxf/resources/icon-store-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/sections/acdsdata.py` & `ezdxf-1.1.0b5/src/ezdxf/sections/acdsdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/sections/blocks.py` & `ezdxf-1.1.0b5/src/ezdxf/sections/blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/sections/classes.py` & `ezdxf-1.1.0b5/src/ezdxf/sections/classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/sections/entities.py` & `ezdxf-1.1.0b5/src/ezdxf/sections/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/sections/header.py` & `ezdxf-1.1.0b5/src/ezdxf/sections/header.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/sections/headervars.py` & `ezdxf-1.1.0b5/src/ezdxf/sections/headervars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/sections/objects.py` & `ezdxf-1.1.0b5/src/ezdxf/sections/objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/sections/table.py` & `ezdxf-1.1.0b5/src/ezdxf/sections/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/sections/tables.py` & `ezdxf-1.1.0b5/src/ezdxf/sections/tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/analyze.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/analyze.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/binarydata.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/binarydata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/codepage.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/codepage.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/complex_ltype.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/complex_ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/crypt.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/debug.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/debug.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/difftags.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/handle.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/indexing.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/juliandate.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/pattern.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/rawloader.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/rawloader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/standards.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/standards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/strip.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/strip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/test.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/test.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/text.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/text_layout.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/text_size.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/zipmanager.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/zipmanager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/_iso_pattern.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/_iso_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf/tools/__init__.py` & `ezdxf-1.1.0b5/src/ezdxf/tools/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/src/ezdxf.egg-info/PKG-INFO` & `ezdxf-1.1.0b5/src/ezdxf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.1.0b4
+Version: 1.1.0b5
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -66,14 +66,15 @@
 - read/write/new support for DXF versions: R12, R2000, R2004, R2007, R2010, R2013 and R2018
 - additional read-only support for DXF versions R13/R14 (upgraded to R2000)
 - additional read-only support for older DXF versions than R12 (upgraded to R12)
 - read/write support for ASCII DXF and Binary DXF
 - retains third-party DXF content
 - optional C-extensions for CPython are included in the binary wheels, available 
   on [PyPI](https://pypi.org/project/ezdxf/) for Windows, Linux and macOS
+- command line script `ezdxf` to display, convert and inspect DXF files
 
 Included Extensions
 -------------------
 
 Additional packages required for these add-ons are not automatically installed 
 during the *basic* setup, for more information about the setup & dependencies 
 visit the [documentation](https://ezdxf.mozman.at/docs/setup.html).
@@ -159,14 +160,48 @@
 drawing add-on:
 
     pip install ezdxf[draw]
 
 For more information about the setup & dependencies visit the 
 [documentation](https://ezdxf.mozman.at/docs/setup.html).
 
+Command Line
+------------
+
+Use `python -m ezdxf ...` if your shell can't find the `ezdxf` script.
+
+Get additional help for a sub-command:
+
+    ezdxf <cmd> -h
+
+Preview DXF files in a graphical window:
+
+    ezdxf view <file.dxf>
+
+Export the modelspace of DXF files as PNG|SVG|PDF:
+
+    ezdxf draw -o file.<png|svg|pdf> <file.dxf>
+
+Print basic information about DXF files:
+
+    ezdxf info <file.dxf>
+
+Show detailed information and structures of DXF files:
+
+    ezdxf browse <file.dxf>
+
+Audit DXF files:
+
+    ezdxf audit <file.dxf>
+
+Preview and convert HPGL/2 plot files:
+
+    ezdxf hpgl <file.plt>
+
+
 Website
 -------
 
 https://ezdxf.mozman.at/
 
 Documentation
 -------------
@@ -233,14 +268,18 @@
 - NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
   add-on to change/override foreground- and background color by the frontend 
 - NEW: `TextPolicy` configuration settings for the `drawing` add-on, render text as 
   solid filling, outline path, replace text by (filled) rectangles or ignore text at all 
 - NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
   stroke fonts included in CAD applications
 - NEW: added setter to `BlockLayout.base_point` property
+- NEW: `ezdxf.entities.acad_table_to_block()` function, converts a `ACAD_TABLE` entity 
+  to an `INSERT` entity
+- NEW: `ACADProxyEntity.explode()` method, to explode `ACAD_PROXY_ENTITY` into proxy 
+  graphic entities
 - CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
   including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
 - REMOVED: configuration option `use_matplotlib` - is not needed anymore
 - REMOVED: configuration option `font_cache_directory` - is not needed anymore
@@ -252,15 +291,20 @@
 - REMOVED: Matplotlib/Qt path converters from `ezdxf.path.converter`
 - REMOVED: `Pillow` backend and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
 - BUGFIX: [#898](https://github.com/mozman/ezdxf/issues/898)
-  use `dimclrd` color for dimension arrow blocks 
+  use `dimclrd` color for dimension arrow blocks
+- BUGFIX: [#906](https://github.com/mozman/ezdxf/issues/906)
+  linetype and fill flag parsing for proxy graphics 
+- BUGFIX: [#907](https://github.com/mozman/ezdxf/issues/907)
+  fix ATTRIB and ATTDEF handling of version- and lock_position tags which share the 
+  same group code 280 in the same subclass
 
 Version 1.0.3 - 2023-03-26
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing
```

## Comparing `ezdxf-1.1.0b4/src/ezdxf.egg-info/SOURCES.txt` & `ezdxf-1.1.0b5/src/ezdxf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_010_binary_data.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_010_binary_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_012_crypt.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_012_crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_013_juliandate.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_013_juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_016_encoding.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_016_encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_018_handle.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_018_handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_024_render_tag.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_024_render_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_040_tags.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_040_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_041_group_tags.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_041_group_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py` & `ezdxf-1.1.0b5/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_101_dxfnamespace.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_101_dxfnamespace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_102_appdata.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_102_appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_103_reactors.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_103_reactors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_104_extension_dict.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_104_extension_dict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_105_xdata.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_105_xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_110_dxfentity.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_110_dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112a_dxfgfx.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_112a_dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112b_dxfobj.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_112b_dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_113_dxfclass.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_113_dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_114_factory.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_114_factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_115_new_empty_drawing.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_115_new_empty_drawing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_116_dictionary.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_116_dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_117_layer_table_entry.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_117_layer_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_119_ucs_table_entry.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_119_ucs_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_120_style_table_entry.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_120_style_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_121_ltype_table_entry.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_121_ltype_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_123_view_table_entry.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_123_view_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_125_image_def.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_125_image_def.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_126_image_def_reactor.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_126_image_def_reactor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_127_raster_variables.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_127_raster_variables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_128_pdf_definition.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_128_pdf_definition.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_129_xrecord.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_129_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_130_id_buffer.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_130_id_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_131_field_list.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_131_field_list.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_132_layer_filter.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_132_layer_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_133_sun.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_133_sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_134_material.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_134_material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_135_geo_data.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_135_geo_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_136_vba_project.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_136_vba_project.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_137_sortentstable.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_137_sortentstable.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_138_setup_visual_styles.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_138_setup_visual_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_139_user_record.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_139_user_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_140_block_record.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_140_block_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_141_layer_vp_override.py` & `ezdxf-1.1.0b5/tests/test_01_dxf_entities/test_141_layer_vp_override.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/conftest.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_200_line.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_200_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_201_point.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_201_point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_202_circle.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_202_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_203_arc.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_203_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_204_shape.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_204_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_205_solid.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_205_solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_206_text.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_206_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_207_attdef.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_207_attdef.py`

 * *Files 20% similar despite different names*

```diff
@@ -208,14 +208,151 @@
 
     def test_dxf_export_matches_test_data(self, attdef):
         result = TagCollector.dxftags(attdef, dxfversion=const.DXF2018)
         expected = basic_tags_from_text(EMBEDDED_MTEXT)
         assert result == expected
 
 
+def test_lock_position_and_ignore_version_tag():
+    """Version tag and lock_position tags are present."""
+    attdef = AttDef.from_text(LOCK_POSITION_AND_VERSION)
+    assert attdef.dxf.lock_position == 2
+
+
+def test_lock_position_without_version_tag():
+    """Just the lock_position tag is present."""
+    attdef = AttDef.from_text(LOCK_POSITION_WITHOUT_VERSION)
+    assert attdef.dxf.lock_position == 2
+
+
+def test_version_without_lock_position():
+    """Only the version tag is present and the lock_position tag is missing.
+
+    The version tag is always 0 and just for testing purposes set to 7:
+    """
+    attdef = AttDef.from_text(VERSION_WITHOUT_LOCK_POSITION)
+    assert attdef.dxf.lock_position == 7
+
+
+LOCK_POSITION_AND_VERSION = """  0
+ATTDEF
+5
+0
+330
+0
+100
+AcDbEntity
+8
+AttribLayer
+100
+AcDbText
+10
+1
+20
+2
+30
+0
+40
+3.0
+1
+TEST VENUE
+7
+Arial_3 NARROW
+100
+AcDbAttributeDefinition
+280
+0
+3
+TITLE-OF-DRAWING
+2
+DRAWING-NAME
+70
+0
+74
+2
+280
+2
+"""
+
+LOCK_POSITION_WITHOUT_VERSION = """  0
+ATTDEF
+5
+0
+330
+0
+100
+AcDbEntity
+8
+AttribLayer
+100
+AcDbText
+10
+1
+20
+2
+30
+0
+40
+3.0
+1
+TEST VENUE
+7
+Arial_3 NARROW
+100
+AcDbAttributeDefinition
+3
+TITLE-OF-DRAWING
+2
+DRAWING-NAME
+70
+0
+74
+2
+280
+2
+"""
+
+VERSION_WITHOUT_LOCK_POSITION = """  0
+ATTDEF
+5
+0
+330
+0
+100
+AcDbEntity
+8
+AttribLayer
+100
+AcDbText
+10
+1
+20
+2
+30
+0
+40
+3.0
+1
+TEST VENUE
+7
+Arial_3 NARROW
+100
+AcDbAttributeDefinition
+280
+7
+3
+TITLE-OF-DRAWING
+2
+DRAWING-NAME
+70
+0
+74
+2
+"""
+
 EMBEDDED_MTEXT = r"""  0
 ATTDEF
 5
 28A
 330
 285
 100
@@ -244,16 +381,14 @@
 45.3
 21
 45.0
 31
 0.0
 100
 AcDbAttributeDefinition
-280
-0
 3
 TITLE-OF-DRAWING
 2
 DRAWING-NAME
 70
 0
 74
```

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_208_attrib.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_208_attrib.py`

 * *Files 18% similar despite different names*

```diff
@@ -152,17 +152,15 @@
 
 def test_load_from_text(entity):
     assert entity.dxf.layer == "0"
     assert entity.dxf.color == 256, "default color is 256 (by layer)"
     assert entity.dxf.insert == (0, 0, 0)
 
 
-@pytest.mark.parametrize(
-    "txt,ver", [(ENTITY_R2000, DXF2000), (ENTITY_R12, DXF12)]
-)
+@pytest.mark.parametrize("txt,ver", [(ENTITY_R2000, DXF2000), (ENTITY_R12, DXF12)])
 def test_write_dxf(txt, ver):
     expected = basic_tags_from_text(txt)
     attdef = TEST_CLASS.from_text(txt)
     collector = TagCollector(dxfversion=ver, optional=True)
     attdef.export_dxf(collector)
     assert collector.tags == expected
 
@@ -256,15 +254,36 @@
     def test_set_invalid_mtext_attribute(self):
         txt = EmbeddedMText()
         assert txt.dxf.hasattr("color") is False
         with pytest.raises(AttributeError):
             txt.dxf.color = 3
 
 
-EMBEDDED_MTEXT = r"""0
+def test_lock_position_and_ignore_version_tag():
+    """Version tag and lock_position tags are present."""
+    attrib = Attrib.from_text(LOCK_POSITION_AND_VERSION)
+    assert attrib.dxf.lock_position == 2
+
+
+def test_lock_position_without_version_tag():
+    """Just the lock_position tag is present."""
+    attrib = Attrib.from_text(LOCK_POSITION_WITHOUT_VERSION)
+    assert attrib.dxf.lock_position == 2
+
+
+def test_version_without_lock_position():
+    """Only the version tag is present and the lock_position tag is missing.
+
+    The version tag is always 0 and just for testing purposes set to 7:
+    """
+    attrib = Attrib.from_text(VERSION_WITHOUT_LOCK_POSITION)
+    assert attrib.dxf.lock_position == 7
+
+
+LOCK_POSITION_AND_VERSION = """0
 ATTRIB
 5
 2AE
 330
 2AD
 100
 AcDbEntity
@@ -301,14 +320,152 @@
 2
 DRAWING-NAME
 70
 0
 74
 2
 280
+2
+"""
+
+LOCK_POSITION_WITHOUT_VERSION = """0
+ATTRIB
+5
+2AE
+330
+2AD
+100
+AcDbEntity
+8
+AttribLayer
+62
+7
+100
+AcDbText
+10
+574.8
+20
+961.1
+30
+0.0
+40
+3.0
+1
+TEST VENUE
+7
+Arial_3 NARROW
+72
+1
+11
+592.3
+21
+962.6
+31
+0.0
+100
+AcDbAttribute
+2
+DRAWING-NAME
+70
+0
+74
+2
+280
+2
+"""
+
+VERSION_WITHOUT_LOCK_POSITION = """0
+ATTRIB
+5
+2AE
+330
+2AD
+100
+AcDbEntity
+8
+AttribLayer
+62
+7
+100
+AcDbText
+10
+574.8
+20
+961.1
+30
+0.0
+40
+3.0
+1
+TEST VENUE
+7
+Arial_3 NARROW
+72
+1
+11
+592.3
+21
+962.6
+31
+0.0
+100
+AcDbAttribute
+280
+7
+2
+DRAWING-NAME
+70
+0
+74
+2
+"""
+
+EMBEDDED_MTEXT = r"""0
+ATTRIB
+5
+2AE
+330
+2AD
+100
+AcDbEntity
+8
+AttribLayer
+62
+7
+100
+AcDbText
+10
+574.8
+20
+961.1
+30
+0.0
+40
+3.0
+1
+TEST VENUE
+7
+Arial_3 NARROW
+72
+1
+11
+592.3
+21
+962.6
+31
+0.0
+100
+AcDbAttribute
+2
+DRAWING-NAME
+70
+0
+74
+2
+280
 0
 71
 2
 72
 0
 11
 592.3
```

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_209_vertex.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_209_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_1.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_2.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_explode.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_211_viewport.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_211_viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_212_insert.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_212_insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_213_minsert.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_213_minsert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_214_block.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_214_block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_215_dimension.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_215_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_216_dimlines_R12.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_216_dimlines_R12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_221_ellipse.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_221_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_222_xline.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_222_xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_223_ray.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_223_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_224_group.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_224_group.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_225_mtext.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_225_mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_226_spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_228_mesh.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_228_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229b_hatch_extended.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_229b_hatch_extended.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_231_underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay_2.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_231_underlay_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_232_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis_2.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_232_acis_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_surface.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_232_surface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_233_helix.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_233_helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_234_light.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_234_light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_235_leader.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_235_leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_236_multileader.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_236_multileader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_237_mline.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_237_mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_238_tolerance.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_238_tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_239_proxy_graphic.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_239_proxy_graphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_240_arc_dimension.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_240_arc_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_241_hyperlink.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_241_hyperlink.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_242_random_transform.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_242_random_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_243_replace_entity.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_243_replace_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_245_wipeout.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_245_wipeout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_246_spline_audit.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_246_spline_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mpolygon.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_248_mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_249_boundary_paths.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_249_boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_251_upright.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_251_upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_253_ole2frame.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_253_ole2frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_254_get_font_name.py` & `ezdxf-1.1.0b5/tests/test_02_dxf_graphics/test_254_get_font_name.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_300_layout.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_300_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_302_block_references.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_302_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_303_auto_block_references.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_303_auto_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_304_new_entity_space.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_304_new_entity_space.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_307_groupby.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_307_groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_308_query.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_308_query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_309_query_parser.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_309_query_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_312_virtual_layout.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_312_virtual_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_313_redraw_order.py` & `ezdxf-1.1.0b5/tests/test_03_dxf_layouts/test_313_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_401_headersection.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_401_headersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_402_classessection.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_402_classessection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_403_entity_database.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_403_entity_database.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404a_tables.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_404a_tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_405_classes.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_405_classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_407_entity_section.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_407_entity_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_408_objects_section.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_408_objects_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_409_create_objects.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_409_create_objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_410_table.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_410_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_411_acds_data.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_411_acds_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_415_layout_management.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_415_layout_management.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_417_bbox.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_417_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_424_audit.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_424_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_427_appsettings.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_427_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py` & `ezdxf-1.1.0b5/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/conftest.py` & `ezdxf-1.1.0b5/tests/test_05_tools/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_500_units.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_500_units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_501_truecolor.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_501_truecolor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_502_raw_color.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_502_raw_color.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_503_indexing.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_503_indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_504_suppress_zeros.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_504_suppress_zeros.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_507_dxf_pretty_printer.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_507_dxf_pretty_printer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_508_read_zip.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_508_read_zip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_509_comments.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_509_comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_510_byte_stream.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_510_byte_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_511_bit_stream.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_511_bit_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_512_pattern.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_512_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_513_reorder_entities.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_513_reorder_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_514_text.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_514_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_515a_fonts_truetype.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_515a_fonts_truetype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_515b_fonts_shapefiles.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_515b_fonts_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_515c_fonts_lff.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_515c_fonts_lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_516_zoom.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_516_zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_517_text_layout.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_517_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_519_mtext_editor.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_519_mtext_editor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_520_mtext_context.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_520_mtext_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_521_mtext_parser.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_521_mtext_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_522_text_scanner.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_522_text_scanner.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_523_text_size.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_523_text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_524_block_reference_manager.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_524_block_reference_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_525_transparency.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_525_transparency.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_526_explode.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_526_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_527_gfxattribs.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_527_gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_528_difftags.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_528_difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_529_acis_sat.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_529_acis_sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_530_acis_sab.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_530_acis_sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_531_acis_entities.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_531_acis_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_532_acis_mesh.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_532_acis_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_533_shapefiles.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_533_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_534_dwg_info.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_534_dwg_info.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_535_xref_basic.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_535_xref_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,14 +539,17 @@
         assert document_has_no_errors(tdoc) is True
 
         loaded_block_ref = cast(Insert, tdoc.modelspace()[0])
         loaded_block_name = loaded_block_ref.dxf.name
         assert (
             loaded_block_name == "*U4"
         ), "expected next available anonymous block name in tdoc"
+        block_layout = tdoc.blocks.get(loaded_block_name)
+        assert block_layout.block_record.dxf.name == loaded_block_name
+        assert block_layout.block.dxf.name == loaded_block_name
 
 
 def test_loaded_external_reference():
     sdoc = ezdxf.new()
     sdoc.add_xref_def("my.dxf", "my_xref")
     sdoc.modelspace().add_blockref("my_xref", insert=(0, 0))
```

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_536_xref_conflict.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_536_xref_conflict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_537_transform.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_537_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_538_scale_mtext_inline_commands.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_538_scale_mtext_inline_commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_539_npshapes.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_539_npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_05_tools/test_540_lff_parser.py` & `ezdxf-1.1.0b5/tests/test_05_tools/test_540_lff_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/conftest.py` & `ezdxf-1.1.0b5/tests/test_06_math/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_600_base.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_600_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_601_bulge.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_601_bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_602_vec3.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_602_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_603_vec2.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_603_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_604_banded_matrix.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_604_banded_matrix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_604_linalg.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_604_linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_605_matrix44.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_605_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_606_convexhull.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_606_convexhull.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_607_perlin_noise.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_607_perlin_noise.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_608_intersection_line_line_2d.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_608_intersection_line_line_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_609_point_on_line.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_609_point_on_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_610_ocs.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_610_ocs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_611_ucs.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_611_ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_612_ucs_pass_trough.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_612_ucs_pass_trough.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_613_point_in_poygon.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_613_point_in_poygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_614_construct_3d.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_614_construct_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_615_rytz_axis.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_615_rytz_axis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_616_plane.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_616_plane.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_617_clockwise_orientation.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_617_clockwise_orientation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_618_clipping.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_618_clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_619_greiner_hormann.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_619_greiner_hormann.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_620_knot.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_620_knot.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_621_bspline.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_621_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_622_bsplineu.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_622_bsplineu.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_623_rbspline.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_623_rbspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_624_global_bspline_interpolation.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_624_global_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_626_local_bspline_interpolation.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_626_local_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_627_bspline_basis.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_627_bspline_basis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_629_bezier.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_629_bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_630a_bezier4p_base.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_630a_bezier4p_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_630b_bezier4p_functions.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_630b_bezier4p_functions.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_631_euler_spiral.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_631_euler_spiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_632_bezier3p.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_632_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_640_bbox.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_640_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_641_construction_ray.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_641_construction_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_642_construction_line.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_642_construction_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_643_construction_box.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_643_construction_box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_644_construction_circle.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_644_construction_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_645_construction_arc.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_645_construction_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_646_offset_vertices_2d.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_646_offset_vertices_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_647_transform_tools.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_647_transform_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_648_construction_ellipse.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_648_construction_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_650_elliptic_arc_span.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_650_elliptic_arc_span.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_651_construction_polyline.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_651_construction_polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_652_approx_param_t.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_652_approx_param_t.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_653_polyline_intersection.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_653_polyline_intersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_654_rtree.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_654_rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_655_dbscan.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_655_dbscan.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_656_k_means.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_656_k_means.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_657_mapbox_earcut.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_657_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_658_bevel_tools.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_658_bevel_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_659_intersection_line_polygon_3d.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_659_intersection_line_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_660_intersection_ray_polygon_3d.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_660_intersection_ray_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_06_math/test_662_is_convex_polygon_2d.py` & `ezdxf-1.1.0b5/tests/test_06_math/test_662_is_convex_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_701_arrows.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_701_arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_702_render_forms.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_702_render_forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_703_mesh_builder.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_703_mesh_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_704_render_linear_dimension.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_704_render_linear_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_705_shape.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_705_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_707_trace.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_707_trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_708a_path.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_708a_path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_708b_path_tools.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_708b_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_708c_matplotlib_path_tools.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_708c_matplotlib_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_708d_qpainter_path_tools.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_708d_qpainter_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_708e_path_shapes.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_708e_path_shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_708f_path_nesting.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_708f_path_nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_709_linetype_renderer.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_709_linetype_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_711_points.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_711_points.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_712_render_curved_dimension.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_712_render_curved_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_713_mleader_builder.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_713_mleader_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_714_mleader_render_engine.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_714_mleader_render_engine.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_715_hatching.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_715_hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_07_render/test_715_issue_747_explode_3d_dim.py` & `ezdxf-1.1.0b5/tests/test_07_render/test_715_issue_747_explode_3d_dim.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_800_mtext_surrogate.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_800_mtext_surrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_801_r12spline.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_801_r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_802_table_painter.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_802_table_painter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_803_entities_to_code.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_803_entities_to_code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_804_importer.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_804_importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_805_pycsg.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_805_pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_806_acadctb.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_806_acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_807_dwg_loader_basics.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_807_dwg_loader_basics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_810_drawing_properties.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_810_drawing_properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_811a_drawing_frontend.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_811a_drawing_frontend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_811b_drawing_recorder.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_811b_drawing_recorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_811c_viewport_processing.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_811c_viewport_processing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_812_drawing_graphic_proxy.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_812_drawing_graphic_proxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_813_geo_interface.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_813_geo_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_814_text2path.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_814_text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_815_dxf_browser.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_815_dxf_browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_816_bin_packing.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_816_bin_packing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_817_genetic_algorithm.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_817_genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_818_meshex.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_818_meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_819_menger_sponge.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_819_menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_820_openscad.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_820_openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_821_hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_822_clipper.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_822_clipper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_823_drawing_layout.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_823_drawing_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_824_svg_drawing_backend.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_824_svg_drawing_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_08_addons/test_825_hpgl2_drawing_backend.py` & `ezdxf-1.1.0b5/tests/test_08_addons/test_825_hpgl2_drawing_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_901_acc_vec2.py` & `ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_901_acc_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_902_acc_vec3.py` & `ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_902_acc_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_903_acc_matrix44.py` & `ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_903_acc_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py` & `ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py` & `ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_906_acc_bspline.py` & `ezdxf-1.1.0b5/tests/test_09_cython_acceleration/test_906_acc_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_414_bbox_calculation.py` & `ezdxf-1.1.0b5/tests/test_10_issues/test_issue_414_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py` & `ezdxf-1.1.0b5/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_574_flattening_error.py` & `ezdxf-1.1.0b5/tests/test_10_issues/test_issue_574_flattening_error.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py` & `ezdxf-1.1.0b5/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_749_text_layout.py` & `ezdxf-1.1.0b5/tests/test_10_issues/test_issue_749_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_873_circle_inverted_normal.py` & `ezdxf-1.1.0b5/tests/test_10_issues/test_issue_873_circle_inverted_normal.py`

 * *Files identical despite different names*

