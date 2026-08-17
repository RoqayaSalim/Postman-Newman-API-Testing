# Postman Newman API Testing

This repository contains automated API test scripts and execution reports for The Movie Database (TMDB) API, tested using Postman and executed via Newman with an HTML report.

## 📁 Repository Files

- **The_Movie_Database_Api.postman_collection.json**: The Postman collection containing API requests and JavaScript test scripts.
- **TMDB_API.postman_environment.json**: The environment variables configuration file.
- **bug-report.html**: The automated test execution HTML report generated using Newman (htmlextra reporter).

## 🛠️ Tools & Technologies
- **Postman**: For creating API requests and writing test scripts using JavaScript.
- **Newman**: Command-line collection runner for Postman.
- **Newman-Reporter-Htmlextra**: For generating detailed, interactive test execution reports.

## 🚀 How to Run Tests Locally

Make sure Node.js and Newman are installed, then run the following command in your terminal:

```bash
newman run The_Movie_Database_Api.postman_collection.json -e TMDB_API.postman_environment.json -r htmlextra --reporter-htmlextra-export bug-report.html
```
