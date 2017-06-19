# owncloud-docker

    docker service create  \
      --name owncloud3  \
      --mount type=volume,source=owncloud01,destination=/var/www/html,volume-driver=rbd  \
      --mount type=volume,source=owncloud02,destination=/etc/apache2,volume-driver=rbd  \
      --secret source=trans.pem,target=trans.pem \
      --secret source=trans.key,target=trans.key \
      --publish 8443:443  \
      --publish 81:80  \
      --network docker-network  \
      --env SSL_CERTIFICATE=trans.pem \
      --env SSL_CERTIFICATE_KEY=trans.key \
      xingjiudong/owncloud 
