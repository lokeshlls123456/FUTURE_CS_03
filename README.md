# FUTURE_CS_03 – API Security Risk Analysis

## Project Overview

This project was completed as part of the Cyber Security Internship at Future Interns.

The main objective of this task is to analyze API security risks in public APIs by identifying vulnerabilities such as:

* Missing Authentication
* Broken Authorization
* Lack of Rate Limiting
* Weak Input Validation
* Sensitive Data Exposure

This project demonstrates practical API security testing using industry-standard tools in Parrot OS.

---

## Objective

The purpose of this project is to perform a security risk analysis on sample public APIs and identify potential security weaknesses.

This assessment helps understand how insecure APIs can expose sensitive information and become vulnerable to attacks.

---

## Tools Used

* Parrot OS
* Postman
* Browser DevTools
* Curl Commands
* Public Test APIs
* GitHub

---

## Tested API

Public API used for testing:

https://jsonplaceholder.typicode.com/

Endpoints tested:

* /users
* /posts
* /comments
* /todos

---

## Security Checks Performed

### 1. Authentication Testing

Checked whether APIs require authentication such as:

* API Keys
* JWT Tokens
* OAuth Tokens

Finding:

* No authentication required

Risk Level:
Medium

---

### 2. Authorization Testing

Checked if unauthorized users can access restricted resources.

Tested by accessing multiple resources:

* /posts/1
* /posts/2
* /posts/3

Finding:

* Resources accessible without restriction

Risk Level:
High

---

### 3. Rate Limiting Testing

Performed multiple API requests to identify rate limiting.

Method:

* Repeated requests using curl
* High-frequency API calls

Finding:

* No visible rate limiting

Risk Level:
Medium

---

### 4. Input Validation Testing

Tested invalid inputs and unexpected values.

Examples:

* /posts/999999
* Invalid IDs
* Unexpected parameters

Finding:

* Weak validation in some cases

Risk Level:
Low

---

## Vulnerabilities Identified

| Vulnerability          | Risk Level | Impact              |
| ---------------------- | ---------- | ------------------- |
| Missing Authentication | Medium     | Unauthorized Access |
| Broken Authorization   | High       | Data Leakage        |
| Missing Rate Limiting  | Medium     | Abuse / DoS         |
| Weak Input Validation  | Low        | Unexpected Errors   |

---

## Recommendations

Recommended security improvements:

* Implement Authentication (JWT/OAuth)
* Apply Role-Based Access Control
* Enable API Rate Limiting
* Improve Input Validation
* Monitor API Logs
* Encrypt Sensitive Data
* Implement Proper Error Handling

---

## Project Deliverables

This repository contains:

* Security Risk Analysis Report
* Screenshots
* API Testing Results
* Documentation

---

## Screenshots Included

* Project Setup
* API Response Testing
* Postman Analysis
* Curl Request Testing
* Risk Assessment Table
* GitHub Upload

---

## Learning Outcomes

Through this project, I gained practical experience in:

* API Security Testing
* Risk Analysis
* Authentication & Authorization Testing
* Vulnerability Reporting
* Security Documentation

---

## Conclusion

APIs are a critical part of modern applications, and securing them is essential.

This project helped identify common API security risks and understand practical mitigation strategies.

Proper authentication, authorization, validation, and monitoring are essential to protect APIs from attacks.

---

## Author

ERIKALA LOKESH
Cyber Security Intern – Future Interns
