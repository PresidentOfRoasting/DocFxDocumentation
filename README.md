# DocFxDocumentation
## 1. General information
DocFX can produce documentation from source code (including C#, F#, Visual Basic, REST, JavaScript, Java, Python and TypeScript) as well as raw Markdown files.

It can run on every platform.
## 2. Install choclatey
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

## 3. Create docfx framework
Run

**docfx init -q**

## Run the application

Run the following command to run the application

**docfx docfx.json --serve**

You can now see your documentation on http://localhost:8080/

## 4. Create documentation
Whatever you write into the markdown file will appear on the html page.

If you create a new .md file, you need to register it in toc.yml

## 5. Create a new section
To create a new section you need to create a new markdown file in the article folder.

Now add your folder to the sections in toc.yml
