# owncloud-docker

<<<<<<< HEAD
    docker service create  \
      --name NAME  \
      --mount type=volume,source=$VOLUME01,destination=/var/www/html,volume-driver=$VOLUME_DRIVER  \
      --mount type=volume,source=$VOLUME02,destination=/etc/apache2,volume-driver=$VOLUME_DRIVER  \
      --secret source=$SSL_CERTIFICATE,target=$SSL_CERTIFICATE \
      --secret source=SSL_CERTIFICATE_KEY,target=SSL_CERTIFICATE_KEY \
      --secret source=SSL_CERTIFICATE_CRT,target=SSL_CERTIFICATE_CRT \
      --publish 8443:443  \
      --publish 81:80  \
      --network docker-network  \
      --env SSL_CERTIFICATE=$SSL_CERTIFICATE \
      --env SSL_CERTIFICATE_KEY=$SSL_CERTIFICATE_KEY \
      --env SSL_CERTIFICATE_CRT=$SSL_CERTIFICATE_CRT \
      xingjiudong/owncloud
=======
>>>>>>> aa75c9bc8e51b3356e3e89d72987e8658ab210cc
