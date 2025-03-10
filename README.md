Backend/Devops Project Info
Language: Go 1.23 (stdlib net/http)
An endpoint refers to the URL or URI that serves as a gateway to a particular server or application, in the computer network an endpoint can be communication endpoint or a conection point that enables communication between different devices & software components.
2.1 Client endpoints: A client endpoint is typically associated with client-server architecture, the client could be web broswer or a mobile app, communicates with the server through a designated endpoint, the client sends requests to the server through a designated endpoint.
2.2 Web API endpoints: In the realm of web developers & API's (application program interfaces) an API endpoint defines a specific URL where API request can be made, for example if you're building a weather app you might have an API endpoint that provides weather forecast in your area.
2.3 Network endpoints: In networking, a network endpoint represents a device or a software component that's apart of the network.
Network endpoints are assigned unique identifiers to facilitate communication & data exchange between them, endpoints also contribute to the security system by accessing specific resourses & functionalities.



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
