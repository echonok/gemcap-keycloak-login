Find the keycloak container ID

    sudo docker ps -a

Connect to docker to find the keycloak container ID

    sudo docker exec -it ${container_ID} bin/bash

Copy theme into the keycloak theme folder

    sudo docker cp gemcap-keycloak-login/. ${container_ID}:/opt/keycloak/themes

Restart the docker keycloak container

    sudo docker restart ${container_ID}
