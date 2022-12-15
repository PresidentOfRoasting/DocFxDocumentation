# DocFxDocumentation
## 1. Install choclatey
### Check your execution policy 
Execute the following commands in the Windows Powershell
**ExecutionPolicy** 

If the powershell shows

**Restricted**

Run

**Set-ExecutionPolicy AllSigned** 

or 

**Set-ExecutionPolicy Bypass -Scope Process** 

Now run the following command 

**Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))**

### Install Docfx via choclatey
Run

**choco install docfx**

## 2. Create docfx framework
Run

**docfx init -q**
