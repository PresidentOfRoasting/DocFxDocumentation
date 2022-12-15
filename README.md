# DocFxDocumentation
## 1. Install choclatey
### Check your execution policy 
**ExecutionPolicy** <br />
If the powershell shows <br />
**Restricted** <br />
Run <br />
**Set-ExecutionPolicy AllSigned** <br />
or <br />
**Set-ExecutionPolicy Bypass -Scope Process** <br />
Now run the following command <br />
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

### Install Docfx via choclatey
Run
choco install docfx
