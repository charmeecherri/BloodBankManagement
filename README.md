# BloodBankManagementAPI

Project Overview
This is a RESTful API for managing blood bank entries built with ASP.NET Core. The API supports:

CRUD operations: Create, Read, Update, Delete blood bank entries.
Pagination: Retrieve entries in a paginated format.
Search: Search entries by blood type, status, or donor name.
The project uses an in-memory list as the database and includes testing support through Swagger and Postman.

Features
CRUD Operations:
Add, view, update, and delete blood bank entries.
Pagination:
Retrieve paginated results.
Search:
Search by blood type, status, or donor name.
Swagger Integration:
Easily test the API via Swagger UI.

Setup instructions
Prerequisites
Install .NET 6 SDK.
Install an IDE like Visual Studio or VS Code.
Steps
1.Clone the repository
2.Open the project in Visual Studio.
3.Restore dependencies: dotnet restore
4.Run the project: dotnet run
5.Open your browser and navigate to url to access the Swagger UI.

Endpoints
CRUD Endpoints
POST /api/bloodbank: Add a new entry.
GET /api/bloodbank: Retrieve all entries.
GET /api/bloodbank/{id}: Retrieve an entry by ID.
PUT /api/bloodbank/{id}: Update an entry by ID.
DELETE /api/bloodbank/{id}: Delete an entry by ID.
Pagination Endpoint
GET /api/bloodbank?page={pageNumber}&size={pageSize}: Retrieve entries with pagination.
Search Endpoints
GET /api/bloodbank/search?bloodType={bloodType}: Search by blood type.
GET /api/bloodbank/search?status={status}: Search by status.
GET /api/bloodbank/search?donorName={donorName}: Search by donor name.

Testing
Using Swagger:
Access the Swagger UI at http://localhost:<port>/swagger.
Test all endpoints interactively.
Use Postman:
Import the provided sample JSON payloads.
Test each endpoint manually and capture screenshots






