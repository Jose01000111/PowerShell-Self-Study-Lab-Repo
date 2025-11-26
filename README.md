# 🔍 PowerShell Self-Study & Lab Repo ⚡

Welcome to my **PowerShell Self-Study Repository**.  
This repo contains **personal notes, lab exercises, and example scripts** to build skills from beginner to advanced PowerShell.  
Everything is structured for **hands-on learning** and **practical use**.

**Study Advice:**  
- 🛠️ Learn by doing — experiment and run commands.  
- 🏗️ Start simple and progress to advanced scripts.  
- 📝 Document useful commands and concepts.  
- 💡 Use lab exercises to reinforce learning.

---

## 1.0 PowerShell Basics (Beginner) 🐣

| Objective | Description | Notes | Labbing | File |
|----------|-------------|-------|---------|------|
| 🖥️ PowerShell Interface | Overview of consoles and editors | Console, ISE, VS Code; Execution policy with `Set-ExecutionPolicy` | Open PowerShell, check version `$PSVersionTable`; navigate directories `Get-ChildItem`, `Set-Location`; run `Get-Process`, `Get-Service` | `BasicNavigation.ps1` |
| 📜 Cmdlets Overview | Built-in commands in Verb-Noun format | Use `Get-Help` for documentation, `Get-Command` to list cmdlets | List cmdlets containing "service"; get help for `Get-Service` | `CmdletsOverview.ps1` |
| 💾 Variables | Storing data for reuse | `$variableName = value`; types: string, int, array, hashtable; scope: local, global, script | Create variables of different types; output and manipulate values | `VariablesLab.ps1` |
| 🔗 Pipelines & Output | Passing objects between commands | `|` operator; `Format-Table`, `Format-List`, `Select-Object` | Pipe `Get-Process | Sort-Object CPU -Descending | Select-Object -First 5`; format output | `PipelinesLab.ps1` |

---

## 2.0 Operators & Expressions ⚙️

| Objective | Description | Notes | Labbing | File |
|----------|-------------|-------|---------|------|
| ⚖️ Comparison Operators | Compare values | `-eq`, `-ne`, `-gt`, `-lt`, `-ge`, `-le`, `-like`, `-match` | Compare integers and strings; filter process names using `-like` | `ComparisonOperators.ps1` |
| 🔀 Logical Operators | Combine multiple conditions | `-and`, `-or`, `-not`; use in `if` or `Where-Object` | Filter processes with multiple conditions; create script checking multiple criteria | `LogicalOperators.ps1` |
| ➕ Arithmetic Operators | Perform calculations | `+`, `-`, `*`, `/`, `%`; supports numbers, strings, arrays | Perform math operations and assign results; concatenate strings with `+` | `ArithmeticOperators.ps1` |

---

## 3.0 Objects & Data Handling 🧩

| Objective | Description | Notes | Labbing | File |
|----------|-------------|-------|---------|------|
| 🧱 Understanding Objects | PowerShell is object-oriented | Everything is an object; properties vs methods | Use `Get-Process | Get-Member` to explore properties and methods | `ObjectsLab.ps1` |
| 🔎 Selecting & Sorting Data | Choose and order object properties | `Select-Object` selects properties; `Sort-Object` orders objects | Get top 5 processes by CPU; display only Name and CPU properties | `SortingSelecting.ps1` |
| 🗂️ Filtering Data | Filter objects based on conditions | `Where-Object` filters collections | Filter running services; filter files by extension or size | `FilteringLab.ps1` |
| 📤 Exporting Data | Save objects for later use | `Export-Csv`, `Out-File`, `ConvertTo-Json` | Export process list to CSV; convert list of services to JSON | `ExportLab.ps1` |

---

## 4.0 Scripting Fundamentals 📝

| Objective | Description | Notes | Labbing | File |
|----------|-------------|-------|---------|------|
| 🖊️ Script Files & Execution | Writing reusable scripts | Scripts are `.ps1`; execution policy must allow scripts (`RemoteSigned`) | Create script printing "Hello World"; run it in PowerShell | `HelloWorld.ps1` |
| 🔄 Conditional Statements | Control flow based on conditions | `if`, `elseif`, `else` | Script that checks a variable and prints messages based on value | `ConditionalsLab.ps1` |
| 🔁 Loops | Repeat actions | `for`, `foreach`, `while`, `do-while`; iterate arrays or collections | Loop through files in folder and print names; use `for` to calculate 1–10 | `LoopsLab.ps1` |
| 🛠️ Functions | Encapsulate code | `function Function-Name {}`; parameters, return values | Create function that accepts a number and returns its square | `FunctionsLab.ps1` |
| ⚠️ Error Handling | Handle exceptions | `try`, `catch`, `finally`; `$Error` stores recent errors | Script that handles division by zero gracefully | `ErrorHandlingLab.ps1` |

---

## 5.0 Advanced Topics 🚀

| Objective | Description | Notes | Labbing | File |
|----------|-------------|-------|---------|------|
| 📦 Modules & Importing | Use and create modules | `Import-Module`, `Get-Module`; create custom modules | Import a module and list cmdlets; create simple module with one function | `ModulesLab.ps1` |
| 🌐 Remoting & Jobs | Remote execution & background tasks | `Invoke-Command`, `Enter-PSSession`, `Start-Job` | Run a command remotely; start a background job and check status | `RemotingJobsLab.ps1` |
| 🛡️ Advanced Functions & Parameters | Functions with pipeline input | Parameter validation, switches, pipeline input | Function that accepts pipeline input and validates parameters | `AdvancedFunctions.ps1` |
| 🗄️ Registry & File System Automation | Automate system settings and files | `Get-ItemProperty`, `Set-ItemProperty`; automate file tasks | Read registry key; script to back up a folder automatically | `RegistryFileSystem.ps1` |
| 🔗 Interacting with APIs | Call and process web data | `Invoke-RestMethod`, `Invoke-WebRequest`; parse JSON/XML | Call public API and output parsed JSON; automate data collection | `APILab.ps1` |

---

## 6.0 Administration & Security 🛡️

| Objective | Description | Notes | Labbing | File |
|----------|-------------|-------|---------|------|
| 👥 User & Group Management | Manage Active Directory accounts | `Get-ADUser`, `New-ADUser`, `Add-ADGroupMember`; RSAT required | List all users in a group; add test user to a security group | `ADUserGroup.ps1` |
| ⚙️ Process & Service Management | Manage processes and services | `Get-Process`, `Stop-Process`, `Get-Service`, `Start-Service` | Stop test process; start/stop service via script | `ProcessServiceLab.ps1` |
| 📈 Event Logs & Monitoring | Monitor system events | `Get-EventLog`, `Get-WinEvent`; useful for auditing | List recent system errors; export event logs to CSV | `EventLogsLab.ps1` |
| 📅 Scheduled Reporting | Automate tasks & reporting | `Register-ScheduledTask` | Schedule script to run daily that logs disk usage | `ScheduledTasksLab.ps1` |

