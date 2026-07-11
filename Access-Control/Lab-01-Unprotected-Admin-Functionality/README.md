# Lab 01 - Unprotected Admin Functionality

## Difficulty
Apprentice

## Category
Access Control

## Objective
Delete the user "carlos" by accessing an exposed administrative panel.

## Vulnerability
Administrative functionality was accessible without proper authorization checks.

## Methodology

1. Explored the application.
2. Identified exposed administrative functionality.
3. Accessed the administrative interface.
4. Deleted the target user.

## Impact
Attackers can gain unauthorized administrative access and perform privileged actions.

## Remediation

- Implement server-side authorization.
- Restrict access to administrative endpoints.
- Apply least privilege principles.

## Skills Learned

- Access Control Testing
- Forced Browsing
- Privilege Escalation Concepts
- Burp Suite Usage
