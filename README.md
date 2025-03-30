## 🚀 Overview
The **Person Management System** is a simple desktop application built with **C#** and **WPF (Windows Presentation Foundation)**. It demonstrates basic CRUD (Create, Read, Update, Delete) operations for managing a list of persons using **SQL Server** as the database backend.

---

## 💡 Features
- **View Persons**: Display a list of persons from the database.
- **Add Person**: Add a new person to the database.
- **Delete Person**: Remove a selected person from the database.
- **Data Binding**: Uses **ObservableCollection** for real-time updates.
- **MVVM Architecture**: Separates UI, business logic, and data access.

---

## 🛠️ Technologies Used
- **C# / .NET Framework / .NET Core**
- **WPF (Windows Presentation Foundation)**
- **SQL Server**
- **ADO.NET** for database interaction
- **MVVM (Model-View-ViewModel) Architecture**

---

## 🚧 Getting Started

### ✅ Prerequisites
- Visual Studio 2019 or newer
- SQL Server
- .NET Framework / .NET Core
- Database connection string configured in `App.config`

### ⚙️ Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/projekt.git
   ```
2. Open the solution file (.sln) in Visual Studio.
3. Configure the database connection string in App.config:
   ```bash
   <connectionStrings>
    <add name="Projekt.Properties.Settings.PersonDBConnectionString" 
         connectionString="Your SQL Server Connection String" 
         providerName="System.Data.SqlClient" />
   </connectionStrings>
   ```
4. Run the following SQL script to create the database and table:
   ```bash
   CREATE DATABASE PersonDB;
   USE PersonDB;
   CREATE TABLE dbo.Person (
     Id INT IDENTITY PRIMARY KEY,
     Name NVARCHAR(50),
     Surname NVARCHAR(50),
     Age INT,
     Gender NVARCHAR(10)
    );
   ```
5. Build and run the application from Visual Studio.

## 🗃️ Project Structure
   ```bash
  Projekt
  ├── Models          # Data models (Person class)
  ├── Data            # Data access layer (PersonRepository)
  ├── ViewModels      # MVVM view models (MainWindowViewModel)
  ├── Views           # WPF UI views (MainWindow.xaml)
  └── App.config      # Configuration file with connection string
   ```
## 📝 Usage
1. Run the application.
2. Use the input fields to enter the person's details and click "Add" to save.
3. Select a person from the list and click "Delete" to remove them.

## 📝 License
- This project is licensed under the MIT License.
- Author: Oskar Kierys

