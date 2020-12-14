### springboot集成keycloak mysql5.7
##### 因为编码问题，先初始化mysql，然后把mysql的编码转化为utf8

##### 启动mysql实例
````
docker run -d --name mysql \
	--net keycloak-network \
	-p 3306:3306 \
	-e MYSQL_DATABASE=keycloak \
	-e MYSQL_USER=keycloak \
	-e MYSQL_PASSWORD=keycloak \
	-e MYSQL_ROOT_PASSWORD=123456 \
	mysql:5.7
````

