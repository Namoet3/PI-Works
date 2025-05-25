

# User Management Screen - UI Specification

## Overview

The User Management Screen allows administrators to manage user accounts within the system. This includes viewing user details, creating new users and assigning roles.

## Functional Requirements

* Display a list of all users with relevant details.
* Provide functionality to add a new user.
* Implement sort and filter capabilities for easy navigation.

## UI Components

### Header

**Buttons:**

* **Add User**: Opens a form to create a new user.
* **Hide Disabled User**: Checkbox to only show enabled users.
* **Save User**: Submits and saves the new user.

### Sort and Filter

**Filter and Sort Columns in the Table:**

* **ID**: Filter users by ID and sort from smaller to larger or vice versa.
* **UserName**: Filter users by name and sort alphabetically.
* **Email**: Filter users by email and sort alphabetically.
* **Enabled**: Filter users by enabled state and sort by `true` or `false`.

### User Table

**Columns:**

* ID
* User Name
* Email
* Enabled

### Modals

#### Add User Modal

**Fields:**

* Username
* Display Name
* Phone
* Email
* User Role (Dropdown)
* Enabled (Checkbox)

**Buttons:**

* Save (located in the header)

## Behavior

### On Page Load

* Fetch and display the list of users.
* Set default filters to show all users.

### Filter Functionality

Selecting options from the role dropdown or column filters will update the displayed user list accordingly.

### Add User

Clicking **Add User** opens the modal. Upon clicking **Save**, the new user is added and the modal closes.

## Initial State

* The user list is populated with existing users.
* No filters are applied; all users are shown.


