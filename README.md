```
docker run --name push1 \
-d -e MYSQL_HOST=mysql1\
 -e SPRING_PROFILES_ACTIVE=prod \
--link mysql1 \
--label=com.centurylinklabs.watchtower.enable=true \
-t ringodev/spring-web-push
```
