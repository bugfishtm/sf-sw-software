# 📦 Software Module

## 📙 Introduction 

This software module is designed for deployment to Suitefish-Windows client instances via the Suitefish-CMS store. To utilize this package, you must have the Suitefish Windows application installed on your computer or a valid Suitefish online instance for distributing software to client devices. Alternatively, you can unzip the package and run the software independently; however, this approach does not provide automatic update functionality.

You may download the example module here: [Download](https://raw.githubusercontent.com/bugfishtm/suitefish-cms/refs/heads/main/_packages/_software-1.10.100.zip)

- Software modules operate independently from the Suitefish-CMS system as they are intended for Windows environments and are not integrated within the CMS itself. For deployment to Windows clients, please use the Suitefish Windows application available at: [https://github.com/bugfishtm/suitefish-windows](https://github.com/bugfishtm/suitefish-windows).
- Software modules can also be distributed through the "Deployment" section in Suitefish-CMS.

## 🛠️ Installation

1. Method: Open the Suitefish Windows application, browse the software store, and select the desired module. You can then effortlessly download and install it directly through the interface.

2. Method: Unzip the module’s ZIP archive and move the entire folder—ensuring it includes the version.php file—into your Suitefish installation’s sf-apps directory. The software will automatically recognize and register the module.

3. Method: Unzip the module’s ZIP archive and launch the starter .exe file as specified in version.php. Note that modules installed using this method cannot be automatically updated, as they are not managed through the Suitefish Windows application.

## 📁 Folder Structure 

| Folder/File | Description | Optional |
|----------|--------|----------|
| `./__Output` | Folder for persistent data between suitefish-cms product updates. | Optional | 
| `./__Persistent` | Folder for persistent data between suitefish-cms product updates. | Optional | 
| `./__Config` | Folder for persistent data between suitefish-cms product updates. | Optional | 
| `./_lang` | Store your language files in this folder | Optional | 
| `./_lang/de.php` | Translation File for German | Optional | 
| `./_lang/en.php` | Translation File for English | Optional | 
| `./_lang/es.php` | Translation File for Spanish | Optional | 
| `./_lang/fr.php` | Translation File for French | Optional | 
| `./_lang/in.php` | Translation File for Hindu | Optional | 
| `./_lang/it.php` | Translation File for Italian | Optional | 
| `./_lang/ja.php` | Translation File for Japanese | Optional | 
| `./_lang/kr.php` | Translation File for Korean | Optional | 
| `./_lang/pt.php` | Translation File for Portuguese | Optional | 
| `./_lang/ru.php` | Translation File for Russian | Optional | 
| `./_lang/tr.php` | Translation File for Turkish | Optional | 
| `./_lang/zh.php` | Translation File for Chinese | Optional | 
| `./_lang/[LANGEUAGECODE].php`  | Other language Files you may add | Optional | 
| `./_lang/index.php`  | Prevent Directory Listing | Optional | 
| `./_changes/`  | Folder for Changelogs | Optional |
| `./_changes/index.php`  | Prevent Directory Listing | Optional | 
| `./_changes/1.10.100.php`  | Changelog for version 1.10.100 | Optional | 
| `./_licenses` | Store your external licenses in this folder | Optional | 
| `./_licenses/example.lic` | Example License File | Optional | 
| `./_licenses/[LIBNAME].lic` | Store your other License files here | Optional | 
| `./_licenses/index.php` | Prevent Directory Listing | Optional | 
| `./preview.jpg` | Preview image for the store and other areas the module is visble at | Mandatory | 
| `./LICENSE.md` | License information about the module | Mandatory | 
| `./README.md` | Readme file with general information about the module | Mandatory | 
| `./version.php` | Versioning and meta file of the module | Mandatory | 
| `./index.php`  | Prevent Directory Listing | Optional | 
| `./[YOURSOFTWARE].exe`  | Starter File for your software | Mandatory | 

## 📐 Developer Insights

This section provides important information for developers about module development, including essential coding guidelines to be followed prior to submitting or deploying modules.

### 📋 Code Guidelines

Please follow these coding guidelines when developing modules:

- The module's **Rname** identifier must be unique.
- Public image modules should have an Rname starting with **"sw"**.
- Ensure the Rname does not exceed 20 characters.
- Avoid using special characters in the Rname, as they may cause critical errors.
- Only alphanumeric characters. (Leading underscore is reserved for official suitefish modules)

### 📚 Language Files

Language files in this type of module are used only to display the name and description in the store for multilingual support. Below is an example of an English language file (en.php). The initial lines restrict public access to the file. The translation variables enable the store to present the name and description in multiple languages. For detailed information on the file structure and module setup, refer to the Example module files in the https://github.com/bugfishtm/suitefish-cms/tree/main/_developers directory.

### 📝 Changelog File

Changelog of changes between this and last version of this module. Store the changelog in simple html format in the $x variable in files fitting the version number at `_changes`. For detailed information on the file structure and module setup, refer to the Example module files in the https://github.com/bugfishtm/suitefish-cms/tree/main/_developers directory.

## 📄 Documentation 

If you are a developer you can find examples of modules in the _developers folder at the suitefish-cms github repository if you want to create an own module! For more information about the Suitefish CMS: https://github.com/bugfishtm/suitefish-cms. You can find the suitefish windows software at: https://github.com/bugfishtm/suitefish-windows.

🐟 Bugfish