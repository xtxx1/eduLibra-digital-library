# Sample Functional Test Cases for EduLibra

## Overview
This document provides sample functional test cases for the EduLibra platform. These test cases are designed to validate core functionalities and user workflows.

## Test Cases

### User Registration

| Test Case ID | Description                                                                   | Precondition                     | Test Steps                                                                 | Expected Result                                                                 |
|--------------|-------------------------------------------------------------------------------|----------------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| TC-001       | Verify that a new user can register with a valid email address.              | None                            | 1. Navigate to the registration page.<br/>2. Enter a valid email address and other required details.<br/>3. Submit the registration form. | User receives a confirmation email and is redirected to the login page.      |
| TC-002       | Verify that the system prevents registration with an invalid email address.   | None                            | 1. Navigate to the registration page.<br/>2. Enter an invalid email address and submit the form. | System displays an error message and registration fails.                     |

### Content Search and Filtering

| Test Case ID | Description                                                                   | Precondition                     | Test Steps                                                                 | Expected Result                                                                 |
|--------------|-------------------------------------------------------------------------------|----------------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| TC-003       | Verify that users can search for content using keywords.                      | User is logged in               | 1. Navigate to the content search page.<br/>2. Enter a keyword into the search bar.<br/>3. Execute the search. | The system returns a list of content items matching the keyword.            |
| TC-004       | Verify that users can filter content by subject and difficulty level.         | User is logged in               | 1. Navigate to the content search page.<br/>2. Apply filters for subject and difficulty level.<br/>3. Execute the search. | The system returns filtered content items based on the selected filters.   |

### Content Upload and Management

| Test Case ID | Description                                                                   | Precondition                     | Test Steps                                                                 | Expected Result                                                                 |
|--------------|-------------------------------------------------------------------------------|----------------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| TC-005       | Verify that content creators can upload new content with metadata.            | User has content creator role   | 1. Navigate to the content upload page.<br/>2. Upload a file and add metadata.<br/>3. Submit the upload form. | Content is uploaded successfully and pending review.                          |
| TC-006       | Verify that content awaiting review is not visible to regular users.         | Content is uploaded and awaiting review | 1. Log in as a regular user.<br/>2. Navigate to content search and view available content. | The newly uploaded content is not visible to regular users.                  |

### Learning Path Creation and Management

| Test Case ID | Description                                                                   | Precondition                     | Test Steps                                                                 | Expected Result                                                                 |
|--------------|-------------------------------------------------------------------------------|----------------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| TC-007       | Verify that corporate trainers can create a new learning path.                | User has corporate trainer role | 1. Navigate to the learning path management page.<br/>2. Create a new learning path and add content items.<br/>3. Save the learning path. | The new learning path is created and accessible.                              |
| TC-008       | Verify that users can track their progress through a learning path.          | User is enrolled in a learning path | 1. Log in as a user enrolled in a learning path.<br/>2. Navigate to the learning path and complete some modules. | The system accurately tracks and displays the user's progress.              |

### Subscription Management

| Test Case ID | Description                                                                   | Precondition                     | Test Steps                                                                 | Expected Result                                                                 |
|--------------|-------------------------------------------------------------------------------|----------------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| TC-009       | Verify that administrators can manage subscription plans.                    | User has administrator role     | 1. Navigate to the subscription management page.<br/>2. Modify an existing subscription plan.<br/>3. Save the changes. | The subscription plan is updated successfully in the system.                |
| TC-010       | Verify that users receive notifications prior to subscription renewal.       | User has an active subscription | 1. Simulate the approach of the subscription renewal date.<br/>2. Check user notifications. | The system sends a notification reminding the user of the upcoming renewal. |

