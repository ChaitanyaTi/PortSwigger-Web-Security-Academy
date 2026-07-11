# Lab 03 - User Role Controlled by Request Parameter

## Difficulty
Apprentice

## Category
Access Control

## Objective

Delete the user **carlos** by gaining access to administrative functionality through manipulation of a user-controlled request parameter.

---

## Lab Description

This lab contains an admin panel whose access is controlled by a request parameter. By modifying application behavior, it is possible to obtain administrative privileges and perform privileged actions.

---

## Vulnerability

The application trusts a client-controlled parameter to determine user privileges.

Authorization decisions should never rely on data that can be modified by the client.

---

## Methodology

### Step 1: Analyze Application Behavior

Examined requests and responses using Burp Suite.

### Step 2: Identify Authorization Parameter

Discovered a request parameter influencing user role assignment.

### Step 3: Modify Request

Manipulated the parameter and resent the request.

### Step 4: Access Administrative Functionality

Successfully accessed administrative features.

### Step 5: Delete Target User

Used the available functionality to remove the target account.

---

## Impact

An attacker can elevate privileges and gain unauthorized administrative access.

Potential consequences include:

- Account takeover
- User management abuse
- Sensitive data exposure
- Complete compromise of application functionality

---

## Remediation

- Perform authorization checks on the server side.
- Never trust client-controlled parameters for role assignment.
- Validate user permissions against trusted backend data.
- Apply role-based access control (RBAC).

---

## Key Learning

Client-side controls are not security controls.

Authorization decisions must always be enforced by the server.

---

## Tools Used

- Burp Suite Community Edition
- Firefox
- PortSwigger Web Security Academy

---

## Skills Learned

- Access Control Testing
- Parameter Tampering
- Authorization Bypass Testing
- Burp Repeater Usage
- Web Application Security Assessment

---
