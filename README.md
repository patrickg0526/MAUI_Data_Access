# MAUI_Data_Access

A .NET MAUI app that stores people in a local SQLite database using a Data Access Layer.

- `Models/Person.cs`: data model (ID, FirstName, LastName, DoB) mapped to the People table
- `Models/DatabaseConstants.cs`: database file name, open flags, and path
- `DataAccess/PersonData.cs`: DAL with CRUD methods (get all, get by ID, save, delete) using sqlite-net-pcl
- `MainPage`: entry form with validation (required names, no future birth date) and a CollectionView bound to the saved people
