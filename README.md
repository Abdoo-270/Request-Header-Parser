# Request Header Parser Microservice

The Request Header Parser Microservice is a simple Node.js Express API that extracts and provides information from the headers of incoming HTTP requests. Specifically, it returns details about the client's IP address, preferred language, and software information.

## How to Use

To retrieve information from the HTTP headers, make a GET request to the /api/whoami endpoint. This endpoint analyzes the incoming request's headers and responds with a JSON object containing the following details:

```json
{
  "ipaddress": "Your IP Address",
  "language": "Your Preferred Language",
  "software": "Your Software Information"
}
```

- ipaddress: Represents the IP address of the client making the request.
- language: Indicates the preferred language of the client's browser based on the "Accept-Language" header.
- software: Provides information about the client's browser or user-agent based on the "User-Agent" header.

## Usage Example

- Retrieve IP Address, Language, and Software
  Make a GET request to /api/whoami. The response will include the client's IP address, preferred language, and software information.

Example Request:
GET /api/whoami
Example Response:

```json
{
  "ipaddress": "192.168.1.100",
  "language": "en-US",
  "software": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/94.0.4606.81 Safari/537.36"
}
```

## Deployment

This Request Header Parser Microservice API is currently deployed and accessible via the following link:

https://fcc-request-header-parser.onrender.com

## Author

Abdelrahman Mohammed
