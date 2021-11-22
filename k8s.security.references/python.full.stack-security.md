1 Defense In Depth
     
            1.1 Attack surface
            1.2 Defense in depth
            1.2.1 Security standards
            1.2.2 Best practices
            1.2.3 Security fundamentals
            1.3 Tools
            1.3.1 Staying practical
   
## Part 1 Cryptographic Foundations
     
2 Hashing
     
            2.1 What is a hash function?
            2.1.1 Cryptographic hash function properties
            2.2 Archetypal characters
            2.3 Data integrity
            2.4 Choosing a cryptographic hash function
            2.4.1 Which hash functions are safe?
            2.4.2 Which hash functions are unsafe?
            2.5 Cryptographic hashing in Python
            2.6 Checksum functions
   
3 Keyed Hashing
     
            3.1 Data authentication
            3.1.1 Key generation
            3.1.2 Keyed hashing
            3.2 HMAC functions
            3.2.1 Data authentication between parties
            3.3 Timing attacks
   
4 Symmetric Encryption
     
            4.1 What is encryption?
            4.1.1 Package management
            4.2 The cryptography package
            4.2.1 Hazardous materials layer
            4.2.2 Recipes layer
            4.2.3 Key rotation
            4.3 Symmetric encryption
            4.3.1 Block ciphers
            4.3.2 Stream ciphers
            4.3.3 Encryption modes
   
5 Asymmetric Encryption
     
            5.1 Key-distribution problem
            5.2 Asymmetric encryption
            5.2.1 RSA public-key encryption
            5.3 Nonrepudiation
            5.3.1 Digital signatures
            5.3.2 RSA digital signatures
            5.3.3 RSA digital signature verification
            5.3.4 Elliptic-curve digital signatures
   
6 Transport Layer Security
     
            6.1 SSL? TLS? HTTPS?
            6.2 Man-in-the-middle attack
            6.3 The TLS handshake
            6.3.1 Cipher suite negotiation
            6.3.2 Key exchange
            6.3.3 Server authentication
            6.4 HTTP with Django
            6.4.1 The DEBUG setting
            6.5 HTTPS with Gunicorn
            6.5.1 Self-signed public-key certificates
            6.5.2 The Strict-Transport-Security response header
            6.5.3 HTTPS redirects
            6.6 TLS and the requests package
            6.7 TLS and database connections
            6.8 TLS and email
            6.8.1 Implicit TLS
            6.8.2 Email client authentication
            6.8.3 SMTP authentication credentials
   
## Part 2 Authentication And Authorization
     
7 HTTP Session Management
     
            7.1 What are HTTP sessions?
            7.2 HTTP cookies
            7.2.1 Secure directive
            7.2.2 Domain directive
            7.2.3 Max-Age directive
            7.2.4 Browser-length sessions
            7.2.5 Setting cookies programmatically
            7.3 Session-state persistence
            7.3.1 The session serializer
            7.3.2 Simple cache-based sessions
            7.3.3 Write-through cache-based sessions
            7.3.4 Database-based session engine
            7.3.5 File-based session engine
            7.3.6 Cookie-based session engine
   
8 User Authentication
     
            8.1 User registration
            8.1.1 Templates
            8.1.2 Bob registers his account
            8.2 User authentication
            8.2.1 Built-in Django views
            8.2.2 Creating a Django app
            8.2.3 Bob logs into and out of his account
            8.3 Requiring authentication concisely
            8.4 Testing authentication
   
9 User Password Management
     
            9.1 Password-change workflow
            9.1.1 Custom password validation
            9.2 Password storage
            9.2.1 Salted hashing
            9.2.2 Key derivation functions
            9.3 Configuring password hashing
            9.3.1 Native password hashers
            9.3.2 Custom password hashers
            9.3.3 Argon2 password hashing
            9.3.4 Migrating password hashers
            9.4 Password-reset workflow
   
10 Authorization
     
            10.1 Application-level authorization
            10.1.1 Permissions
            10.1.2 User and group administration
            10.2 Enforcing authorization
            10.2.1 The low-level hard way
            10.2.2 The high-level easy way
            10.2.3 Conditional rendering
            10.2.4 Testing authorization
            10.3 Antipatterns and best practices
   
11 OAuth 2

        11.1 Grant types
        11.1.1 Authorization code flow
        11.2 Bob authorizes Charlie
        11.2.1 Requesting authorization
        11.2.2 Granting authorization
        11.2.3 Token exchange
        11.2.4 Accessing protected resources
        11.3 Django OAuth Toolkit
        11.3.1 Authorization server responsibilities
        11.3.2 Resource server responsibilities
        11.4 requests-oauthlib
        11.4.1 OAuth client responsibilities
   
## Part 3 Attack Resistance
     
12 Working With The Operating System
     
        12.1 Filesystem-level authorization
        12.1.1 Asking for permission
        12.1.2 Working with temp files
        12.1.3 Working with filesystem permissions
        12.2 Invoking external executables
        12.2.1 Bypassing the shell with internal APIs
        12.2.2 Using the subprocess module
   
13 Never Trust Input
     
        13.1 Package management with Pipenv
        13.2 YAML remote code execution
        13.3 XML entity expansion
        13.3.1 Quadratic blowup attack
        13.3.2 Billion laughs attack
        13.4 Denial of service
        13.5 Host header attacks
        13.6 Open redirect attacks
        13.7 SQL injection
        13.7.1 Raw SQL queries
        13.7.2 Database connection queries
   
14 Cross-Site Scripting Attacks
     
        14.1 What is XSS?
        14.1.1 Persistent XSS
        14.1.2 Reflected XSS
        14.1.3 DOM-based XSS
        14.2 Input validation
        14.2.1 Django form validation
        14.3 Escaping output
        14.3.1 Built-in rendering utilities
        14.3.2 HTML attribute quoting
        14.4 HTTP response headers
        14.4.1 Disable JavaScript access to cookies
        14.4.2 Disable MIME type sniffing
        14.4.3 The X-XSS-Protection header
   
15 Content Security Policy
     
        15.1 Composing a content security policy
        15.1.1 Fetch directives
        Navigation and document directives
        15.2 Deploying a policy with django-csp
        15.3 Using individualized policies
        15.4 Reporting CSP violations
        15.5 Content Security Policy Level 3
   
16 Cross-Site Request Forgery
     
        16.1 What is request forgery?
        16.2 Session ID management
        16.3 State-management conventions
        16.3.1 HTTP method validation
        16.4 Referer header validation
        16.4.1 Referrer-Policy response header
        16.5 CSRF tokens
        16.5.1 POST requests
        16.5.2 Other unsafe request methods
   
17 Cross-Origin Resource Sharing
     
        17.1 Same-origin policy
        17.2 Simple CORS requests
        17.2.1 Cross-origin asynchronous requests
        17.3 CORS with django-cors-headers
        17.3.1 Configuring Access-Control-Allow-Origin
        17.4 Preflight CORS requests
        17.4.1 Sending the preflight request
        17.4.2 Sending the preflight response
        17.5 Sending cookies across origins
        17.6 CORS and CSRF resistance
   
18 Clickjacking
     
        18.1 The X-Frame-Options header
        18.1.1 Individualized responses
        18.2 The Content-Security-Policy header
        18.2.1 X-Frame-Options versus CSP
        18.3 Keeping up with Mallory