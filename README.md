# Getting Started

### Reference Documentation

This is a sample bare metal codebase to demonstrate OAuth2 integration with spring boot application with KeyCloak as authentication provider.

### Prerequisites

- Java 21
- Maven 3.8+
- KeyCloak 25+

### Installation

1. Make sure you have KeyCloak server running on your local machine on port 8080. If not, you can download it from [here](https://www.keycloak.org/downloads).
2. Use realm-export.json to import the realm configuration in your KeyCloak server. Make sure the client secret in the realm configuration is same as the client secret provided in application.yml.
3. Add a user in the realm with username and password.

### Usage

1. Start the application.
2. In the browser, hit the URLs:
   1. `http://localhost:9090/public` to hit unprotected endpoint.
   2. `http://localhost:9090/private` to hit protected endpoint. You will be redirected to KeyCloak login page. Enter the credentials of the added user and you will be redirected back to the application.