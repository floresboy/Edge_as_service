# Edge_as_service


# Instructions for running this PowerShell installation script.

 1) Open Windows PowerShell as administrator.

 2) Temporarily sets the current PowerShell session execution policy to Bypass.
 Set-ExecutionPolicy Bypass -Scope Process -Force

 3) Navigate to the folder where you downloaded the PowerShell script and execute the "Install-HiveMQ-WindowsServer-Standalone.ps1" script to install HiveMQ.
 .\Install-HiveMQ-WindowsServer-Standalone.ps1


# Version 

Alpha 1 - !! Not production ready !!
250721-1241

# Need to fix:
Hardcoded 2025.11 in line 131

# Commands
 .\nssm.exe remove HiveMQEdgeService

Example: Forcefully delete all transcript files in a directory
Remove-Item -Path "c:\hivemq-edge\*" -Include *.txt,*.log -Force -Recurse -ErrorAction SilentlyContinue

Stop-Transcript
