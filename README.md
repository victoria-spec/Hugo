# Hugo Portfolio Setup (Windows Environment)

This guide explains the steps to install and configure a Hugo portfolio website on Windows.

---

## 🛠 Step 1: Install Required Software

1. Open **PowerShell** as **Administrator**

2. Run the following commands from:

```powershell
   C:\Windows\System32
```
4. Install required tools:

```powershell
winget install Hugo.Hugo.Extended
winget install Git.Git
winget install GoLang.Go
```
4. Navigate to root directory: **C:\\** folder
```powershell
cd C:\
```
6. Create a websites folder **websites**:
```powershell
mkdir websites
cd C:\websites
```
5. Create a new Hugo site using YAML format:
```powershell
hugo new site mysite --format="yaml"
```
5. Exit PowerShell:
```powershell
exit
```
## 📂 Step 3: Folder Structure

```powershell
C:
└── website
└── mysite
├── archetypes\ # Content templates
├── assets\ # CSS, JS, images processed by Hugo Pipes
├── content\ # Website pages and blog posts
├── data\ # YAML/JSON/TOML data files
├── layouts\ # Custom layout templates
├── static\ # Static files (images, favicon, etc.)
├── themes\ # Installed themes
│ └── hugo-profile
├── config.yaml # Site configuration file
└── public\ # Generated site (after running hugo)
```

### 📌 Quick Explanations

| Folder/File       | Purpose |
|------------------|---------|
| `archetypes/`    | Templates used when creating new content with `hugo new` |
| `assets/`        | Stylesheets, JS, and images that Hugo processes |
| `content/`       | Markdown files for pages and blog posts |
| `data/`          | Optional structured data files for your site |
| `layouts/`       | HTML templates for customizing the site layout |
| `static/`        | Files copied directly to the final site without processing |
| `themes/`        | Installed themes for your site |
| `config.yaml`    | Main configuration file for your Hugo site |
| `public/`        | Auto-generated folder containing the website output (Appears after the the site is generated) |

---
## 🛠 Step 3: Download Isabela Protfolio

1. Open **PowerShell** as **Administrator**
2. Navigate to root directory: **C:\\website\mysite\themes** folder
```powershell
cd C:\\website\mysite\themes
```
3. Download **hugo-profile** profile. Run following command
```powershell
git clone https://github.com/gurusabarish/hugo-profile
```
3. View Hugo-Profile theme
```powershellcd
cd C:\\website\mysite\themes\hugo-profile
```
4. View Hugo-Profile theme
```powershell
C:
├── archetypes
└──exampleSite
└──i18n
└──images
└──i18n
└──layouts
└──.gitignore
└──LICENSE
└──.gitignore
└──netlify.toml
└──theme.toml
```
4. Go to **C:\websites\mysite\themes\hugo-profile\exampleSite** and copy following folders and files to **c:\websites\mysite**   
```powershell
   static
   ccontent
   hugo.yaml
```
## 🌟 Step 4: Start Local Web site 

1. Open **PowerShell** as **Administrator**
2. Go to **c:\websites\mysite**
```powershell
   cd c:\websites\mysite
```
3. run Hugo server
```powershell
   hugo server -D
```

```powershell
   hugo server -D --disableFastRender
```

4 Start web brouser and run 
```powershell
   http://localhost:1313
```
