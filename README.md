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

## 🛠 Step 2: Download Isabela Protfolio

1. Open **PowerShell** as **Administrator**
2. Navigate to root directory: **C:\\website\mysite\themes** folder
```powershell
cd C:\\website\mysite\themes
```
3. Download **hugo-profile** profile. Run following command
```powershell
git clone https://github.com/gurusabarish/hugo-profile
```
4. View Hugo-Profile theme
   

