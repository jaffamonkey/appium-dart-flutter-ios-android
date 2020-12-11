An example of running appium_dart

## Install Chocolately

First, ensure that you are using an administrative shell - you can also install as a non-admin, check out Non-Administrative Installation.
Install with powershell.exe

NOTE: Please inspect https://chocolatey.org/install.ps1 prior to running any of these scripts to ensure safety. We already know it's safe, but you should verify the security and contents of any script from the internet you are not familiar with. 

With PowerShell, you must ensure Get-ExecutionPolicy is not Restricted. 

We suggest using Bypass to bypass the policy to get things installed or AllSigned for quite a bit more security.

Run 
```
Get-ExecutionPolicy
```. 
If it returns Restricted, then run 
```
Set-ExecutionPolicy AllSigned
```
OR
```
Set-ExecutionPolicy Bypass -Scope Process.
```

Now run the following command:
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

Paste the copied text into your shell and press Enter.
Wait a few seconds for the command to complete.
If you don't see any errors, you are ready to use Chocolatey! Type choco or choco -? now


## Install Dart SDK

choco install dart-sdk
choco upgrade dart-sdk

```
$ pub get
$ dart --enable-asserts main.dart
```
