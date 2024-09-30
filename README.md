# Chemical Supplies Web Application

This web application provides a user interface for managing chemical supply data. It allows users to view, edit, add, delete, and reorder chemical entries in a table format. The application is built using HTML, CSS (Bootstrap), and JavaScript.

## Features
1. Display chemical data in a sortable table
2. Add new chemical entries
3. Edit existing chemical entries inline
4. Move entries up and down in the table
5. Delete chemical entries
6. Refresh data from the server
7. Save updated data to a JSON file

## HTML Structure
The main components of the HTML structure are:
1. **Header**: Displays the application title.
2. **Toolbar**: Contains action buttons for managing chemical entries.
3. **Table**: A responsive table to display chemical data.

## CSS Styling
The application uses **Bootstrap 5.1.3** for its primary styling and includes some custom styles to ensure responsiveness and manage table interactions.

## JavaScript Functionality

### Data Management
- **`chemicalData`**: An array that stores the chemical supply data.
- **`fetchData()`**: Fetches data from 'invoice.json' and populates the table.
- **`renderTable()`**: Renders the chemical data in the table.
- **`updateData()`**: Updates the `chemicalData` array when inline editing occurs.

### Table Interactions
- **Sorting**: Clicking on column headers sorts the table.
- **Row selection**: Clicking on a row highlights it.
- **Inline editing**: Table cells are `contenteditable` to allow inline editing.

### Button Actions
- **Add Row**: Adds a new empty row to the table.
- **Move Up**: Moves the selected row up in the table.
- **Move Down**: Moves the selected row down in the table.
- **Delete Row**: Removes the selected row from the table.
- **Refresh**: Fetches data from the server and updates the table.
- **Save**: Downloads the updated data as a JSON file.

## Data Structure
Each chemical entry in the `chemicalData` array has the following properties:
- **`id`**: Unique identifier.
- **`chemical_name`**: Name of the chemical.
- **`vendor`**: Supplier of the chemical.
- **`density`**: Density in g/m³.
- **`viscosity`**: Viscosity in m²/s.
- **`packaging`**: Type of packaging.
- **`pack_size`**: Size of the package.
- **`unit`**: Unit of measurement.
- **`quantity`**: Amount of the chemical.

## Initialization
The application initializes by calling **`fetchData()`** to load the initial data from 'invoice.json'.

## Potential Improvements
1. Implement server-side saving instead of client-side file download.
2. Add form validation for inline editing.
3. Implement pagination for large datasets.
4. Add search functionality.
5. Implement undo/redo functionality.
6. Add user authentication and authorization.

---

This documentation provides an overview of the **Chemical Supplies Web Application**'s structure and functionality. It can serve as a reference for understanding the code and for future maintenance or enhancements.
