Backend/Devops Project Info
Language: Go 1.23 (stdlib net/http)
An endpoint refers to the URL or URI that serves as a gateway to a particular server or application, in the computer network an endpoint can be communication endpoint or a conection point that enables communication between different devices & software components.
2.1 Client endpoints: A client endpoint is typically associated with client-server architecture, the client could be web broswer or a mobile app, communicates with the server through a designated endpoint, the client sends requests to the server through a designated endpoint.
2.2 Web API endpoints: In the realm of web developers & API's (application program interfaces) an API endpoint defines a specific URL where API request can be made, for example if you're building a weather app you might have an API endpoint that provides weather forecast in your area.
2.3 Network endpoints: In networking, a network endpoint represents a device or a software component that's apart of the network.
Network endpoints are assigned unique identifiers to facilitate communication & data exchange between them, endpoints also contribute to the security system by accessing specific resourses & functionalities.
Session based authenication: Is a stateful authenication method used during sessions for the client and this keep track of the authenication of the user, the user puts their info into the browser which goes to server if the info is correct, usernames & emails are required then a session is created with a session ID.
Ory Kratos is to identify user management & authentication system, Ory Kratos is a open source service that provides a quick efficient way to work & it's a safe database that clients & businesses can use alike.
Middleware: Is software that's use to bridge the gap between applications & operating rating system, middleware works as a hidden translation layer that connects tools, databases, & others technologies, single system then provides a unified service to it's user, middleware is also known as plumbing because it's a pipeline.
Enterprise middleware: Is what the software companies use for their businesses.
Platform middleware: Platform middleware supports application development.
Middleware: Middleware works by using common messaging frameworks middleware makes possible to link several application & systems simultaneously.
Hypertext transfer protocol aka HTTP is the secure version which the primary protocol used to send data between a web browser & a website, HTTPS is encrypted in order to increase security of the data transfer.
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
