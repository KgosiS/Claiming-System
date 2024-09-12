# Contract Monthly Claim System (CMCS)

## Project Overview

The **Contract Monthly Claim System (CMCS)** is a WPF application designed to streamline the process of submitting and approving monthly claims for Independent Contractor (IC) lecturers. The system is user-role-based and includes interfaces for Lecturers, Programme Coordinators, Academic Managers, and Admins.

### Features:
- **Lecturers**: 
  - Submit claims.
  - Upload supporting documents.
  - Track the status of their claims.
- **Coordinators and Managers**: 
  - View pending claims.
  - Approve or reject claims.
  - View and download supporting documents.
- **Admin**:
  - Manage users, roles, and system settings.

---

## Installation

### Prerequisites
- **.NET Framework 4.8** or higher.
- **Visual Studio** with WPF development components installed.
- **SQLite** or a relational database for user authentication and claim tracking (can be extended based on requirements).

### Steps to Run the Project
1. Clone the repository:
    ```bash
    git clone [https://github.com/KgosiS/CMCS.git](https://github.com/RC-Pretoria-Campus/part-1-KgosiS/tree/main)
    ```

2. Open the project in Visual Studio:
   - Open `CMCS1.sln` using Visual Studio.
   
3. Restore NuGet Packages:
   - Navigate to `Tools` > `NuGet Package Manager` > `Manage NuGet Packages for Solution`.
   - Restore all required packages.

4. Build and run the project:
   - Press `F5` or click `Start` to build and run the application.
   - You will see the **Welcome Window**, where you can log in or register as a user.

---

## Usage

### 1. **Login & Registration**
   - On application startup, you will be prompted to either log in or register.
   - The registration form collects your name, surname, employee ID, and role (Lecturer, Admin, Coordinator, Manager).
   - After successful login, the system will redirect you to the appropriate dashboard based on your role.

### 2. **Lecturer Dashboard**
   - Submit monthly claims by filling out a form.
   - Upload any supporting documents required.
   - Track the status of submitted claims, which will display as "Pending", "Approved", or "Rejected".

### 3. **Coordinator & Manager Dashboard**
   - View all submitted claims in a table format with status indicators.
   - Approve or reject claims with a single click.
   - View and download supporting documents for each claim.

### 4. **Admin Dashboard**
   - Manage users: create, delete, or update users and assign roles.
   - Manage system settings.

---

## Project Structure

- `MainWindow.xaml`: The main welcome window with navigation options to login or register.
- `LoginWindow.xaml`: The login window where users can input their credentials.
- `RegisterWindow.xaml`: The registration window where new users can sign up.
- `LecturerWindow.xaml`: The interface for lecturers to submit and track claims.
- `CoordinatorWindow.xaml`: The interface for coordinators to verify and approve claims.
- `ManagerWindow.xaml`: The interface for managers to approve/reject claims and view documents.
- `AdminWindow.xaml`: The admin interface for managing the application.
- `App.xaml`: Defines global application settings.

---


## Technologies Used

- **WPF**: Windows Presentation Foundation for building the user interface.
- **C#**: The programming language used for the application logic.

---

## Future Enhancements
- Implement database connectivity for user authentication and claim tracking.
- Add email notifications for claim status updates.
- Enhance the UI with more advanced styles and animations.
- Add role-based permissions to restrict access to certain features.

---


## Contact
For any inquiries or support, please contact **Kgosi Sebako** at [sebakokgosi@gmail.com].
