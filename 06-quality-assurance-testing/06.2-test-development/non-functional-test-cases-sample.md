# Sample Non-Functional Test Cases for EduLibra

## Overview
This document provides sample test cases for non-functional testing of the EduLibra platform, covering performance, security, usability, and compatibility aspects.

## Test Cases

### Performance Testing

| Test Case ID | Description                                                                   | Precondition                     | Test Steps                                                                 | Expected Result                                                                 |
|--------------|-------------------------------------------------------------------------------|----------------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| TC-011       | Verify that the system can handle 10,000 concurrent users.                   | System is deployed on staging environment | 1. Use load testing tools to simulate 10,000 concurrent users.<br/>2. Monitor system performance metrics. | The system maintains response times under 2 seconds without errors.          |
| TC-012       | Verify that the search functionality returns results within 2 seconds.       | Large dataset of content is available in the system | 1. Execute search queries with varying complexity.<br/>2. Measure response times. | Search results are returned within 2 seconds for all queries.              |

### Security Testing

| Test Case ID | Description                                                                   | Precondition                     | Test Steps                                                                 | Expected Result                                                                 |
|--------------|-------------------------------------------------------------------------------|----------------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| TC-013       | Verify that user data is encrypted in transit and at rest.                   | User data is present in the system | 1. Inspect network traffic and database storage for encryption.<br/>2. Attempt unauthorized data access. | User data is encrypted and inaccessible without proper authorization.       |
| TC-014       | Verify that the system prevents SQL injection attacks.                      | Application is configured for testing | 1. Attempt SQL injection through input fields.<br/>2. Monitor system response. | The system blocks injection attempts and logs security events.              |

### Usability Testing

| Test Case ID | Description                                                                   | Precondition                     | Test Steps                                                                 | Expected Result                                                                 |
|--------------|-------------------------------------------------------------------------------|----------------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| TC-015       | Verify that the platform complies with WCAG 2.1 accessibility standards.     | Platform is deployed with sample content | 1. Navigate through the platform using screen readers and keyboard-only inputs.<br/>2. Check for compliance with accessibility guidelines. | The platform is fully accessible and complies with WCAG 2.1 standards.      |
| TC-016       | Verify that the platform interface supports multiple Indian languages.        | Platform is configured with multilingual support | 1. Change the interface language to different Indian languages.<br/>2. Verify the correct display and functionality. | The platform interface correctly displays and functions in selected languages. |

### Compatibility Testing

| Test Case ID | Description                                                                   | Precondition                     | Test Steps                                                                 | Expected Result                                                                 |
|--------------|-------------------------------------------------------------------------------|----------------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| TC-017       | Verify that the platform functions correctly on different web browsers.      | Platform is accessible via URL   | 1. Access the platform using various browsers (Chrome, Firefox, Safari, Edge).<br/>2. Navigate through key features. | The platform functions correctly and consistently across all browsers.      |
| TC-018       | Verify that the platform functions correctly on mobile devices.              | Platform is accessible via URL   | 1. Access the platform using various mobile devices and screen sizes.<br/>2. Navigate through key features. | The platform is responsive and functions correctly on all mobile devices.   |

