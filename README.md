## Compilación
javac -d . Hello.java Server.java  Client.java 

## Levantar el servicio en el background
rmiregistry &

## Activar al servidor
java -classpath . -Djava.rmi.server.codebase=file:. example.hello.Server

## Activar al cliente
java  -classpath . example.hello.Client

