# Go OAuth2 File Server

A file server with Google OAuth2 authentication.

## Features
- Serves static files from a configurable directory
- Requires Google OAuth2 authentication
- Session-based authentication
- Configurable server port

## Prerequisites
- Go 1.23.3 or higher
- A Google Cloud Project with OAuth2 credentials
- At least `GOOGLE_CLIENT_ID` and `GOOGLE_CLIENT_SECRET` in your environment

## Configuration
- `GOOGLE_CLIENT_ID`: Your Google OAuth client ID (required)
- `GOOGLE_CLIENT_SECRET`: Your Google OAuth client secret (required)
- `SERVE_DIR`: Directory to serve files from (default: "static")
- `SERVER_PORT`: Port to run the server on (default: 8080)
- 
## Running the Server

1. Clone the repository:

```bash
git clone https://github.com/yourusername/go-oauth-fileserver.git
cd go-oauth-fileserver
```

2. Build and run the server:

```bash
go build
./go-oauth-fileserver
```

The server will start on the configured port (default: 8080)

## Usage

Access the server at http://localhost:8080. You will be redirected to Google login if not authenticated. After successful authentication, you can access files in the configured directory
