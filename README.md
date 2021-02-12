# Increo .NET Developer Test
Implementation of a simple To-Do application, using HTML5 on the frontend, C# and .NET on the backend. The application allows you to add, view, mark as done, and delete tasks.

## Functionality
The application displays a list of tasks to be performed. Tasks are divided into _done_ and _to be done_. Tasks _done_ are crossed out and are marked in color `#9eb2c0` and the checkbox on the left is checked. Tasks _to be done_ are marked with color `#2e3641` and the checkbox on the left is unchecked.

A field with the function of adding a new task is always displayed under the last task in the list. The new task added through there is always _to be done_. When adding a task from that field, the new task will appear at the bottom of the list, but above the add-new-task field. To add the new task from the field at the bottom, it should react to clicking the `+` icon on the left, or pressing the `ENTER` key. Either way, the focus should return to the title field and the field emptied after the new task is created and added to the list. You cannot add a task without adding a title. Validation should be on both the frontend and backend sides.

Each task can be deleted by clicking the trash icon, but should display a message box to the user asking: `Are you sure?`

## Frontend
Application design:

![Application design](https://raw.githubusercontent.com/nagilum/increo-dotnet-dev-test/main/assets/to-do-list.png)

* In the [assets](https://github.com/nagilum/increo-dotnet-dev-test/tree/main/assets) folder you will find the `PSD` Photoshop file with the application design. You can use [Photopea](https://www.photopea.com/) to work with `PSD` files online.
* The application should be written as a `Single Page Application`, using only one `HTML` file, one `CSS` file, and one `JavaScript` file.
* Communication between frontend and backend should work in the background, without reloading the page, preferably using `AJAX`.
* Application style should be built using a `CSS Preprocessor`, like `SCSS` or `LESS`.
* Application logic should be divided with `Model-View-Controller` or `Model-View-Whatever` architecture.
* Please do not use any JS libraries, or use them with minimal amount. We prefer `Vanilla JS`.
* Use a sans-serif font, like [Open Sans](https://fonts.google.com/specimen/Open+Sans), from [Google Fonts](https://fonts.google.com/).

## Backend
* API should be written according to the REST specification. All queries and responses are sent in JSON format. If there is no error, the response should be 200 or 201 accordingly. If there is an error, it should return 400 with an array of error messages.
* Separate the `Controller` code and the `Data` code.
* There will be no user service or authentication, each person has access to create, read, delete, or updating tasks.
*  [OPTIONAL] Implement some sort of storage cache for the data layer, it can be in-memory for ease. You need to make sure the cache is invalidated and updated when the user adds a new task.

## Misc
* The code should be *readable and described* by comments. JavaScript according to [documentationjs](https://github.com/documentationjs/documentation/blob/master/docs/GETTING_STARTED.md), .NET according to [Microsoft Docs](https://docs.microsoft.com/en-us/dotnet/csharp/codedoc), and other languages according to the selected specification.
* We leave the application in the development version, we do not minify the files, we do not compress them, we do not combine them, etc.
* Please attach instructions on how to run the application(s).

### Good luck

#### Copyrights
Graphic design is a rewritten version of [To Do List](https://www.behance.net/gallery/10852567/To-Do-List-(PSD)) by [Marijan Petrovski](https://www.behance.net/psdchat).

This .NET developer test is distributed under the MIT license.