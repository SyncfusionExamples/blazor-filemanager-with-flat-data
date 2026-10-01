# Blazor-Filemanager-With-Flat-Data

## Overview

This sample demonstrates how to integrate the Syncfusion [Blazor File Manager](https://www.syncfusion.com/blazor-components/blazor-file-manager) within a Blazor Server application. Instead of relying solely on a hierarchical file provider, the application uses a custom `FileManagerService` to manage file and folder operations while supplying data in a format that can be consumed by the File Manager component.

The sample showcases how common file management operations such as reading folders, creating directories, deleting items, renaming files, searching content, moving files, copying files, uploading files, downloading files, and image preview loading can be implemented through File Manager event handlers. It serves as a reference implementation for developers who want to connect the File Manager component to custom storage systems, APIs, databases, or service-based file repositories.

## Key Features

- Integrates the Blazor File Manager component in a Blazor Server application.
- Uses a custom `FileManagerService` for backend file and folder operations.
- Retrieves file and folder information using the `GetFiles()` method.
- Handles File Manager read requests through the `OnReadAsync(ReadEventArgs args)` event handler.
- Processes folder creation using the `FolderCreatingAsync(FolderCreateEventArgs args)` event handler and the `Create()` service method.
- Deletes files and folders using the `ItemsDeletingAsync(ItemsDeleteEventArgs args)` event handler and the `Delete()` service method.
- Supports file and folder searching using the `SearchingAsync(SearchEventArgs args)` event handler and the `Search()` service method.
- Renames files and folders using the `ItemRenamingAsync(ItemRenameEventArgs args)` event handler and the `Rename()` service method.
- Supports file and folder move operations using the `Move()` service method.
- Supports file and folder copy operations using the `Copy()` service method.
- Handles file uploads through the `ItemsUploadedAsync(ItemsUploadedEventArgs args)` event handler.
- Loads image previews using the `BeforeImageLoadAsync(BeforeImageLoadEventArgs args)` event handler and the `GetImage()` service method.
- Supports file downloads using the `BeforeDownload(BeforeDownloadEventArgs args)` event handler and the `Download()` service method.
- Demonstrates file-system validation logic during upload operations to prevent directory traversal issues.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the following project file:

   `blazor-filemanager-with-flat-data.csproj`

3. Restore NuGet packages.
4. Build the project.
5. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Open a terminal and navigate to the project directory.
3. Restore the required packages:

```bash
dotnet restore
```

4. Run the application:

```bash
dotnet run
```

5. Open the local URL displayed in the terminal after the application starts.

## Usage

The File Manager displays files and folders sourced from a flat data structure. User interactions such as creating folders or deleting items are handled through the locally injected File Manager service.

## Configuration

The flat data logic is implemented within the FileManagerService.cs file. You can customize this service to connect to databases or APIs and extend file operation behavior as needed.

## Project Structure

`FileManagerService.cs` - Core service implementation containing file operations, flat-data processing, image retrieval, uploads, downloads, move, copy, rename, create, delete, and search logic.

`Pages/Index.razor` - Primary sample page hosting the File Manager component and wiring File Manager events to service methods.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- File Manager documentation: https://help.syncfusion.com/file-manager-sdk/blazor/getting-started-with-web-app

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.
