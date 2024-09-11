
# User Management Interface Specification

## 1. Overview
The **User Management** screen's user interface (UI), which allows administrators to create, change, enable, disable, and assign roles to users, is described in this article.

## 2. Initial View
The list of current users is shown in a table format when the user initially accesses the website.
- The list is filtered to only display enabled users by default, with the `Hide Disabled User` button ticked.
- The New User form on the right panel is blank and waiting for information to be entered for a new user.
- Columns for ID, Username, Email, and Enabled status are present in the list.

## 3. UI Components

### 3.1 User Table
- **Columns**:
  - **ID**: Shows the user's unique ID (read-only).
  - **User Name**: Shows the username.
  - **Email**: Shows the email address of the user.
  - **Enabled**: Shows a true or false indicator of the user's enablement.
- **Sortable Columns**: Each column can be sorted ascending or descending.
- **Checkbox - Hide Disabled Users**: If the checkbox labeled `Hide Disabled User` is selected, only users who have the status "Enabled" set to "true" will be seen.
- **Behavior**: The table dynamically updates based on sorting and filter criteria.


### 3.2 New User Form
- **Fields**:
  - **Username**: Enter the input for the username.
  - **Display Name**: Enter the input for the display name.
  - **Phone**: Enter the input for the phone number.
  - **Email**: Enter the input for the user's email address.
  - **User Roles**:  A drop-down menu allowing you to choose between the roles of Guest, Admin, and SuperAdmin.
  - **Enabled**: Checkbox to mark the user as enabled or disabled.
  
- **Buttons**:
  - **Save User**: When clicked, saves the user information .
  - **+ New User**: Makes the form clear so that a new user can be created.
  
### 3.3 Behavior
- **Adding a New User**:
  - Click the "+ New User" button to add a new user.
  - Fill in the required fields and select roles for the user.
  - Click the "Save User" button to save the new user.
  - The user is added to the table and displayed based on the filter criteria.
  
  
- **Enabling/Disabling a User**:
  - Modify the "Enabled" checkbox in the form.
  - If a user is disabled, they will be hidden if the "Hide Disabled Users" checkbox is checked.

### 3.4 Additional Features
- **Search**: Users can be filtered by email address or name using the search feature in the table.
- **Validation**: Verify that all fields (Username, Email, Roles) are correctly filled in before saving.
- **Error Handling**: Show error messages if saving fails or if invalid input is entered (duplicate usernames or invalid email format).
