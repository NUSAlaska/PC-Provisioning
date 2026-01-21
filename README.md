Currently using Boxstarter to standardize the windows 11 pro instance on new machines.

Find more info about boxstarter here: https://boxstarter.org/weblauncher

Command to run on new machines from admin powershell:

```powershell
START https://boxstarter.org/package/url?https://raw.githubusercontent.com/NUSAlaska/PC-Provisioning/refs/heads/main/NUS-Chocolatey-default
```
The link is built to reference the `NUS-Chocolatey-default` file in this repo.

Once the above is complete, use the following command to run the debloat tool:

```powershell
iwr -useb https://christitus.com/win | iex
```

The `win-util.json` is a standard settings import for the windows tool.

More info on this tool here: https://christitus.com/windows-tool/