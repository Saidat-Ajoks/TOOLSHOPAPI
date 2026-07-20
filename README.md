# Toolshop API Automation

## Project Description

This project contains API automation tests for the Practice Software Testing Toolshop API using Postman, Newman, and GitHub Actions.

## Tools Used

- Postman
- Newman
- Newman HTML Extra Reporter
- GitHub
- GitHub Actions

## Project Structure

- Postman Collection
- Environment File
- Newman HTML Report
- GitHub Actions Workflow

## How to Run

Install Newman:

```bash
npm install -g newman
```

Run the collection:

```bash
newman run Toolshop API.postman_collection.json
```

Generate HTML report:

```bash
newman run Toolshop API.postman_collection.json -r htmlextra --reporter-htmlextra-export newman/report.html
```

## GitHub Actions

A GitHub Actions workflow is included to automatically run the Postman collection using Newman whenever changes are pushed to the repository.

## Note

This project uses the public Practice Software Testing demo API.

Some tests may fail because:

- The demo API data changes frequently.
- Authentication tokens may expire.
- Some endpoints require authorization.
- The public API may return different responses during automated execution.

The GitHub Actions workflow executes successfully, but some test assertions may fail due to the behavior of the public demo API.

## Author

Ajoke Saidat
