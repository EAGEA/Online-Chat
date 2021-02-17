# Online-Chat

An online chat for several users using Java RMI.

## Instructions

First of all you need to compile the source code:

```console
user:~/Online-Chat/ $ make
```

Next you need first to start the server. To do this you have
to execute the following commands:

```console
user:~/Online-Chat/ $ rmiregistry &
user:~/Online-Chat/ $ javac -d classes\
					  -cp .:classes:lib/Chat.jar
					  src/Server.java
```

Then to start a user connection:

```console
user:~/Online-Chat/ $ rmiregistry &
user:~/Online-Chat/ $ javac -d classes\
					  -cp .:classes:lib/Chat.jar
					  src/Client.java localhost 
```
