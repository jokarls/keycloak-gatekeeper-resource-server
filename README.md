# keycloak-gatekeeper-resource-server

This repo shows how to configure Keycloak Gatekeep as a resources server for protecting a web service.

Add the following line to your hosts file.

`127.0.0.1  keycloak`

Gatekeeper validates the *iss* of the token so hostnames need to match.

This sample also requires a client called *frontend* (with authorization code flow) to be added in Keycloak. Requests to *localhost:3000* can be performed with **Postman**. Requests without a valid token will return *401* and requests with valid tokens will return *200*.
