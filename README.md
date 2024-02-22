# To-do-list

1. **Document Type Declaration**: `<!DOCTYPE html>` declares the document type and version of HTML being used, which is HTML5 in this case.

2. **HTML Structure**: 
   - `<html>`: The root element of the HTML document.
   - `<head>`: Contains meta-information about the HTML document, such as character set, viewport settings, title, and links to external resources like CSS and JavaScript files.
   - `<body>`: Contains the visible content of the HTML document.

3. **External Resources**:
   - Google Fonts: Imports the "Quick Sand" font from Google Fonts for use in the web application.
   - Font Awesome: Imports the Font Awesome library for icons used in the application.
   
4. **Page Title**: `<title>` element sets the title of the web page.

5. **Body Content**:
   - `<div id="header">`: Contains the header section of the application, including theme selector buttons and the main title.
   - `<div id="form">`: Contains the form for adding new tasks to the to-do list.
   - `<div class="version">`: Positioned in the top left corner, contains information about the version of the application and a link to the GitHub repository.
   - `<div id="myUnOrdList">`: Contains the unordered list (`<ul>`) element where the to-do list items will be displayed.
   - JavaScript: Includes a reference to the JavaScript file `main.js` for adding interactivity to the application.
   
7. **Inline JavaScript**:
   - `<script src="/Project/TO-DO-LIST/time.js"></script>`: Loads a JavaScript file `time.js` that may be responsible for displaying the current date and time.
   
This HTML code sets up the basic structure of a to-do list web application, including styling and functionality through external CSS and JavaScript files. It provides areas for displaying tasks, adding new tasks, and selecting themes, among other features.

This CSS code provides styling for your to-do list web application. Let's break down the key components:

### Reset Styles:
- `*`: Resets margin, padding, and sets box-sizing to border-box for all elements.
- `body`: Aligns content to the center vertically, sets the font family, and adds some padding to the top.

### Body Themes:
- `.standard`, `.light`, `.darker`: Defines styles for different themes including background color and text color.

### Header and Form:
- `#header`, `#form`: Defines styles for the header and form sections.
- `.flexrow-container`: Styles for the theme selector buttons.
- `.theme-selector`: Styles for individual theme selector buttons.
- `#title`: Styles for the main title including animation for typing effect.

### Form:
- `form`: Styles for the form element.
- `form input`: Styles for the input field including different background colors based on the theme.
- `form button`: Styles for the button including different background colors based on the theme.

### To-Do List:
- `#myUnOrdList`: Styles for the unordered list container.
- `.todo-list`: Styles for the list itself.
- `.todo`: Styles for individual to-do items including background color and padding.
- `.todo li`: Styles for the to-do item text.
- `.check-btn`, `.delete-btn`: Styles for the check and delete buttons.
- `.completed`: Styles for completed to-do items including text decoration and opacity.
- `.fall`: Styles for the animation when deleting a to-do item.

### Responsive Design:
- Media queries for adjusting styles based on screen width to ensure responsiveness on different devices.

Overall, this CSS code provides comprehensive styling for your to-do list web application, including different themes, form input styles, and responsive design adjustments.

This JavaScript code provides the functionality for your to-do list web application. Let's break down the key components:

### Selectors:
- `toDoInput`, `toDoBtn`, `toDoList`: Select various elements from the HTML document using query selectors.
- `standardTheme`, `lightTheme`, `darkerTheme`: Select theme selector buttons.

### Event Listeners:
- `toDoBtn`: Listens for clicks on the "Add" button to add a new to-do item.
- `toDoList`: Listens for clicks on the to-do list for actions such as deletion or completion.
- `DOMContentLoaded`: Listens for the DOM content to be loaded and then calls the `getTodos` function to load saved to-dos.
- Theme selector buttons: Listens for clicks on theme selector buttons and calls the `changeTheme` function accordingly.

### Functions:
- `addToDo(event)`: Adds a new to-do item to the list. Checks for an empty input field and prevents submission if it's empty.
- `deletecheck(event)`: Handles deletion and completion of to-do items. Removes the item from the list and updates local storage accordingly.
- `savelocal(todo)`: Saves to-do items to local storage.
- `getTodos()`: Retrieves to-do items from local storage and displays them on the page.
- `removeLocalTodos(todo)`: Removes to-do items from local storage.
- `changeTheme(color)`: Changes the theme of the application. Updates CSS classes for elements based on the selected theme and saves the theme choice to local storage.

Overall, this JavaScript code provides the necessary functionality for adding, deleting, and completing to-do items in the web application, as well as the ability to switch between different themes.

