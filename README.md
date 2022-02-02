# keycloak-theme

Theme for FDPG-Style Login Page.

### Deploying Theme
To deploy the themes you need to create a JAR archive with the theme resources.

>jar cf FDPG.jar theme/ META-INF/

on your Terminal to create a JAR file with the name "FDPG" and the theme and META-INF files in it.

Then copy the newly created JAR file to the deployments directory of your keycloak container

>docker cp /path/to/FDPG.jar yourkeycloakcontainer:/opt/jboss/keycloak/standalone/deployments/

And select the login theme "FDPG" from the dropdown menu in the keycloak admin console.
