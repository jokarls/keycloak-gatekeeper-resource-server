# keycloak-gatekeeper-resource-server

This repo shows how to configure Keycloak Gatekeep as a resources server for protecting a web service.

Add 127.0.0.1 keycloak to your hosts file. Gatekeeper validates the *iss* of the token so hostnames need to match.
