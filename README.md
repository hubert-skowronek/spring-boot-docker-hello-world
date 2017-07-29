# Hello World

Dockerized Spring Boot simple Hello World application.

<h2>Running the app</h2>
<code>$ docker run -p 8080:8080 -t ${docker.image.prefix}/${artifactId}</code>
<h2>Debugging</h2>
Use JPDA transport:

<code>$ docker run -e "JAVA_OPTS=-agentlib:jdwp=transport=dt_socket,address=5005,server=y,suspend=n" -p 8080:8080 -p 5005:5005 -t ${docker.image.prefix}/${artifactId}</code>