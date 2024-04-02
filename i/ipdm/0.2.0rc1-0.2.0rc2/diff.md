# Comparing `tmp/ipdm-0.2.0rc1.tar.gz` & `tmp/ipdm-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipdm-0.2.0rc1.tar", last modified: Mon Apr  1 07:22:57 2024, max compression
+gzip compressed data, was "ipdm-0.2.0rc2.tar", last modified: Tue Apr  2 12:17:25 2024, max compression
```

## Comparing `ipdm-0.2.0rc1.tar` & `ipdm-0.2.0rc2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       27 2024-04-01 07:22:39.388066 ipdm-0.2.0rc1/README.md
--rw-r--r--   0        0        0      689 2024-04-01 07:22:57.704041 ipdm-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0      246 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/__init__.py
--rw-r--r--   0        0        0     5811 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/__main__.py
--rw-r--r--   0        0        0    21466 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/api.py
--rw-r--r--   0        0        0    18438 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/const.py
--rw-r--r--   0        0        0     1214 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/exceptions.py
--rw-r--r--   0        0        0     1593 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/logging.py
--rw-r--r--   0        0        0        0 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/models/__init__.py
--rw-r--r--   0        0        0     4753 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/models/index.py
--rw-r--r--   0        0        0     6681 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/models/ipk.py
--rw-r--r--   0        0        0     6226 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/models/lock.py
--rw-r--r--   0        0        0     2939 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/models/requirement.py
--rw-r--r--   0        0        0        0 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/project/__init__.py
--rw-r--r--   0        0        0      473 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/project/env.py
--rw-r--r--   0        0        0     6509 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/project/toml_file.py
--rw-r--r--   0        0        0      404 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/typing.py
--rw-r--r--   0        0        0        0 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/utils/__init__.py
--rw-r--r--   0        0        0     1230 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/utils/_freeze.py
--rw-r--r--   0        0        0     3210 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/utils/freeze.py
--rw-r--r--   0        0        0      768 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/utils/git.py
--rw-r--r--   0        0        0      486 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/utils/hash.py
--rw-r--r--   0        0        0     1615 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/utils/loader.py
--rw-r--r--   0        0        0      997 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/utils/resolve.py
--rw-r--r--   0        0        0      160 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/utils/urlparser.py
--rw-r--r--   0        0        0       70 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/utils/uuid.py
--rw-r--r--   0        0        0     1648 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/src/ipm/utils/version.py
--rw-r--r--   0        0        0        0 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/tests/__init__.py
--rw-r--r--   0        0        0      491 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/tests/test_api.py
--rw-r--r--   0        0        0     2601 2024-04-01 07:22:39.392066 ipdm-0.2.0rc1/tests/test_cli.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 ipdm-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       27 2024-04-02 12:17:07.841571 ipdm-0.2.0rc2/README.md
+-rw-r--r--   0        0        0      689 2024-04-02 12:17:25.841590 ipdm-0.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      246 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/__init__.py
+-rw-r--r--   0        0        0     5958 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/__main__.py
+-rw-r--r--   0        0        0    23305 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/api.py
+-rw-r--r--   0        0        0    18438 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/const.py
+-rw-r--r--   0        0        0     1214 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/exceptions.py
+-rw-r--r--   0        0        0     1595 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/logging.py
+-rw-r--r--   0        0        0        0 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/models/__init__.py
+-rw-r--r--   0        0        0     4753 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/models/index.py
+-rw-r--r--   0        0        0     6688 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/models/ipk.py
+-rw-r--r--   0        0        0     5591 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/models/lock.py
+-rw-r--r--   0        0        0     3516 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/models/requirement.py
+-rw-r--r--   0        0        0        0 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/project/__init__.py
+-rw-r--r--   0        0        0      473 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/project/env.py
+-rw-r--r--   0        0        0     6509 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/project/toml_file.py
+-rw-r--r--   0        0        0      404 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/typing.py
+-rw-r--r--   0        0        0        0 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/__init__.py
+-rw-r--r--   0        0        0     1230 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/_freeze.py
+-rw-r--r--   0        0        0     2495 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/freeze.py
+-rw-r--r--   0        0        0      768 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/git.py
+-rw-r--r--   0        0        0      486 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/hash.py
+-rw-r--r--   0        0        0     1615 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/loader.py
+-rw-r--r--   0        0        0      997 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/resolve.py
+-rw-r--r--   0        0        0      160 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/urlparser.py
+-rw-r--r--   0        0        0       70 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/uuid.py
+-rw-r--r--   0        0        0     1648 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/src/ipm/utils/version.py
+-rw-r--r--   0        0        0        0 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0      491 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/tests/test_api.py
+-rw-r--r--   0        0        0     2601 2024-04-02 12:17:07.845571 ipdm-0.2.0rc2/tests/test_cli.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 ipdm-0.2.0rc2/PKG-INFO
```

### Comparing `ipdm-0.2.0rc1/pyproject.toml` & `ipdm-0.2.0rc2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ipdm"
-version = "0.2.0-rc.1"
+version = "0.2.0-rc.2"
 description = "Infini 包管理器"
 authors = [
     { name = "苏向夜", email = "fu050409@163.com" },
     { name = "简律纯", email = "leader@hydroroll.team" },
 ]
 dependencies = [
     "typer>=0.9.0",
```

### Comparing `ipdm-0.2.0rc1/src/ipm/__main__.py` & `ipdm-0.2.0rc2/src/ipm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,21 @@
         error(str(err), echo=True)
     finally:
         status.stop()
 
 
 @main.command()
 def update():
-    """更新 Infini 依赖"""
-    raise NotImplementedError
+    """更新规则包依赖"""
+    try:
+        if api.update(Path.cwd(), echo=True):
+            tada()
+    except IPMException as err:
+        error(str(err), echo=True)
+    finally:
+        status.stop()
 
 
 main.add_typer(yggdrasil)
 
 if __name__ == "__main__":
     main()
```

### Comparing `ipdm-0.2.0rc1/src/ipm/api.py` & `ipdm-0.2.0rc2/src/ipm/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from datetime import datetime
 from pathlib import Path
+from distlib.version import SemanticVersion
 from typing import Optional
 
 from ipm.const import INDEX, VUE_CODE
 from ipm.models.lock import PackageLock, ProjectLock
 from ipm.project.env import new_virtualenv
 from ipm.project.toml_file import (
     add_yggdrasil,
     init_infini,
     init_pyproject,
     remove_yggdrasil,
 )
 from ipm.typing import StrPath
 from ipm.utils import freeze, loader
 from ipm.utils.git import get_user_name_email, git_init, git_tag
-from ipm.logging import confirm, status, update, info, success, warning, error, ask
+from ipm.logging import confirm, status, statusup, info, success, warning, error, ask
 from ipm.exceptions import (
     EnvironmentError,
     ProjectError,
     TomlLoadFailed,
     FileNotFoundError,
     NameError,
     RuntimeError,
 )
-from ipm.models.ipk import InfiniProject, InfiniFrozenPackage
+from ipm.models.ipk import InfiniProject
 from ipm.models.index import Yggdrasil
 
 from infini.loader import Loader
 
 import shutil
 import sys
 import re
@@ -36,43 +37,43 @@
 import tomlkit
 import json
 
 
 def lock(target_path: StrPath, echo: bool = False) -> bool:
     info("生成项目锁...", echo)
 
-    update("检查环境中...", echo)
+    statusup("检查环境中...", echo)
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
     project = InfiniProject(toml_path.parent)
     success("环境检查完毕.", echo)
 
-    update("写入依赖锁文件...", echo)
+    statusup("写入依赖锁文件...", echo)
     lock = ProjectLock.init_from_project(project)
     lock.dump()
     success("项目依赖锁写入完成.", echo)
     return True
 
 
 def check(target_path: StrPath, echo: bool = False) -> bool:
     info("检查项目环境...", echo)
-    update("检查基础环境中...", echo)
+    statusup("检查基础环境中...", echo)
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
     project = InfiniProject(toml_path.parent)
     success("环境检查完毕.", echo)
 
-    update("同步世界树中...", echo)
+    statusup("同步世界树中...", echo)
     global_lock = PackageLock()
     for index in project.yggdrasils.values():
-        update(f"同步世界树: [green]{index}[/]...", echo)
+        statusup(f"同步世界树: [green]{index}[/]...", echo)
         if not (yggdrasil := global_lock.get_yggdrasil_by_index(index)):
             Yggdrasil.init(index)
         else:
             yggdrasil.sync()
         success(f"世界树 [green]{index}[/] 同步完毕.", echo)
 
     if not lock(target_path, echo=echo):
@@ -81,15 +82,15 @@
     return True
 
 
 def tag(target_path: StrPath, tag: str, echo: bool = False):
     info(f"更新规则包版本号为: [bold green]{tag}[/]", echo)
     tag = tag.lstrip("v")
 
-    update("检查环境中...", echo)
+    statusup("检查环境中...", echo)
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
     if not (project_path := Path(target_path).joinpath("pyproject.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]pyproject.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
@@ -107,24 +108,24 @@
     tomlkit.dump(py_project, project_file)
     toml_file.close()
     project_file.close()
 
     success("项目文件写入完成.", echo)
 
     if toml_path.parent.joinpath(".git").is_dir():
-        update("处理 Git 标签中...", echo)
+        statusup("处理 Git 标签中...", echo)
         git_tag(toml_path.parent, tag)
         success(f"标签 [bold green]{tag}[/] 已写入.", echo)
 
     return True
 
 
 def init(target_path: StrPath, force: bool = False, echo: bool = False) -> bool:
     info("初始化规则包...", echo)
-    update("检查环境...", echo)
+    statusup("检查环境...", echo)
     target_path = Path(target_path).resolve()
     if (toml_path := (target_path / "infini.toml")).exists() and not force:
         warning(
             f"无法在已经初始化的地址重新初始化, 如果你的确希望重新初始化, 请使用[bold red]`ipm init --force`[/bold red].",
             echo,
         )
         return False
@@ -154,15 +155,15 @@
 
     standalone = confirm("对项目进行分发?", default=True) if echo else True
     init_git = confirm("初始化 Git 仓库?", default=True) if echo else True
     init_virtualenv = confirm("创建虚拟环境?", default=True) if echo else False
     sync_now = confirm("立刻同步环境?", default=True) if echo else False
 
     status.start()
-    update("构建环境中...", echo)
+    statusup("构建环境中...", echo)
 
     init_infini(
         toml_path=toml_path,
         target_path=target_path,
         name=name,
         version=version,
         description=description,
@@ -203,15 +204,15 @@
 
     return True
 
 
 def new(dist_path: StrPath, echo: bool = False) -> bool:
     info("新建规则包...", echo)
 
-    update("检查环境...", echo)
+    statusup("检查环境...", echo)
     path = Path(dist_path).resolve()
     if path.exists():
         warning(
             f"路径 [blue]{path.relative_to(Path('.').resolve())}[/blue] 已经存在.", echo
         )
         return False
     path.mkdir(parents=True, exist_ok=True)
@@ -220,29 +221,37 @@
     if not init(path, echo=echo):
         return False
 
     success(f"规则包 [bold green]{path.name}[/bold green] 新建完成!", echo)
     return True
 
 
-def build(target_path: StrPath, echo: bool = False) -> Optional[InfiniFrozenPackage]:
+def build(target_path: StrPath, echo: bool = False) -> bool:
     info("构建规则包...", echo)
-    update("检查构建环境...", echo)
+    statusup("检查构建环境...", echo)
 
     if not (Path(target_path).resolve() / "infini.toml").exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
 
     try:
         ipk = InfiniProject(target_path)
     except TomlLoadFailed as e:
-        return error(f"环境存在异常: {e}", echo)
+        error(f"环境存在异常: {e}", echo)
+        return False
 
-    return freeze.build_ipk(ipk, echo)
+    update("开始构建规则包...", echo)
+    ifp = freeze.build_ipk(ipk)
+    success(f"文件 SHA256 值为 [purple]{ifp.hash}[/purple].", echo)
+    success(
+        f"包 [bold green]{ifp.name}[/bold green] [yellow]{ifp.version}[/yellow] 构建成功.",
+        echo,
+    )
+    return True
 
 
 def extract(
     source_path: StrPath,
     hash: Optional[str] = None,
     dist_path: Optional[StrPath] = None,
     echo: bool = False,
@@ -255,30 +264,30 @@
     return True
 
 
 def yggdrasil_add(
     target_path: StrPath, name: str, index: str, echo: bool = False
 ) -> bool:
     info(f"新增世界树: [bold green]{name}[/]", echo)
-    update("检查环境中...", echo)
+    statusup("检查环境中...", echo)
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
     success("环境检查完毕.", echo)
-    update("同步世界树中...", echo)
+    statusup("同步世界树中...", echo)
     Yggdrasil.init(index)
     add_yggdrasil(toml_path, name, index)
     success("更改均已写入文件.", echo)
     return True
 
 
 def yggdrasil_remove(target_path: StrPath, name: str, echo: bool = False) -> bool:
     info(f"新增世界树: [bold green]{name}[/]", echo)
-    update("检查环境中...", echo)
+    statusup("检查环境中...", echo)
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
     project = InfiniProject(toml_path.parent)
     success("环境检查完毕.", echo)
     remove_yggdrasil(project, name)
@@ -292,24 +301,24 @@
     *,
     path: Optional[str] = None,
     yggdrasil: Optional[str] = None,
     index: Optional[str] = None,
     echo: bool = False,
 ) -> bool:
     info(f"新增规则包依赖: [bold green]{name}[/bold green]", echo)
-    update("检查环境中...", echo)
+    statusup("检查环境中...", echo)
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
     project = InfiniProject(toml_path.parent)
     global_lock = PackageLock()
     success("环境检查完毕.", echo)
 
-    update("检查世界树中...", echo)
+    statusup("检查世界树中...", echo)
     ygd = (
         Yggdrasil.init(index or INDEX)
         if not global_lock.has_index(index or INDEX)
         else global_lock.get_yggdrasil_by_index(index or INDEX)
     )
     if not ygd:
         raise ProjectError("世界树检查失败！")
@@ -323,15 +332,15 @@
         version = ygd.get_lastest_version(name)
 
     if not version:
         raise ProjectError(f"无法找到一个匹配 [red]{name}[/] 的版本。")
 
     check(target_path, echo=echo)
 
-    update("处理 Infini 项目依赖锁...", echo)
+    statusup("处理 Infini 项目依赖锁...", echo)
     project.require(
         name,
         version=version,
         path=path,
         yggdrasil=yggdrasil,
         index=index,
     )
@@ -342,27 +351,27 @@
 
     success("规则包依赖新增完成.", echo)
     return True
 
 
 def unrequire(target_path: StrPath, name: str, echo: bool = False):
     info(f"删除规则包依赖: [bold green]{name}[/bold green]", echo)
-    update("处理 Infini 项目依赖锁...", echo)
+    statusup("处理 Infini 项目依赖锁...", echo)
     project = InfiniProject()
     project.unrequire(name)
     project.dump()
     success("项目文件写入完成.", echo)
     check(target_path, echo=echo)
     success("规则包依赖删除完成.", echo)
     return True
 
 
 def add(target_path, name: str, echo: bool = False) -> bool:
     info(f"新增环境依赖项: [bold green]{name}[/bold green]", echo)
-    update("检查环境中...", echo)
+    statusup("检查环境中...", echo)
     if not (
         match := re.match(r"^((?:[a-zA-Z_-]|\d)+)(?:([>=<]+\d+(?:[.]\d+)*))?$", name)
     ):
         raise NameError(f"版本号 [bold red]{name}[/] 不合法.")
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
@@ -371,15 +380,15 @@
     if not shutil.which("pdm"):
         raise EnvironmentError(
             "IPM 未能在环境中找到 [bold green]PDM[/] 安装, 请确保 PDM 在环境中被正确安装. "
             "你可以使用`[bold green]pipx install pdm[/]`来安装此包管理器."
         )
     success("环境检查完毕.", echo)
 
-    update("安装依赖中...", echo)
+    statusup("安装依赖中...", echo)
 
     name = match.group(1)
     version = match.group(2)
     project.add(name, version or "*")
     if (
         result := subprocess.run(
             ["pdm", "add", name],
@@ -394,15 +403,15 @@
     project.dump()
     success("项目文件写入完成.", echo)
     return True
 
 
 def remove(target_path: StrPath, name: str, echo: bool = False):
     info(f"删除环境依赖项: [bold green]{name}[/bold green]", echo)
-    update("检查环境中...", echo)
+    statusup("检查环境中...", echo)
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
     project = InfiniProject(toml_path.parent)
     if not shutil.which("pdm"):
         raise EnvironmentError(
@@ -426,15 +435,15 @@
     project.dump()
     success("项目文件写入完成.", echo)
     return True
 
 
 def sync(target_path: StrPath, echo: bool = False) -> bool:
     info(f"同步依赖环境...", echo)
-    update("检查环境中...", echo)
+    statusup("检查环境中...", echo)
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
     project = InfiniProject(toml_path.parent)
     lock = ProjectLock(target_path)
     if not lock._lock_path.exists():
@@ -445,21 +454,21 @@
     if not shutil.which("pdm"):
         raise EnvironmentError(
             "IPM 未能在环境中找到 [bold green]PDM[/] 安装, 请确保 PDM 在环境中被正确安装. "
             "你可以使用`[bold green]pipx install pdm[/]`来安装此包管理器."
         )
     success("环境检查完毕.", echo)
 
-    update("同步依赖环境中...", echo)
+    statusup("同步依赖环境中...", echo)
     for requirement in lock.requirements:
         if not requirement.is_local():
             if global_lock.has_frozen_package(requirement.name, requirement.version):
                 continue
-            update(
-                f"下载 [bold green]{requirement.name}=={requirement.version}[/]...",
+            statusup(
+                f"下载 [bold green]{requirement.name}[/] [bold yellow]{requirement.version}[/]...",
                 echo,
             )
             ifp = loader.load_from_remote(
                 requirement.name,
                 requirement.yggdrasil.index.rstrip("/") + (requirement.url or ""),
                 requirement.hash or "",
             )
@@ -470,23 +479,23 @@
                 requirement.yggdrasil.index,
                 str(ifp._source_path),
             )
             success(
                 f"[bold green]{requirement.name} {requirement.version}[/] 安装完成！",
                 echo,
             )
-    update("同步依赖环境中...", echo)
+    statusup("同步依赖环境中...", echo)
     dependencies = []
     for name, version in project.dependencies.items():
         if version == "*":
             dependencies.append(name)
         else:
             dependencies.append(f"{name}{version}")
     if dependencies:
-        update(
+        statusup(
             "安装依赖: "
             + ", ".join(
                 ["[bold green]" + dependency + "[/]" for dependency in dependencies]
             )
             + "...",
             echo,
         )
@@ -506,15 +515,15 @@
 
     success("依赖环境同步完毕！", echo)
     return True
 
 
 def install(target_path: StrPath, echo: bool = False) -> bool:
     info("安装规则包环境中...", echo)
-    update("检查环境中...", echo)
+    statusup("检查环境中...", echo)
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
     project = InfiniProject(toml_path.parent)
     global_lock = PackageLock()
     if not shutil.which("pdm"):
@@ -523,15 +532,15 @@
             "你可以使用`[bold green]pipx install pdm[/]`来安装此包管理器."
         )
     success("环境检查完毕.", echo)
 
     check(target_path, echo)
     sync(target_path, echo)
 
-    update("安装依赖中...", echo)
+    statusup("安装依赖中...", echo)
     lock = ProjectLock(target_path)
     packages_path = toml_path.parent.joinpath("packages")
     packages_path.mkdir(parents=True, exist_ok=True)
     ProjectLock.init_from_project(project, packages_path)
     for requirement in lock.requirements:
         try:
             prj = InfiniProject(packages_path.joinpath(requirement.name))
@@ -561,15 +570,15 @@
     submodule: bool = False,
     echo: bool = False,
 ) -> bool:
     info("构建项目文档...", echo)
     if type.lower() != "vue":
         raise EnvironmentError("目前仅支持 Vue 部署！")
 
-    update("准备环境中...", echo)
+    statusup("准备环境中...", echo)
     if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
         raise FileNotFoundError(
             f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
         )
     if not submodule and not shutil.which("npm"):
         raise EnvironmentError(
             "IPM 未能在环境中找到 [bold green]Node.js[/] 安装, 请确保 NPM 在环境中被正确安装. "
@@ -595,7 +604,41 @@
         docs["readme"] = project.readme
         docs["doc_create_at"] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         dist_path.joinpath("index.json").write_text(json.dumps(docs), encoding="utf-8")
         dist_path.joinpath("index.vue").write_text(VUE_CODE, encoding="utf-8")
     else:
         raise ProjectError("未被支持。")
     return True
+
+
+def update(target_path: StrPath, echo: bool = False) -> bool:
+    info("更新依赖环境...", echo)
+    statusup("检查环境中...", echo)
+    if not (toml_path := Path(target_path).joinpath("infini.toml")).exists():
+        raise FileNotFoundError(
+            f"文件 [green]infini.toml[/green] 尚未被初始化, 你可以使用[bold green]`ipm init`[/bold green]来初始化项目."
+        )
+    project = InfiniProject(toml_path.parent)
+    if not shutil.which("pdm"):
+        raise EnvironmentError(
+            "IPM 未能在环境中找到 [bold green]PDM[/] 安装, 请确保 PDM 在环境中被正确安装. "
+            "你可以使用`[bold green]pipx install pdm[/]`来安装此包管理器."
+        )
+    success("环境检查完毕.", echo)
+
+    statusup("更新依赖中...", echo)
+    for requirement in project.requirements:
+        lastest_version = requirement.yggdrasil.get_lastest_version(requirement.name)
+        if not lastest_version:
+            raise ProjectError(f"包 [bold red]{requirement.name}[/] 被从世界树燃烧了。")
+        if SemanticVersion(lastest_version) > SemanticVersion(requirement.version):
+            project.require(requirement.name, version=lastest_version)
+            success(
+                f"将 [bold green]{requirement.version}[/] 升级到 [bold yellow]{lastest_version}[/].",
+                echo,
+            )
+
+    check(target_path, echo)
+    sync(target_path, echo)
+
+    install(target_path, echo)
+    return True
```

### Comparing `ipdm-0.2.0rc1/src/ipm/const.py` & `ipdm-0.2.0rc2/src/ipm/const.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc1/src/ipm/exceptions.py` & `ipdm-0.2.0rc2/src/ipm/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc1/src/ipm/logging.py` & `ipdm-0.2.0rc2/src/ipm/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from rich.prompt import Confirm, Prompt
 from .typing import List, Any
 
 console = Console()
 status = console.status("")
 
 
-def update(message: str, echo: bool = False) -> None:
+def statusup(message: str, echo: bool = False) -> None:
     return status.update(message) if echo else status.stop()
 
 
 def info(message: str, echo: bool = False) -> None:
     return console.print(message) if echo else None
```

### Comparing `ipdm-0.2.0rc1/src/ipm/models/index.py` & `ipdm-0.2.0rc2/src/ipm/models/index.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc1/src/ipm/models/ipk.py` & `ipdm-0.2.0rc2/src/ipm/models/ipk.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     @property
     def dependencies(self) -> Dict[str, str]:
         return self._data.unwrap().get("dependencies", {})
 
     @property
     def requirements(self) -> Requirements:
         return Requirements(
-            self._data.get("requirements") or {},
+            self._data.unwrap().get("requirements", {}),
             yggdrasils={
                 name: global_lock.get_yggdrasil_by_index(url)
                 for name, url in self.yggdrasils.items()
             },
         )
 
     @property
```

### Comparing `ipdm-0.2.0rc1/src/ipm/models/lock.py` & `ipdm-0.2.0rc2/src/ipm/models/lock.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import tomlkit
 
 
 if TYPE_CHECKING:
     from ipm.models import ipk
     from ipm.models.index import Yggdrasil
-    from ipm.models.ipk import InfiniFrozenPackage
 
 
 class IPMLock(metaclass=ABCMeta):
     """IPM 锁基类"""
 
     _lock_path: Path
     metadata: Dict[str, str]
@@ -149,34 +148,17 @@
         lock._data.add("metadata", metadata)
 
         packages = tomlkit.aot()
         requirements = get_requirements_by_project(project)
 
         for requirement in requirements:
             if requirement.is_local():
-                packages.append(
-                    tomlkit.item(
-                        {
-                            "name": requirement.name,
-                            "version": requirement.version,
-                            "path": requirement.path,
-                        }
-                    )
-                )
+                packages.append(tomlkit.item(requirement.as_dict()))
             else:
-                packages.append(
-                    tomlkit.item(
-                        {
-                            "name": requirement.name,
-                            "version": requirement.version,
-                            "yggdrasil": requirement.yggdrasil.index,
-                            "url": requirement.url,
-                        }
-                    )
-                )
+                packages.append(tomlkit.item(requirement.as_dict()))
         lock._data.add("package", packages)
 
         return lock
 
     @property
     def requirements(self) -> List[Requirement]:
         from ipm.models.lock import PackageLock
```

### Comparing `ipdm-0.2.0rc1/src/ipm/models/requirement.py` & `ipdm-0.2.0rc2/src/ipm/models/requirement.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,27 +28,46 @@
         yggdrasil = yggdrasil or global_lock.get_yggdrasil_by_index(INDEX)
         if not yggdrasil:
             raise ProjectError("未能找到任何世界树地址，请先添加一个世界树地址。")
         self.name = name
         self.version = version
         self.path = path
         self.url = url or yggdrasil.get_url(name, version)
+        if not self.url:
+            raise ProjectError(
+                f"规则包 [bold red]{name}[/] 不存在版本 [bold yellow]{version}[/]"
+            )
         self.yggdrasil = yggdrasil
         self.hash = hash
 
     def __eq__(self, __value: "Requirement") -> bool:
         return (
             __value.name == self.name
             and __value.version == self.version
             and __value.yggdrasil.index == self.yggdrasil.index
         )
 
     def is_local(self) -> bool:
         return bool(self.path)
 
+    def as_dict(self) -> dict:
+        if self.is_local():
+            return {
+                "name": self.name,
+                "version": self.version,
+                "path": self.path,
+            }
+        else:
+            return {
+                "name": self.name,
+                "version": self.version,
+                "yggdrasil": self.yggdrasil.index,
+                "url": self.url,
+            }
+
 
 class Requirements(List[Requirement]):
     def __init__(
         self,
         requirements: Dict[str, Union[Dict, str]],
         yggdrasils: Optional[Dict[str, Optional[Yggdrasil]]] = None,
     ) -> None:
```

### Comparing `ipdm-0.2.0rc1/src/ipm/project/toml_file.py` & `ipdm-0.2.0rc2/src/ipm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc1/src/ipm/utils/_freeze.py` & `ipdm-0.2.0rc2/src/ipm/utils/_freeze.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc1/src/ipm/utils/freeze.py` & `ipdm-0.2.0rc2/src/ipm/utils/freeze.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,53 @@
 from pathlib import Path
 from typing import Optional
 from ipm.exceptions import FileNotFoundError, VerifyFailed
 from ipm.models.ipk import InfiniProject, InfiniFrozenPackage
 from ipm.typing import StrPath
-from ipm.logging import update, info, success, error
-from ipm.utils.hash import ifp_hash, ifp_verify
+from ipm.utils.hash import ifp_verify
 from ipm.utils import _freeze
 
 import tempfile
 import shutil
 
 
-def build_ipk(ipk: InfiniProject, echo: bool = False) -> InfiniFrozenPackage:
-    update("构建开发环境...", echo)
-
+def build_ipk(ipk: InfiniProject) -> InfiniFrozenPackage:
     arcname = f"{ipk.name}-{ipk.version}"
     build_dir = ipk._source_path.joinpath(".ipm-build")
+    build_dir.joinpath(".gitignore").write_text("*\n")
     arc_dir = build_dir.joinpath(arcname)
     src_path = ipk._source_path / "src"
     dist_path = ipk._source_path / "dist"
     ifp_path = dist_path.joinpath(ipk.default_name + ".ipk")
 
     if not ipk._source_path.exists():
         raise FileNotFoundError(
             f"文件或文件夹 [blue]{ipk._source_path.resolve()}[/blue]]不存在!"
         )
     if build_dir.exists() or dist_path.exists():
-        update("清理构建环境...")
         shutil.rmtree(build_dir, ignore_errors=True)
         shutil.rmtree(dist_path, ignore_errors=True)
-        success("构建环境清理完毕.")
 
     dist_path.mkdir(parents=True, exist_ok=True)
     arc_dir.mkdir(parents=True, exist_ok=True)
-    success("开发环境构建完毕.", echo)
 
-    update("复制工程文件...", echo)
     shutil.copytree(src_path, arc_dir.joinpath("src"))
     shutil.copy2(ipk._source_path / "infini.toml", arc_dir / "infini.toml")
     shutil.copy2(
         ipk._source_path.joinpath("pyproject.toml"), arc_dir.joinpath("pyproject.toml")
     )
     shutil.copy2(
         ipk._source_path.joinpath(ipk.readme_file), arc_dir.joinpath(ipk.readme_file)
     )
-    success("工程文件复制完毕.", echo)
 
-    update("打包 [bold green]ipk[/bold green]文件...", echo)
     _freeze.create_tar_gz(
         str(build_dir),
         str(ifp_path),
     )
     shutil.copy2(ifp_path, dist_path.joinpath(ipk.default_name + ".tar.gz"))
-    success(f"打包文件已存至 [blue]{ifp_path}[/blue].", echo)
-
-    update("创建 SHA256 验证文件...", echo)
-    hash_bytes = ifp_hash(ifp_path)
-    info(f"文件 SHA256 值为 [purple]{hash_bytes}[/purple].", echo)
-
-    success(
-        f"包 [bold green]{ipk.name}[/bold green] [yellow]{ipk.version}[/yellow] 构建成功.",
-        echo,
-    )
 
     return InfiniFrozenPackage(ifp_path, ipk.name, version=ipk.version)
 
 
 def extract_ipk(
     source_path: StrPath,
     dist_path: StrPath,
```

### Comparing `ipdm-0.2.0rc1/src/ipm/utils/git.py` & `ipdm-0.2.0rc2/src/ipm/utils/git.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc1/src/ipm/utils/loader.py` & `ipdm-0.2.0rc2/src/ipm/utils/loader.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc1/src/ipm/utils/resolve.py` & `ipdm-0.2.0rc2/src/ipm/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc1/src/ipm/utils/version.py` & `ipdm-0.2.0rc2/src/ipm/utils/version.py`

 * *Files identical despite different names*

### Comparing `ipdm-0.2.0rc1/tests/test_cli.py` & `ipdm-0.2.0rc2/tests/test_cli.py`

 * *Files identical despite different names*

