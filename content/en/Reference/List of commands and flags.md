---
title: List of commands and flags
weight: 93
description: 'In this section, you will find the list of Ritchie''s main commands'
---

---

## Commands

### **Configuration commands**

| Commands | Operation | Flags |
| :--- | :--- | :--- |
| rit init  | initialize Ritchie before use |
| rit upgrade | upgrade to the last Ritchie stable version |
| rit tutorial  | enable or disable the tutorial | `--enabled=false` |
| rit set formula-runner | configures the runtime to execute via docker or locally | `--runner=docker` |
| rit --version | return Ritchie currently installed version |

### Repo commands 

| Command | Operation |
| :--- | :--- |
| rit add repo | add a new repository \(to access repository formulas with Ritchie\) |
| rit list repo |  show a list with all your available repositories |
| rit update repo | update all repositories  \(to access new formulas from those repositories with Ritchie\) |
| set repo-priority | set a repository priority |
| rit delete repo | delete a repository \(to remove access to the repository formulas with Ritchie\) |

### Formula commands

<table>
  <thead>
    <tr>
      <th style="text-align:left">Command</th>
      <th style="text-align:left">Operation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">rit create formula</td>
      <td style="text-align:left">
        <p>create a new formula from scratch</p>
        <p>(as well as a new local repository if necessary)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">rit build formula</td>
      <td style="text-align:left">build a formula locally for test</td>
    </tr>
    <tr>
      <td style="text-align:left">rit build formula --watch</td>
      <td style="text-align:left">build a formula monitoring the code to update real time changes</td>
    </tr>
  </tbody>
</table>

{{% alert color="danger" %}}
The rit build formula command was deprecated from Ritchie's version 2.5.0.
{{% /alert %}}

### Autocomplete commands

| Commands | Operation |
| :--- | :--- |
| rit completion zsh | add autocomplete via zsh |
| rit completion bash | add autocomplete via bash |
| rit completion fish | add autocomplete via fish |
| rit completion powershell | add autocomplete via powershell |

### Env commands

| Commands | Operation |
| :--- | :--- |
| rit set env | set a new environment |
| rit show env | show the current environment used |
| rit delete env | delete a environment |

### Credential commands

| Commands | Operation |
| :--- | :--- |
| rit set credential | set new credentials for the context |
| rit list credential | list all credential names and fields |

### Workspace commands

| Commands | Operation |
| :--- | :--- |
| rit list workspace | list all formula's workspaces  |
| rit add workspace | add a new workspace |
| rit delete workspace | delete a specific formula's workspace |

## Flags 

### Main flags

| Flags | Operation |
| :--- | :--- |
| --default | attribute the **default** values configured on the formula. |
| --docker | run a formula using **Docker** |
| --help | returns a list of executable available commands and flags for the user |
| --local | run a formula **locally** |
| --verbose | run a formula without log details |
