# Broken Access Control via Cookie Manipulation

## Overview
This project demonstrates a Broken Access Control vulnerability where user role can be modified via client-side cookie manipulation.

## Environment
- Lab / Test Application (no real production system)
- Browser: Chrome DevTools

## Vulnerability Description
The application stores user role information in a cookie. By changing the cookie value from normal user to admin, unauthorized access to the admin panel was achieved.

## Steps to Reproduce
1. Login as a normal user
2. Open browser DevTools (Inspect → Application tab)
3. Locate the cookie storing role information
4. Change value from `user` → `admin`
5. Refresh the page
6. Admin panel access granted

## Impact
- Unauthorized admin access
- Broken authorization control
- Sensitive operations exposed

## Screenshots
(<img width="1366" height="768" alt="Screenshot (65)" src="https://github.com/user-attachments/assets/97ebd486-7c49-4e37-9c71-4c9615c2fbc4" />
)

## Fix Recommendation
- Do not store role in client-side cookies
- Always validate roles on server-side
- Use secure session/JWT with proper verification

## Disclaimer
This project is for educational purposes only and performed in a controlled lab environment.
