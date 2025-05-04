
## Requirement list

| No  | Requirement                                                                                                                                                                                                                                                                   | Use case              |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
| 1   | System users can register for membership. The required information for membership registration includes ID, password, phone number, payment method, and preferred bike type (standard/electric). The administrator can log in with the given ID (admin) and password (admin). | Regist Membership     |
| 2   | Members can withdraw their membership at any time. Upon withdrawal, all user privileges and data are deleted.                                                                                                                                                                 | Withdrawal Membership |
| 3   | Administrators and members can log in to the system using their ID and password. Upon logout, the system connection is terminated.                                                                                                                                            | Login/ Logout         |


## Use Case Description

#### Register Membership Description

| Actor                                                                                                                                                      | System                                                                                                                                                 |
| :--------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------- |
| the user selects the membership registration menu                                                                                                          |                                                                                                                                                        |
|                                                                                                                                                            | The system presents membership registration form                                                                                                       |
| The user enters the required information (ID, password, phone number, payment method, preferred bike type - standard/electric)1 and requests registration. |                                                                                                                                                        |
|                                                                                                                                                            | The system validates the entered information and processes the registration.                                                                           |
|                                                                                                                                                            | The system displays a message confirming successful membership registration.                                                                           |
|                                                                                                                                                            | If the entered information is invalid (e.g., incorrect format, missing required field), the system displays an error message and prompts for re-entry. |
|                                                                                                                                                            | If the entered ID is already in use, the system displays a message indicating ID duplication and prompts the user to enter a different ID.             |

#### Membership Withdrawal
| Actor                                                                                          | System                                                                            |
| :--------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------- |
| The member selects the membership withdrawal function (e.g., from a profile or settings menu). |                                                                                   |
|                                                                                                | The system displays a confirmation message and outlines the withdrawal procedure. |
| The member confirms the decision to withdraw.                                                  |                                                                                   |
|                                                                                                | The system deletes all the member's user privileges and associated data           |
|                                                                                                | The system displays a message confirming successful membership withdrawal.        |
### Login
| Actor                                                                                               | System                                                                                                                                              |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------ |
| The administrator or member enters their ID and password on the login screen and requests to log i                                                                                                                                                        |
|                                                                                                     | The system verifies the entered ID and password against registered user creden                                                                      |
|                                                                                                     | If authentication is successful, the system grants access to the user and navigates to the main system in                                           |
|                                                                                             If the entered ID or password does not match any registered credentials, the system displays an error message indicating incorrect login details. in details. |

### Logout

| Actor                                                                                | System                                                                 |
| :----------------------------------------------------------------------------------- | :--------------------------------------------------------------------- |
| The administrator or member selects the logout option (e.g., from a menu or button). |                                                                        |
|                                                                                      | The system terminates the user's current session and system connection |
|                                                                                      | The system typically redirects the user to the login screen            |


