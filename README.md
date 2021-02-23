# dev-laptop-config

A Powershell script to install some default apps via chocolatey

## Usage

Open an admin Powershell prompt and run `.\dev-laptop-config.ps1`. This should install Chocolatey if it is not already installed, and then will being installation of the apps.

## Configuration

You can tweak the list of applications assigned to the variable `$chocolateyAppList` in  `dev-laptop-config.ps1` if you want to make any modifications. You can search for available Chocolatey package names here: https://chocolatey.org/packages

Additionally, you can configure which Windows features to install by adjusting the value of the variable `$dismAppList`. To see which Windows features are available, you can run `Dism /online /Get-Features` from an admin prompt.