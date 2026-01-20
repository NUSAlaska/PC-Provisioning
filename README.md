Currently using Boxstarter to standardize the windows 11 pro instance on new machines.

Find more info about boxstarter here: https://boxstarter.org/weblauncher
Old Installation Gist here: https://gist.github.com/KroniK907/de671b3ec850d2a1bc3d616c60807740
New Installation moved to the `NUS-Chocolatey-default` file in this repo.

Command to run on new machines from admin powershell (currently still old version):

```powershell
START https://boxstarter.org/package/url?https://gist.githubusercontent.com/KroniK907/de671b3ec850d2a1bc3d616c60807740/raw/f4937c293e6f42401396823abb0cac4e32b7855b/NUS-Chocolatey-default
```

Once the above is complete, use the following command to run the debloat tool:

```powershell
iwr -useb https://christitus.com/win | iex
```

The `win-util.json` is a standard settings import for the windows tool.

More info on this tool here: https://christitus.com/windows-tool/