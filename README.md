Backend/Devops Project Info
Language: Go 1.23 (stdlib net/http)




    **** Go dependancy Infomation *****
        -
        -
        -
        -

Database: PostgreSQL (Docker Image)

Deployment: AWS (Ec2 + Kubernetes/k3s)

Core Feature Requirements

User Management
    Implement user registration, login and CRUD user endpoints.
    Store user data securely (hashed passwords).
    Implement endpoints to retrieve, update, and delete user information.

Session Management
    Implement session-based authentication.
    Allow users to sign out from all sessions or a specific device.
    Secure cookie handling for sessions.
    Integrate with Ory Kratos for identity management.

Route Protection + Middleware
    Use middleware to protect the User CRUD routes.
    The info of the user making the request should be accessible from all handlers.
    The middleware should validate the Kratos session token.
    Implement middleware for logging requests and errors.

Security
    Final project should be served over HTTPS.
    Implement rate limiting and input validation to prevent abuse.

Session Management
    Support for signing out all sessions for a user.
    Enable signing out specific devices by invalidating sessions.
