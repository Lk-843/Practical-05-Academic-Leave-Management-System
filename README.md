# Academic Calendar & Leave Management System

**Practical 5 — .NET Technologies**

A simple ASP.NET Web Forms practical demonstrating:
- Login form and basic credential validation
- Session state for tracking the logged-in user
- A “Remember Me” cookie
- Calendar date selection
- Leave application form with input validation
- Back and logout navigation

## Files

- `Login.aspx` / `Login.aspx.cs` — login page and code-behind
- `Default.aspx` / `Default.aspx.cs` — academic calendar and selected leave date
- `Leave.aspx` / `Leave.aspx.cs` — leave application form and validation

## Demo login

- **User ID:** `student`
- **Password:** `1234`

These credentials are hard-coded for this classroom demonstration only. Do not use this authentication approach in a real application.

## Run the project

1. Open Visual Studio on Windows.
2. Create an **ASP.NET Web Application (.NET Framework)** project using **Web Forms**.
3. Set the project namespace to `Practical_05_Academic_Leave_Management_System`, or update the `Inherits` declarations and namespaces to match your project.
4. Add these `.aspx` pages and code-behind files to the project.
5. Ensure each `.aspx` page is associated with its `.aspx.cs` code-behind file.
6. Run the project and open `Login.aspx`.

> Note: These source files are the page-level code from the practical. A complete Visual Studio solution/project file and designer files are not included, so you may need to create the Web Forms project first and add the files.

## Concepts demonstrated

**Session:** Stores the current user and selected leave date during the session.

**Cookie:** If “Remember Me” is selected, a `UserID` cookie is created with a seven-day expiry.

**Calendar control:** Selecting a date displays it and stores it in session state.

**Validation:** Leave type, reason, and a positive number of days are required before the application-success message is shown.

## Security note

This is a learning/demo project. It does not store leave applications in a database, and its sample login is not suitable for production.
