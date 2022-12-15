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

## Run the application

Run the following command to run the application

**docfx docfx.json --serve**

You can now see your documentation on http://localhost:8080/

## 3. Create documentation
Whatever you write into the markdown file will appear on the html page.

If you create a new .md file, you need to register it in toc.yml

## 4. Create a new section
To create a new section you need to create a new markdown file in the article folder.

Now add your folder to the sections in toc.yml
