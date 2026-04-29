## Unprotected Admin Functionality with Unpredictable URL

### Steps to Reproduce

1. First, I inspected the website using browser Inspect.
2. Then I searched for "admin" in the source code.
3. Found a hidden admin path: `/admin-Ipyisq`
4. Navigated directly to `/admin-Ipyisq` in the browser.
5. Admin panel loaded successfully without authentication.

### Vulnerability

The application uses an unpredictable URL for the admin panel but does not enforce proper authentication or access control.

### Impact

* Unauthorized users can access admin panel
* Sensitive functionality exposed

### Proof

(<img width="1366" height="768" alt="Screenshot (62)" src="https://github.com/user-attachments/assets/75bb0bd5-cbef-4d41-b665-21dad573e078" />
)
