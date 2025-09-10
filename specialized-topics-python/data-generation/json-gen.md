## Data Generation with JSON

```
Generate a sample JSON array of 10 rows of sample data. The data should include the following keys:
- employee_id (unique and random in the range 1 to 100),
- department_name (randomly assigned to one of the following departments: HR, Engineering, Sales),
- first_name,
- last_name,
- hourly_rate ($25.00 to $75.00, standard deviation of $7.65)
Use international naming conventions for the names.
```

```
Assuming the data is consumable over http://localhost:6543/employees, how would you consume this JSON data using Python? The result should produce a list of Employee objects and adhere to separation of concerns principles. Show the Employee class and a service class to fetch the data.
```

```
How would you securely handle user authentication for this service using JWT tokens? Show a completed Python solution based on the last response, using the `requests` library and best practices for JWT handling.
```




