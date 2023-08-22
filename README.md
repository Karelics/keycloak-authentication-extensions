# Keycloak extension: conditional authenticator to check if the user has SSO configured
This is a sample keycloak extension that provides the condition in the authentication flow to check whether the user has single sign-on (linked identity provider) configured.

# Usage
Set the correct keycloak version in the `pom.xml` file.
```
<keycloak.version>20.0.5</keycloak.version>
```
To build the package, execute `mvn package` command, which creates `target/deploy/authentication-extensions-module-0.1.jar` package file.

To deploy the package to keycloak, it needs to be placed in the `/opt/keycloak/providers` directory of the Keycloak and execute `build` or `start` command of Keycloak.
