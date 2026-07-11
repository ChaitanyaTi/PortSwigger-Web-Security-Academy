# Lab 02 - Unprotected Admin Functionality with Unpredictable URL

## Difficulty
Apprentice

## Category
Access Control

## Objective

Locate the hidden administrative panel and delete the user **carlos**.

---

## Lab Description

This lab contains an administrative interface that is not protected by proper authorization controls. The admin panel is located at an unpredictable URL, but its location is disclosed somewhere within the application.

---

## Vulnerability

The application relies on obscurity rather than proper authorization checks to protect administrative functionality.

Hiding administrative endpoints does not prevent attackers from discovering and accessing them.

---

## Methodology

### Step 1: Explore the Application

Reviewed the application's publicly accessible pages and resources.

### Step 2: Identify Hidden Administrative Functionality

Inspected available content and discovered a reference to an administrative endpoint.

### Step 3: Access the Admin Panel

Navigated directly to the discovered administrative interface.

### Step 4: Perform Administrative Action

Used the exposed functionality to remove the target user.

---

## Impact

An attacker can discover hidden administrative endpoints and gain unauthorized access to sensitive functionality.

Potential impacts include:

- User account manipulation
- Unauthorized administrative actions
- Data exposure
- Privilege escalation

---

## Remediation

- Implement server-side authorization checks.
- Restrict administrative functionality to authorized users only.
- Do not rely on hidden URLs for security.
- Follow the principle of least privilege.

---

## Key Learning

Security through obscurity is not a security control.

Administrative endpoints must always enforce authentication and authorization regardless of whether their URLs are publicly known.

---

## Tools Used

- Burp Suite Community Edition
- Firefox
- PortSwigger Web Security Academy

---

## Skills Learned

- Access Control Testing
- Hidden Endpoint Discovery
- Web Application Enumeration
- Privilege Escalation Concepts
- Burp Suite Navigation

---
