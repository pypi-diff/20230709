# Comparing `tmp/ScriptCollection-3.4.0-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 61676 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat    18794 b- defN 23-Jun-27 21:57 ScriptCollection/Executables.py
+Zip file size: 62303 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat    19068 b- defN 23-Jul-09 10:07 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34378 b- defN 23-Jun-27 21:57 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6275 b- defN 23-May-26 16:46 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    95771 b- defN 23-Jun-27 21:57 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   139730 b- defN 23-Jun-27 21:57 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat    96083 b- defN 23-Jul-09 10:08 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   144026 b- defN 23-Jul-09 10:07 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7649 b- defN 23-Jun-27 21:58 ScriptCollection-3.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-27 21:58 ScriptCollection-3.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2088 b- defN 23-Jun-27 21:58 ScriptCollection-3.4.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-27 21:58 ScriptCollection-3.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1290 b- defN 23-Jun-27 21:58 ScriptCollection-3.4.0.dist-info/RECORD
-14 files, 318962 bytes uncompressed, 59494 bytes compressed:  81.3%
+-rw-rw-rw-  2.0 fat     7649 b- defN 23-Jul-09 10:08 ScriptCollection-3.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 10:08 ScriptCollection-3.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-09 10:08 ScriptCollection-3.4.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-09 10:08 ScriptCollection-3.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-09 10:08 ScriptCollection-3.4.1.dist-info/RECORD
+14 files, 323844 bytes uncompressed, 60121 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.4.0.dist-info/METADATA
+Filename: ScriptCollection-3.4.1.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.4.0.dist-info/WHEEL
+Filename: ScriptCollection-3.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.4.0.dist-info/entry_points.txt
+Filename: ScriptCollection-3.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.0.dist-info/top_level.txt
+Filename: ScriptCollection-3.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.0.dist-info/RECORD
+Filename: ScriptCollection-3.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/Executables.py

```diff
@@ -278,29 +278,31 @@
     return ScriptCollectionCore().SCHealthcheck(args.file)
 
 
 def BuildCodeUnit() -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('--codeunitfolder', required=False, default=".")
     parser.add_argument('--verbosity', required=False, default=1)
-    parser.add_argument('--buildenvironment', required=False, default="QualityCheck")
+    parser.add_argument('--targetenvironment', required=False, default="Development")
     parser.add_argument('--additionalargumentsfile', required=False, default=None)
+    parser.add_argument('--assume_dependent_codeunits_are_already_built', type=GeneralUtilities.string_to_boolean, const=True, default=False, nargs='?',)
     args = parser.parse_args()
-    TasksForCommonProjectStructure().build_codeunit(args.codeunitfolder, int(args.verbosity), args.buildenvironment, args.additionalargumentsfile)
+    TasksForCommonProjectStructure().build_codeunit(args.codeunitfolder, int(args.verbosity), args.targetenvironment, args.additionalargumentsfile,
+                                                    False, None, args.assume_dependent_codeunits_are_already_built)
     return 0
 
 
 def BuildCodeUnits() -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('--repositoryfolder', required=False, default=".")
     parser.add_argument('--verbosity', required=False, default=1)
-    parser.add_argument('--buildenvironment', required=False, default="QualityCheck")
+    parser.add_argument('--targetenvironment', required=False, default="Development")
     parser.add_argument('--additionalargumentsfile', required=False, default=None)
     args = parser.parse_args()
-    TasksForCommonProjectStructure().build_codeunits(args.repositoryfolder, int(args.verbosity), args.buildenvironment, args.additionalargumentsfile)
+    TasksForCommonProjectStructure().build_codeunits(args.repositoryfolder, int(args.verbosity), args.targetenvironment, args.additionalargumentsfile)
     return 0
 
 
 def GenerateCertificateAuthority() -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument('--name', required=True)
     parser.add_argument('--subj_c', required=True)
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -25,15 +25,15 @@
 import PyPDF2
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.4.0"
+version = "3.4.1"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
@@ -1552,15 +1552,15 @@
             days_until_expire = 397
         if password is None:
             password = GeneralUtilities.generate_password()
         rsa_key_length = 4096
         self.run_program("openssl", f'genrsa -out {domain}.key {rsa_key_length}', folder)
         self.run_program("openssl", f'req -new -subj /C={subj_c}/ST={subj_st}/L={subj_l}/O={subj_o}/CN={domain}/OU={subj_ou} -x509 ' +
                          f'-key {domain}.key -out {domain}.unsigned.crt -days {days_until_expire}', folder)
-        self.run_program("openssl", f'pkcs12 -export -out {domain}.pfx -password pass:{password} -inkey {domain}.key -in {domain}.unsigned.crt', folder)
+        self.run_program("openssl", f'pkcs12 -export -out {domain}.selfsigned.pfx -password pass:{password} -inkey {domain}.key -in {domain}.unsigned.crt', folder)
         GeneralUtilities.write_text_to_file(os.path.join(folder, f"{domain}.password"), password)
         GeneralUtilities.write_text_to_file(os.path.join(folder, f"{domain}.san.conf"), f"""[ req ]
 default_bits        = {rsa_key_length}
 distinguished_name  = req_distinguished_name
 req_extensions      = v3_req
 default_md          = sha256
 dirstring_type      = nombstr
@@ -1587,16 +1587,19 @@
                          f'-key {domain}.key -out {domain}.csr -config {domain}.san.conf', folder)
 
     @GeneralUtilities.check_arguments
     def sign_certificate(self, folder: str, ca_folder: str, ca_name: str, domain: str, days_until_expire: int = None) -> None:
         if days_until_expire is None:
             days_until_expire = 397
         ca = os.path.join(ca_folder, ca_name)
-        self.run_program("openssl", f'x509 -req -in {domain}.csr -CA {ca}.crt -CAkey {ca}.key -CAserial {ca}.srl ' +
+        password_file = os.path.join(folder, f"{domain}.password")
+        password = GeneralUtilities.read_text_from_file(password_file)
+        self.run_program("openssl", f'x509 -req -in {domain}.csr -CA {ca}.crt -CAkey {ca}.key -CAcreateserial -CAserial {ca}.srl ' +
                          f'-out {domain}.crt -days {days_until_expire} -sha256 -extensions v3_req -extfile {domain}.san.conf', folder)
+        self.run_program("openssl", f'pkcs12 -export -out {domain}.pfx -inkey {domain}.key -in {domain}.crt -password pass:{password}', folder)
 
     @GeneralUtilities.check_arguments
     def update_dependencies_of_python_in_requirementstxt_file(self, file: str, verbosity: int):
         lines = GeneralUtilities.read_lines_from_file(file)
         new_lines = []
         for line in lines:
             new_lines.append(self.__get_updated_line_for_python_requirements(line.strip()))
```

## ScriptCollection/TasksForCommonProjectStructure.py

```diff
@@ -466,15 +466,15 @@
         <AppendTargetFrameworkToOutputPath>false<\\/AppendTargetFrameworkToOutputPath>
         <OutputPath>\\.\\.\\\\Other\\\\Artifacts\\\\BuildResult_DotNet_win-x64<\\/OutputPath>
         <PlatformTarget>([^<]+)<\\/PlatformTarget>
         <WarningLevel>\\d<\\/WarningLevel>
         <Prefer32Bit>false<\\/Prefer32Bit>
         <NoWarn>([^<]+)<\\/NoWarn>
         <WarningsAsErrors>([^<]+)<\\/WarningsAsErrors>
-        <ErrorLog>\\.\\.\\\\Other\\\\Resources\\\\{codeunit_name_regex}\\.sarif<\\/ErrorLog>
+        <ErrorLog>\\.\\.\\\\Other\\\\Resources\\\\CodeAnalysisResult\\\\{codeunit_name_regex}\\.sarif<\\/ErrorLog>
         <OutputType>([^<]+)<\\/OutputType>
         <DocumentationFile>\\.\\.\\\\Other\\\\Artifacts\\\\MetaInformation\\\\{codeunit_name_regex}\\.xml<\\/DocumentationFile>(\\n|.)*
     <\\/PropertyGroup>
     <PropertyGroup Condition=\\\"'\\$\\(Configuration\\)'=='Development'\\\">
         <DebugType>full<\\/DebugType>
         <DebugSymbols>true<\\/DebugSymbols>
         <Optimize>false<\\/Optimize>
@@ -527,15 +527,15 @@
         <AppendTargetFrameworkToOutputPath>false<\\/AppendTargetFrameworkToOutputPath>
         <OutputPath>\\.\\.\\\\Other\\\\Artifacts\\\\BuildResultTests_DotNet_win-x64<\\/OutputPath>
         <PlatformTarget>([^<]+)<\\/PlatformTarget>
         <WarningLevel>\\d<\\/WarningLevel>
         <Prefer32Bit>false<\\/Prefer32Bit>
         <NoWarn>([^<]+)<\\/NoWarn>
         <WarningsAsErrors>([^<]+)<\\/WarningsAsErrors>
-        <ErrorLog>\\.\\.\\\\Other\\\\Resources\\\\{codeunit_name_regex}Tests\\.sarif<\\/ErrorLog>
+        <ErrorLog>\\.\\.\\\\Other\\\\Resources\\\\CodeAnalysisResult\\\\{codeunit_name_regex}Tests\\.sarif<\\/ErrorLog>
         <OutputType>Library<\\/OutputType>(\\n|.)*
     <\\/PropertyGroup>
     <PropertyGroup Condition=\\\"'\\$\\(Configuration\\)'=='Development'\\\">
         <DebugType>full<\\/DebugType>
         <DebugSymbols>true<\\/DebugSymbols>
         <Optimize>false<\\/Optimize>
         <DefineConstants>TRACE;DEBUG;Development<\\/DefineConstants>
@@ -573,14 +573,16 @@
                                                     copy_license_file_to_target_folder: bool, repository_folder: str, codeunit_name: str, commandline_arguments: list[str]):
         dotnet_build_configuration: str = target_environmenttype_mapping[target_environmenttype]
         verbosity = self.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         codeunit_folder = os.path.join(repository_folder, codeunit_name)
         csproj_file_folder = os.path.dirname(csproj_file)
         csproj_file_name = os.path.basename(csproj_file)
         csproj_file_name_without_extension = csproj_file_name.split(".")[0]
+        sarif_folder = os.path.join(codeunit_folder, "Other", "Resources", "CodeAnalysisResult")
+        GeneralUtilities.ensure_directory_exists(sarif_folder)
         for runtime in runtimes:
             outputfolder = originaloutputfolder+runtime
             self.__sc.run_program("dotnet", "clean", csproj_file_folder, verbosity=verbosity)
             GeneralUtilities.ensure_directory_does_not_exist(os.path.join(csproj_file_folder, "obj"))
             GeneralUtilities.ensure_directory_does_not_exist(outputfolder)
             GeneralUtilities.ensure_directory_exists(outputfolder)
             self.__sc.run_program("dotnet", "restore", codeunit_folder, verbosity=verbosity)
@@ -590,15 +592,15 @@
                 license_file = os.path.join(repository_folder, "License.txt")
                 target = os.path.join(outputfolder, f"{codeunit_name}.License.txt")
                 shutil.copyfile(license_file, target)
             for file, keyfile in files_to_sign.items():
                 self.__sc.dotnet_sign_file(os.path.join(outputfolder, file), keyfile, verbosity)
 
             sarif_filename = f"{csproj_file_name_without_extension}.sarif"
-            sarif_source_file = os.path.join(codeunit_folder, "Other", "Resources", sarif_filename)
+            sarif_source_file = os.path.join(sarif_folder, sarif_filename)
             if os.path.exists(sarif_source_file):
                 sarif_folder = os.path.join(codeunit_folder, "Other", "Artifacts", "CodeAnalysisResult")
                 GeneralUtilities.ensure_directory_exists(sarif_folder)
                 sarif_target_file = os.path.join(sarif_folder, sarif_filename)
                 GeneralUtilities.ensure_file_does_not_exist(sarif_target_file)
                 shutil.copyfile(sarif_source_file, sarif_target_file)
                 GeneralUtilities.ensure_file_does_not_exist(sarif_source_file)
@@ -1002,30 +1004,41 @@
 
     @GeneralUtilities.check_arguments
     def assert_no_uncommitted_changes(self, repository_folder: str):
         if self.__sc.git_repository_has_uncommitted_changes(repository_folder):
             raise ValueError(f"Repository '{repository_folder}' has uncommitted changes.")
 
     @GeneralUtilities.check_arguments
-    def generate_certificate_for_nonproductive_purposes(self, codeunit_folder: str, domain: str,
-                                                        subj_c: str, subj_st: str, subj_l: str, subj_o: str, subj_ou: str,
-                                                        resource_name: str = "NonProductiveCertificate"):
-        target_folder = os.path.join(codeunit_folder, "Other", "Resources", resource_name)
-        certificate_file = os.path.join(target_folder, f"{domain}.unsigned.crt")
+    def generate_certificate_for_nonproductive_purposes(self, codeunit_folder: str,
+                                                        resource_name: str = "DevelopmentCertificate"):
+        resources_folder = os.path.join(codeunit_folder, "Other", "Resources")
+        certificate_folder = os.path.join(resources_folder, resource_name)
+        dev_ca_name = "DevelopmentCertificateAuthority"
+        ca_folder = os.path.join(resources_folder, dev_ca_name)
+        codeunit_name = os.path.basename(codeunit_folder)
+        domain = f"{codeunit_name.lower()}.test.local"
+        certificate_file = os.path.join(certificate_folder, f"{domain}.crt")
+        unsignedcertificate_file = os.path.join(certificate_folder, f"{domain}.unsigned.crt")
         certificate_exists = os.path.exists(certificate_file)
         if certificate_exists:
             certificate_expired = GeneralUtilities.certificate_is_expired(certificate_file)
             generate_new_certificate = certificate_expired
         else:
             generate_new_certificate = True
         if generate_new_certificate:
-            GeneralUtilities.ensure_directory_does_not_exist(target_folder)
-            GeneralUtilities.ensure_directory_exists(target_folder)
-            GeneralUtilities.write_message_to_stdout("Generate TLS-certificate for non-productive purposes.")
-            self.__sc.generate_certificate(target_folder, domain, subj_c, subj_st, subj_l, subj_o, subj_ou)
+            GeneralUtilities.ensure_directory_does_not_exist(certificate_folder)
+            GeneralUtilities.ensure_directory_exists(certificate_folder)
+            GeneralUtilities.ensure_directory_does_not_exist(ca_folder)
+            GeneralUtilities.ensure_directory_exists(ca_folder)
+            GeneralUtilities.write_message_to_stdout("Generate TLS-certificate for development-purposes.")
+            self.__sc.generate_certificate_authority(ca_folder, dev_ca_name, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
+            self.__sc.generate_certificate(certificate_folder, domain, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
+            self.__sc.generate_certificate_sign_request(certificate_folder, domain, "DE", "SubjST", "SubjL", "SubjO", "SubjOU")
+            self.__sc.sign_certificate(certificate_folder, ca_folder, dev_ca_name, domain)
+            GeneralUtilities.ensure_file_does_not_exist(unsignedcertificate_file)
 
     @GeneralUtilities.check_arguments
     def get_codeunits(self, repository_folder: str) -> list[str]:
         result: list[str] = []
         for direct_subfolder in GeneralUtilities.get_direct_folders_of_folder(repository_folder):
             subfoldername = os.path.basename(direct_subfolder)
             if os.path.isfile(os.path.join(direct_subfolder, f"{subfoldername}.codeunit.xml")):
@@ -1374,66 +1387,62 @@
     def replace_common_variables_in_nuspec_file(self, codeunit_folder: str):
         codeunit_name = os.path.basename(codeunit_folder)
         codeunit_version = self.get_version_of_codeunit_folder(codeunit_folder)
         nuspec_file = os.path.join(codeunit_folder, "Other", "Build", f"{codeunit_name}.nuspec")
         self.__sc.replace_version_in_nuspec_file(nuspec_file, codeunit_version)
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_build_for_node_project(self, build_script_file: str, build_environment_target_type: str,
-                                                  verbosity: int, commandline_arguments: list[str]):
-        # TODO use unused parameter
+    def standardized_tasks_build_for_angular_codeunit(self, build_script_file: str, build_environment_target_type: str,
+                                                      verbosity: int, commandline_arguments: list[str]):
         self.copy_source_files_to_output_directory(build_script_file)
-        sc = ScriptCollectionCore()
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
-        sc.program_runner = ProgramRunnerEpew()
         build_script_folder = os.path.dirname(build_script_file)
         codeunit_folder = GeneralUtilities.resolve_relative_path("../..", build_script_folder)
-        sc.run_program("npm", "run build", codeunit_folder, verbosity=verbosity)
+        self.run_with_epew("ng", f"build --configuration {build_environment_target_type}", codeunit_folder, verbosity=verbosity)
         self.standardized_tasks_build_bom_for_node_project(codeunit_folder, verbosity, commandline_arguments)
 
     @GeneralUtilities.check_arguments
     def standardized_tasks_build_bom_for_node_project(self, codeunit_folder: str, verbosity: int, commandline_arguments: list[str]):
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
         # TODO
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_linting_for_node_project(self, linting_script_file: str, verbosity: int,
-                                                    target_environmenttype: str, commandline_arguments: list[str]):
-        # TODO use unused parameter
-        sc = ScriptCollectionCore()
+    def standardized_tasks_linting_for_angular_codeunit(self, linting_script_file: str, verbosity: int,
+                                                        build_environment_target_type: str, commandline_arguments: list[str]):
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
-        sc.program_runner = ProgramRunnerEpew()
         build_script_folder = os.path.dirname(linting_script_file)
         codeunit_folder = GeneralUtilities.resolve_relative_path("../..", build_script_folder)
-        sc.run_program("npm", "run lint", codeunit_folder, verbosity=verbosity)
+        self.run_with_epew("ng", "lint", codeunit_folder, verbosity=verbosity)
         # TODO check if there are errors in sarif-file
 
     @GeneralUtilities.check_arguments
-    def standardized_tasks_run_testcases_for_node_project(self, runtestcases_script_file: str,
-                                                          targetenvironmenttype: str, generate_badges: bool, verbosity: int,
-                                                          commandline_arguments: list[str]):
-        # TODO use targetenvironmenttype etc.
-        sc = ScriptCollectionCore()
+    def standardized_tasks_run_testcases_for_angular_codeunit(self, runtestcases_script_file: str,
+                                                              build_environment_target_type: str, generate_badges: bool, verbosity: int,
+                                                              commandline_arguments: list[str]):
         codeunit_name: str = os.path.basename(str(Path(os.path.dirname(runtestcases_script_file)).parent.parent.absolute()))
         verbosity = TasksForCommonProjectStructure.get_verbosity_from_commandline_arguments(commandline_arguments, verbosity)
-        sc.program_runner = ProgramRunnerEpew()
         codeunit_folder = GeneralUtilities.resolve_relative_path("../..", os.path.dirname(runtestcases_script_file))
-        sc.run_program("npm", "run test", codeunit_folder, verbosity=verbosity)
+        self.run_with_epew(
+            "ng", "test --watch=false --browsers ChromeHeadless --code-coverage", codeunit_folder, verbosity=verbosity)
         coverage_folder = os.path.join(codeunit_folder, "Other", "Artifacts", "TestCoverage")
         target_file = os.path.join(coverage_folder, "TestCoverage.xml")
         GeneralUtilities.ensure_file_does_not_exist(target_file)
         os.rename(os.path.join(coverage_folder, "cobertura-coverage.xml"), target_file)
         repository_folder = GeneralUtilities.resolve_relative_path("..", codeunit_folder)
-        self.run_testcases_common_post_task(repository_folder, codeunit_name, verbosity, generate_badges, targetenvironmenttype, commandline_arguments)
+        self.run_testcases_common_post_task(repository_folder, codeunit_name, verbosity, generate_badges, build_environment_target_type, commandline_arguments)
 
     @GeneralUtilities.check_arguments
     def do_npm_install(self, package_json_folder: str, verbosity: int):
-        sc = ScriptCollectionCore()
+        self.run_with_epew("npm", "install", package_json_folder, verbosity=verbosity)
+
+    @GeneralUtilities.check_arguments
+    def run_with_epew(self, program: str, argument: str, working_directory: str, verbosity: int):
+        sc: ScriptCollectionCore = ScriptCollectionCore()
         sc.program_runner = ProgramRunnerEpew()
-        sc.run_program("npm", "install", package_json_folder, verbosity=verbosity)
+        sc.run_program(program, argument, working_directory, verbosity=verbosity)
 
     @GeneralUtilities.check_arguments
     def set_default_constants(self, codeunit_folder: str):
         self.set_constant_for_commitid(codeunit_folder)
         self.set_constant_for_commitdate(codeunit_folder)
         self.set_constant_for_commitname(codeunit_folder)
         self.set_constant_for_commitversion(codeunit_folder)
@@ -1506,30 +1515,41 @@
             return ""
         elif length == 1:
             return results[0]
         else:
             raise ValueError("Too many results found.")
 
     @GeneralUtilities.check_arguments
-    def set_constants_for_certificate_public_information(self, codeunit_folder: str, domain: str, source_constant_name: str = "NonProductiveCertificate"):
+    def set_constants_for_certificate_public_information(self, codeunit_folder: str, source_constant_name: str = "DevelopmentCertificate"):
         """Expects a certificate-resource and generates a constant for its public information"""
-        certificate_file = os.path.join(codeunit_folder, "Other", "Resources", source_constant_name, f"{domain}.unsigned.crt")
+        codeunit_name = os.path.basename(codeunit_folder)
+        domain = f"{codeunit_name}.test.local"
+        certificate_file = os.path.join(codeunit_folder, "Other", "Resources", source_constant_name, f"{domain}.crt")
         with open(certificate_file, encoding="utf-8") as text_wrapper:
             certificate = crypto.load_certificate(crypto.FILETYPE_PEM, text_wrapper.read())
         certificate_publickey = crypto.dump_publickey(crypto.FILETYPE_PEM, certificate.get_pubkey()).decode("utf-8")
         self.set_constant(codeunit_folder, source_constant_name+"PublicKey", certificate_publickey)
 
     @GeneralUtilities.check_arguments
-    def set_constants_for_certificate_private_information(self, codeunit_folder: str, certificate_resource_name: str = "NonProductiveCertificate"):
+    def set_constants_for_certificate_private_information(self, codeunit_folder: str, certificate_resource_name: str = "DevelopmentCertificate"):
         """Expects a certificate-resource and generates a constant for its sensitive information in hex-format"""
-        self.__generate_constant_from_resource(codeunit_folder, certificate_resource_name, "password", "Password")
-        self.__generate_constant_from_resource(codeunit_folder, certificate_resource_name, "pfx", "PFX")
+        codeunit_name = os.path.basename(codeunit_folder)
+        self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{codeunit_name}.test.local.pfx", "PFX")
+        self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{codeunit_name}.test.local.password", "Password")
+
+    @GeneralUtilities.check_arguments
+    def generate_constant_from_resource_by_filename(self, codeunit_folder: str, resource_name: str, filename: str, constant_name: str):
+        certificate_resource_folder = GeneralUtilities.resolve_relative_path(f"Other/Resources/{resource_name}", codeunit_folder)
+        resource_file = os.path.join(certificate_resource_folder, filename)
+        resource_file_content = GeneralUtilities.read_binary_from_file(resource_file)
+        resource_file_as_hex = resource_file_content.hex()
+        self.set_constant(codeunit_folder, f"{resource_name}{constant_name}Hex", resource_file_as_hex)
 
     @GeneralUtilities.check_arguments
-    def __generate_constant_from_resource(self, codeunit_folder: str, resource_name: str, extension: str, constant_name: str):
+    def generate_constant_from_resource_by_extension(self, codeunit_folder: str, resource_name: str, extension: str, constant_name: str):
         certificate_resource_folder = GeneralUtilities.resolve_relative_path(f"Other/Resources/{resource_name}", codeunit_folder)
         resource_file = self.__sc.find_file_by_extension(certificate_resource_folder, extension)
         resource_file_content = GeneralUtilities.read_binary_from_file(resource_file)
         resource_file_as_hex = resource_file_content.hex()
         self.set_constant(codeunit_folder, f"{resource_name}{constant_name}Hex", resource_file_as_hex)
 
     @GeneralUtilities.check_arguments
@@ -1580,17 +1600,18 @@
         for dependent_codeunit in dependent_codeunits:
             self.__build_codeunit(os.path.join(repo_folder, dependent_codeunit), verbosity, target_environmenttype, additional_arguments_file)
         if 0 < len(dependent_codeunits):
             GeneralUtilities.write_message_to_stdout(f"Finished building dependent codeunits for codeunit {codeunit_name}.")
 
     @GeneralUtilities.check_arguments
     def copy_artifacts_from_dependent_code_units(self, repo_folder: str, codeunit_name: str) -> None:
-        GeneralUtilities.write_message_to_stdout(f"Get dependent artifacts for codeunit {codeunit_name}.")
         codeunit_file = os.path.join(repo_folder, codeunit_name, codeunit_name + ".codeunit.xml")
         dependent_codeunits = self.get_dependent_code_units(codeunit_file)
+        if len(dependent_codeunits) > 0:
+            GeneralUtilities.write_message_to_stdout(f"Get dependent artifacts for codeunit {codeunit_name}.")
         dependent_codeunits_folder = os.path.join(repo_folder, codeunit_name, "Other", "Resources", "DependentCodeUnits")
         GeneralUtilities.ensure_directory_does_not_exist(dependent_codeunits_folder)
         for dependent_codeunit in dependent_codeunits:
             target_folder = os.path.join(dependent_codeunits_folder, dependent_codeunit)
             GeneralUtilities.ensure_directory_does_not_exist(target_folder)
             other_folder = os.path.join(repo_folder, dependent_codeunit, "Other")
             artifacts_folder = os.path.join(other_folder, "Artifacts")
@@ -1625,14 +1646,18 @@
         codeunit_name = os.path.basename(codeunit_folder)
         csproj_file = os.path.join(codeunit_folder, codeunit_name, f"{codeunit_name}.csproj")
         self.__sc.update_dependencies_of_dotnet_project(csproj_file, verbosity)
         test_csproj_file = os.path.join(codeunit_folder, f"{codeunit_name}Tests", f"{codeunit_name}Tests.csproj")
         self.__sc.update_dependencies_of_dotnet_project(test_csproj_file, verbosity)
 
     @GeneralUtilities.check_arguments
+    def update_dependencies_of_typical_node_codeunit(self, update_script_file: str, verbosity: int, cmd_args: list[str]):
+        pass  # TODO
+
+    @GeneralUtilities.check_arguments
     def standardized_tasks_update_version_in_docker_examples(self, file, codeunit_version):
         folder_of_current_file = os.path.dirname(file)
         codeunit_folder = GeneralUtilities.resolve_relative_path("..", folder_of_current_file)
         codeunit_name = os.path.basename(codeunit_folder)
         codeunit_name_lower = codeunit_name.lower()
         examples_folder = GeneralUtilities.resolve_relative_path("Other/Reference/ReferenceContent/Examples", codeunit_folder)
         for example_folder in GeneralUtilities.get_direct_folders_of_folder(examples_folder):
@@ -1671,30 +1696,32 @@
 
     @GeneralUtilities.check_arguments
     def _internal_sort_codenits(self, codeunits=dict[str, set[str]]) -> list[str]:
         return list(TopologicalSorter(codeunits).static_order())
 
     @GeneralUtilities.check_arguments
     def build_codeunit(self, codeunit_folder: str, verbosity: int = 1, target_environmenttype: str = "QualityCheck", additional_arguments_file: str = None,
-                       is_pre_merge: bool = False, export_target_directory: str = None) -> None:
+                       is_pre_merge: bool = False, export_target_directory: str = None, assume_dependent_codeunits_are_already_built: bool = False) -> None:
         codeunit_folder = GeneralUtilities.resolve_relative_path_from_current_working_directory(codeunit_folder)
         codeunit_name = os.path.basename(codeunit_folder)
         repository_folder = os.path.dirname(codeunit_folder)
-        self.build_specific_codeunits(repository_folder, [codeunit_name], verbosity, target_environmenttype, additional_arguments_file, is_pre_merge, export_target_directory)
+        self.build_specific_codeunits(repository_folder, [codeunit_name], verbosity, target_environmenttype, additional_arguments_file,
+                                      is_pre_merge, export_target_directory, assume_dependent_codeunits_are_already_built)
 
     @GeneralUtilities.check_arguments
     def build_codeunits(self, repository_folder: str, verbosity: int = 1, target_environmenttype: str = "QualityCheck", additional_arguments_file: str = None,
                         is_pre_merge: bool = False, export_target_directory: str = None) -> None:
         repository_folder = GeneralUtilities.resolve_relative_path_from_current_working_directory(repository_folder)
         codeunits = self.get_codeunits(repository_folder)
         self.build_specific_codeunits(repository_folder, codeunits, verbosity, target_environmenttype, additional_arguments_file, is_pre_merge, export_target_directory)
 
     @GeneralUtilities.check_arguments
     def build_specific_codeunits(self, repository_folder: str, codeunits: list[str], verbosity: int = 1, target_environmenttype: str = "QualityCheck",
-                                 additional_arguments_file: str = None, is_pre_merge: bool = False, export_target_directory: str = None) -> None:
+                                 additional_arguments_file: str = None, is_pre_merge: bool = False, export_target_directory: str = None,
+                                 assume_dependent_codeunits_are_already_built: bool = True) -> None:
         repository_folder = GeneralUtilities.resolve_relative_path_from_current_working_directory(repository_folder)
         contains_uncommitted_changes = self.__sc.git_repository_has_uncommitted_changes(repository_folder)
         if is_pre_merge and contains_uncommitted_changes:
             raise ValueError(f'Repository "{repository_folder}" has uncommitted changes.')
         subfolders = [os.path.join(repository_folder, codeunit) for codeunit in codeunits]
         codeunits_with_dependent_codeunits: dict[str, set[str]] = dict[str, set[str]]()
         for subfolder in subfolders:
@@ -1715,15 +1742,16 @@
                 for codeunit in sorted_codeunits:
                     i = i+1
                     GeneralUtilities.write_message_to_stdout(f"{i}.: {codeunit}")
             self.__do_repository_checks(repository_folder, project_version)
             line = "----------"
             for codeunit in sorted_codeunits:
                 GeneralUtilities.write_message_to_stdout(line)
-                self.__build_codeunit(os.path.join(repository_folder, codeunit), verbosity, target_environmenttype, additional_arguments_file, is_pre_merge, True)
+                self.__build_codeunit(os.path.join(repository_folder, codeunit), verbosity, target_environmenttype,
+                                      additional_arguments_file, is_pre_merge, assume_dependent_codeunits_are_already_built)
             GeneralUtilities.write_message_to_stdout(line)
         if not contains_uncommitted_changes and self.__sc.git_repository_has_uncommitted_changes(repository_folder) and not is_pre_merge:
             message = f'Due to the build-process the repository "{repository_folder}" has new uncommitted changes.'
             if target_environmenttype == "Development":
                 GeneralUtilities.write_message_to_stdout(message)
             else:
                 raise ValueError(message)
@@ -1794,14 +1822,41 @@
         else:
             if grylibrary_dll_file_exists:
                 GeneralUtilities.write_message_to_stdout("Warning: Can not check for updates of GRYLibrary due to missing internet-connection.")
             else:
                 raise ValueError("Can not download GRYLibrary.")
 
     @GeneralUtilities.check_arguments
+    def ensure_ffmpeg_is_available(self, codeunit_folder: str) -> None:
+        ffmpeg_folder = os.path.join(codeunit_folder, "Other", "Resources", "FFMPEG")
+        internet_connection_is_available = GeneralUtilities.internet_connection_is_available()
+        exe_file = f"{ffmpeg_folder}/ffmpeg.exe"
+        exe_file_exists = os.path.isfile(exe_file)
+        if internet_connection_is_available:  # Load/Update
+            GeneralUtilities.ensure_directory_does_not_exist(ffmpeg_folder)
+            GeneralUtilities.ensure_directory_exists(ffmpeg_folder)
+            ffmpeg_temp_folder = ffmpeg_folder+"Temp"
+            GeneralUtilities.ensure_directory_does_not_exist(ffmpeg_temp_folder)
+            GeneralUtilities.ensure_directory_exists(ffmpeg_temp_folder)
+            zip_file_on_disk = os.path.join(ffmpeg_temp_folder, "ffmpeg.zip")
+            original_zip_filename = "ffmpeg-master-latest-win64-gpl-shared"
+            zip_link = f"https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/{original_zip_filename}.zip"
+            urllib.request.urlretrieve(zip_link, zip_file_on_disk)
+            shutil.unpack_archive(zip_file_on_disk, ffmpeg_temp_folder)
+            bin_folder_source = os.path.join(ffmpeg_temp_folder, "ffmpeg-master-latest-win64-gpl-shared/bin")
+            bin_folder_target = ffmpeg_folder
+            GeneralUtilities.copy_content_of_folder(bin_folder_source, bin_folder_target)
+            GeneralUtilities.ensure_directory_does_not_exist(ffmpeg_temp_folder)
+        else:
+            if exe_file_exists:
+                GeneralUtilities.write_message_to_stdout("Warning: Can not check for updates of FFMPEG due to missing internet-connection.")
+            else:
+                raise ValueError("Can not download FFMPEG.")
+
+    @GeneralUtilities.check_arguments
     def __ensure_plant_uml_is_available(self, codeunit_folder: str) -> None:
         plant_uml_folder = os.path.join(codeunit_folder, "Other", "Resources", "PlantUML")
         internet_connection_is_available = GeneralUtilities.internet_connection_is_available()
         jar_file = f"{plant_uml_folder}/plantuml.jar"
         plantuml_jar_file_exists = os.path.isfile(jar_file)
         if internet_connection_is_available:  # Load/Update PlantUML
             GeneralUtilities.ensure_directory_does_not_exist(plant_uml_folder)
```

## Comparing `ScriptCollection-3.4.0.dist-info/METADATA` & `ScriptCollection-3.4.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.4.0
+Version: 3.4.1
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
```

## Comparing `ScriptCollection-3.4.0.dist-info/entry_points.txt` & `ScriptCollection-3.4.1.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.4.0.dist-info/RECORD` & `ScriptCollection-3.4.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-ScriptCollection/Executables.py,sha256=8uVVxyXrndRwTVxcL1rRlbyzaP6ZYvzxj41f7sy6L90,18794
+ScriptCollection/Executables.py,sha256=BanfD3ls0ov3ECnsbuyzNstdYjqz_HplreQYJxrB8Ag,19068
 ScriptCollection/GeneralUtilities.py,sha256=vZDiW5lWJRCrIZVs1bTCZ-O5slQnM5dv4GcJ-RTMowY,34378
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=nIzY4dG6W-xEpkeoTbozwNZtFSIo-bU_W6t6u1AZKtE,6275
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=6MoxE0Xrj1SKZzqCZ9bU6tUUlogYGaPkIkbsxhy2pJw,95771
-ScriptCollection/TasksForCommonProjectStructure.py,sha256=1VUPMfK3EWKydgUplqujzlH7ZKZgX3CgFvnVjOoc2Ds,139730
+ScriptCollection/ScriptCollectionCore.py,sha256=fGgSe24439rYvBd1iDNq3QniX3pzI319Jxy9K9FAGuo,96083
+ScriptCollection/TasksForCommonProjectStructure.py,sha256=b_QoN7vu_F6IxVy6RzzObjhs5mu9EE3VEKRG6NeLu-0,144026
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.4.0.dist-info/METADATA,sha256=S-qHlKVq3dAMCTvoDw4aDUHSHto1vxkyqwE2E2qQe7U,7649
-ScriptCollection-3.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ScriptCollection-3.4.0.dist-info/entry_points.txt,sha256=dJKdWcH41owxlKx_khj4P7DItr9lhxWP9JU2Dq8GSsQ,2088
-ScriptCollection-3.4.0.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.4.0.dist-info/RECORD,,
+ScriptCollection-3.4.1.dist-info/METADATA,sha256=XkqpMqaZjnWku2gkdcPlwesxWShk9aNNgbPXJo5L2zc,7649
+ScriptCollection-3.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ScriptCollection-3.4.1.dist-info/entry_points.txt,sha256=dJKdWcH41owxlKx_khj4P7DItr9lhxWP9JU2Dq8GSsQ,2088
+ScriptCollection-3.4.1.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.4.1.dist-info/RECORD,,
```

