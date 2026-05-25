# API Security Assessment Report

## Project Overview
This project focuses on performing an **API Security Assessment** on public/demo APIs to identify common security vulnerabilities, authentication weaknesses, and misconfigurations based on the **OWASP API Security Top 10 (2023)** framework.

The assessment was conducted in an ethical and controlled manner using public APIs and documentation-based testing. The objective was to understand API security risks, assess authentication mechanisms, inspect HTTP security headers, and recommend remediation strategies.

---

## Objectives
- Analyze public/demo APIs securely
- Identify common API security vulnerabilities
- Evaluate authentication and authorization mechanisms
- Inspect API request/response behavior
- Assess HTTP security headers
- Map findings to **OWASP API Security Top 10**
- Provide remediation recommendations and best practices

---

## Scope of Assessment
The assessment included testing of the following public/demo APIs:

### APIs Tested
1. **JSONPlaceholder API**
2. **ReqRes API**
3. **Swagger PetStore API**
4. **HTTPBin API**

### In-Scope Activities
Public API testing  
Documentation-based analysis  
Safe GET/POST requests  
Header inspection  
Authentication testing  
Security configuration review  

### Out-of-Scope Activities
 Exploitation attempts  
 Bypassing authentication  
 DoS/Flooding attacks  
 Production/private systems testing  

---

## Tools Used

### API Testing & Inspection
- **Postman**
- **Insomnia**
- **Browser DevTools**
- **curl**

### Security Analysis
- **OWASP API Security Top 10 (2023)**
- HTTP Header Analysis
- Authentication & Authorization Testing

### Documentation
- Microsoft Word
- PDF Documentation
- GitHub

---

## Methodology
The project followed a structured API security assessment process:

### 1. API Discovery
- Identified publicly available/demo APIs
- Reviewed API documentation

### 2. Endpoint Testing
- Tested API endpoints using Postman and Insomnia
- Observed responses and request behavior

### 3. Authentication Analysis
- Checked token validation
- Tested access control
- Verified authorization handling

### 4. HTTP Security Header Review
- Inspected headers such as:
  - Content-Security-Policy
  - Strict-Transport-Security
  - X-Frame-Options
  - X-Content-Type-Options

### 5. Risk Classification
Findings were categorized as:

- Critical
- High
- Medium

### 6. Remediation Planning
Suggested fixes and secure development recommendations.

---

## Key Findings

The assessment identified **16 vulnerabilities** across four APIs.

### Critical Findings
- Broken Authentication
- IDOR (Insecure Direct Object Reference)
- Missing Authentication Controls

### High Severity Findings
- Missing Rate Limiting
- Weak Token Management
- Wildcard CORS Configuration
- Sensitive Data Exposure

### Medium Severity Findings
- Missing Security Headers
- Server Information Disclosure
- Legacy API Versions Accessible

---

##  OWASP API Security Mapping
The vulnerabilities aligned with:

- **API1 – Broken Object Level Authorization**
- **API2 – Broken Authentication**
- **API4 – Unrestricted Resource Consumption**
- **API8 – Security Misconfiguration**
- **API9 – Improper Inventory Management**

---

##  Security Recommendations
- Implement JWT authentication with token expiry
- Enforce authentication on protected endpoints
- Add object-level authorization checks
- Implement rate limiting
- Remove sensitive fields from API responses
- Restrict CORS to trusted origins
- Add security headers globally
- Decommission outdated API versions

---


##  Evidence Included
- API request/response screenshots
- Authentication testing results
- Header analysis screenshots
- Security findings documentation
- Risk classification tables

---

##  Ethical Considerations
This project was conducted strictly for **educational and security awareness purposes**.

- Only public/demo APIs were tested.
- No exploitation attempts were performed.
- No unauthorized systems were targeted.
- All testing followed ethical cybersecurity practices.

---

## Author
**Tanishq Nougrahiya**  
Cybersecurity Enthusiast | Vulnerability Assessment | API Security



---

## Acknowledgment
Special thanks to public API providers and the **OWASP API Security Top 10** framework for enabling secure learning and practical security assessment experience.
