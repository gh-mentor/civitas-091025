# Inventory Management System sample prompts

## SQLite

I want to use the SQLite command-line tool.
- Provide a link to download the SQLite command-line tool.
- Provide a very brief overview of the SQLite command-line tool using the documentation as a source.
- Show how to create a database named 'sql/inventory.db' using the SQLite script 'sql/scripts/inventory.sql' as the source.
- Show the command to display all tables and views.
- Show the SQL command to select all records from the 'products' table.
- Show how to exit the SQLite command-line tool.

## Data Access in Python

Help me understand how to use Python's `sqlite3` module to create a data access layer based on the inventory database.
- Show which Python packages are needed to use SQLite3.

Help me create Python classes for the following tables in the inventory database:
- products, categories, suppliers
- The entities (Supplier, Category, Product) must be represented as Python classes, each in a separate file if possible.
- The schemas for the classes must match the columns defined in the 'sql/scripts/inventory.sql' script.

Help me configure a data access layer in Python to use SQLite based on the following requirements:
- Use context managers for database connections.
- All tables and properties are mapped to the columns defined in the inventory.sql script.
- Show how to make the database path configurable for portability.

How do I ensure that the 'sql/inventory.db' database in the project will be easy to locate relative to the code?

## Web API

Help me extend a Python FastAPI project with the following requirements:
- Supports SQLite database operations.
- Provides two GET endpoints for accessing product data.
- Includes OpenAPI/Swagger for API documentation and testing.
- Configures the database path dynamically for portability.
- Implements basic error handling and relationship management using SQLAlchemy or sqlite3.
- Enforces HTTPS and integrates with the FastAPI middleware pipeline.

## Testing

I want to perform integration testing for the inventory Web API. I do not want to use the actual database in my tests. Please help me set up a new pytest project following these requirements:
- An in-memory database is created and seeded during the test setup.
- A fixture seeds the in-memory database with sample data for Products, Categories, and Suppliers, ensuring the tests have data to work with.
- The integration tests use FastAPI's TestClient to create an HTTP client for testing the API endpoints.
- Test methods validate the API's behavior against expected outcomes.





