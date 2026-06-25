# Blazor-Filemanager-With-Flat-Data

**Repository Description**  
This repository contains a **Blazor sample** that demonstrates how a **flat data representation** can be integrated into the [Blazor File Manager](https://www.syncfusion.com/blazor-components/blazor-file-manager) component.

The sample shows how to manage files and folders using a locally injected `FileManagerService.cs`, enabling file operations such as reading, deleting, and creating folders without relying on a hierarchical file system structure.

## Project Overview
The purpose of this project is to help developers understand how the Blazor File Manager can be configured to work with flat data. It provides a reference implementation for handling file actions using in‑memory or service‑driven data sources within a Blazor application.

## Features
- Integration of **Blazor File Manager**
- Flat data representation for files and folders
- Support for basic file operations:
  - Read files and folders
  - Delete items
  - Create new folders
- Local service‑based file handling using `FileManagerService.cs`
- Clean and lightweight Blazor application structure

## Prerequisites
Ensure the following requirements are met before running this project:
- .NET SDK compatible with Blazor
- Visual Studio 2022 or a compatible IDE
- Syncfusion Blazor packages
- Valid Syncfusion license key (if required)

## Installation

### Clone the Repository
Clone the repository and navigate to the project directory:
```bash
git clone https://github.com/SyncfusionExamples/blazor-filemanager-with-flat-data.git
cd blazor-filemanager-with-flat-data
```
### Restore and Build the Application
Restore the required NuGet packages by running:
```bash
dotnet restore
```
Build the application using:
```bash
dotnet build
```
### Running the Application
After a successful build, run the application with the following command:
```bash
dotnet run
```
Once running, open the application in your browser to view the Blazor File Manager powered by flat data.

## Usage
The File Manager displays files and folders sourced from a flat data structure. User interactions such as creating folders or deleting items are handled through the locally injected File Manager service.

## Configuration
The flat data logic is implemented within the FileManagerService.cs file. You can customize this service to connect to databases or APIs and extend file operation behavior as needed.

## Documentation
- General Syncfusion documentation:
https://help.syncfusion.com/
- Blazor Introduction:
https://blazor.syncfusion.com/documentation/introduction
- Blazor File Manager – Getting Started:
https://blazor.syncfusion.com/documentation/file-manager/getting-started-with-web-app

## Additional Resources
- Syncfusion Blazor File Manager product overview:
https://www.syncfusion.com/blazor-components/blazor-file-manager

## Troubleshooting
- Ensure NuGet packages are restored successfully.
- Verify the FileManagerService.cs is correctly registered and injected.
- Rebuild the solution if changes are not reflected.
- Check application output logs for runtime errors.

## Support
For detailed API references, flat data configuration guidance, and advanced Blazor File Manager scenarios, refer to the Syncfusion Blazor documentation links above.
