Core Features:
Excel File Interaction: Users can open and load data from Excel files into the application. This functionality is facilitated by the load_excel_file method, which uses pandas to read the data and store it in a DataFrame.
Data Display: Loaded data from Excel sheets is displayed in tabs corresponding to each sheet within the Excel file. This is managed by the add_sheet_tab method, which creates a new tab for each sheet and displays its contents in a table format.
Data Editing: The application allows users to directly edit data within the loaded Excel sheets. Edited data is reflected back in the original Excel file, ensuring that changes are persistent. This functionality is primarily handled through the edit_cell method, which enables editing of individual cell values.
Summation of Numeric Values: The application can sum numeric values within selected cells, including cells with multiple numeric values separated by line breaks. This is achieved with the update_sum_display method, which updates a sum label with the total of selected values.
Search Feature: Users can search through all loaded data for specific text, numbers, or phrases, enhancing the ease of data navigation and analysis. This is implemented via the search_tables method.
Context Menus: Right-click context menus provide additional functionality, such as viewing detailed cell information or editing cells, through the show_context_menu method.
Resizable Tables: The application features resizable tables that adjust row heights automatically to accommodate the content, ensuring readability and ease of use.
UI Components:
Main Window Setup: The initUI method sets up the main window, status bar, menu bar, and central widget, which includes the search bar and tab widget for displaying Excel sheet data.
Dialogs for Additional Information: Through openNewTextWindow and openNewTextWindow2, the application can display dialogs that provide information about the program and usage instructions.
Custom Table Widget: A custom table widget, CustomTableWidget, enhances interaction by handling mouse events differently, such as ignoring double-clicks and enabling edit mode on single-clicks under certain conditions.
Utility Functions:
Data Cleaning: The clean_data method processes data from Excel files to ensure it's in a suitable format for display and analysis, such as trimming strings and rounding float values.
Excel File Saving: The save_excel_file method saves changes made within the application back to the original Excel file, ensuring that edits are not lost.
Design and Style:
The application uses a gray color scheme for its widgets and provides a custom font setting for aesthetics and readability.
Error Handling and User Feedback:
Error messages and critical alerts are implemented to inform the user of issues such as file loading errors or saving issues, enhancing the user experience by providing clear feedback.
This summary encapsulates the primary functions and features of the "ARTEMĪDA" application, highlighting its capabilities as a tool for interacting with, editing, and analyzing Excel file data within a PyQt5 GUI framework.
