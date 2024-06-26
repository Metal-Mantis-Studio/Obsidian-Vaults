Open Authorisation (OAuth) is an open standard for secure and delegated access to protected resources. It can provide permission to third-party applications without the need to share credentials.

1. Client Registration with the authorisation server
2. Authorisation Request initiated by the client redirecting the user to the authorisation servers authentication endpoint where they log in and grant permissions
3. User consents the requested permissions, on success, an authorisation code or access token is generated and provided
4. Access Token Request is sent to the token endpoint where the authorisation server validates the code and issues an access token on validation
5. Resource Access using the access token instead of any credentials