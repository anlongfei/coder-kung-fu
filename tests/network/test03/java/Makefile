CLIENT_BINARY_NAME := "java Client"
SERVER_BINARY_NAME := "java Server"

.PHONY: build-cli
build-cli:
	javac Client.java

.PHONY: run-cli
run-cli: build-cli
	sh tool.sh runcli $(CLIENT_BINARY_NAME)

.PHONY: stop-cli
stop-cli:
	sh tool.sh stopcli 

.PHONY: build-srv
build-srv:
	javac Server.java

.PHONY: run-srv
run-srv: build-srv
	sh tool.sh runsrv $(SERVER_BINARY_NAME)

.PHONY: stop-srv
stop-srv: 
	sh tool.sh stopsrv 

.PHONY: clean
clean:
	rm -f *.class
