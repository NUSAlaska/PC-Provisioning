# NUS Compuer Provisioning Details

## Windows 11 Installation Media

Create a USB drive with Windows `Media Creation Tool`. Once installed on the USB drive, copy the `ei.cfg` to the `\Sources` folder on the USB drive to ensure that Windows 11 Pro is installed rather than Windows 11 Home. 

Once installed make sure you make the first account as a "Work Or School" account. 

## Software Installation & Provisioning

Once you finish windows 11 initialization and get to a desktop, we can install all the standard software in an automated fashon using Boxstarter.

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