# Personal Recipes Notebook

Personal Recipes Notebook is a web application built with **ASP.NET Razor Pages** that allows users to store and manage their personal cooking recipes. The application provides basic CRUD functionality for recipes, offering a simple and structured way to keep all recipes in one place.

This project was developed as a personal project to practice web development with .NET, Razor Pages, and database integration using Entity Framework Core.

---

## What the application does

The application provides the following functionality:

- User authentication (register and login)
- Each user has access to their own personal recipe collection
- Create new recipes and save them to a personal “My Recipes” section
- Add ingredients to recipes from a predefined list of ingredients
- For each ingredient, select:
  - measurement unit (e.g. grams, milliliters, pieces)
  - quantity
- View detailed recipe information, including ingredients and preparation steps
- Edit or delete existing recipes  

---

## Technologies used

- **C# / .NET**
- **ASP.NET Razor Pages**
- **Entity Framework Core**
- **JavaScript** 

---

## Running the project locally

### Prerequisites
- .NET SDK 6 or newer
- Visual Studio (recommended) or VS Code

### Steps

1. Clone the repository:
```bash
git clone https://github.com/AndreeaBaghiut/project_personal_recipes_notebook.git

2.Open the solution file in Visual Studio.

3. Restore dependencies and build the project:
      dotnet restore
      dotnet build

4. Run the application:
      dotnet run

5. Open a browser and navigate to:
      https://localhost:5001

---
Project structure:
├── Areas/Identity/       # authentication and user management
├── Data/                 # database context
├── Migrations/           # Entity Framework migrations
├── Models/               # entities (Recipe, Ingredient, User, etc.)
├── Pages/                # Razor Pages and code-behind files
├── wwwroot/              # static files (CSS, JavaScript)
├── Program.cs            # application entry point
├── appsettings.json      # configuration and database settings
└── *.sln                 # solution file

---
Data model overview:
  -Users can have multiple recipes
  -Each recipe can contain multiple ingredients
  -Ingredients are selected from a predefined list
  -Each ingredient entry stores quantity and measurement unit
  -Relationships are handled through Entity Framework Core
