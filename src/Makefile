CC ?= gcc
CFLAGS ?= -static -Wall -Wextra -Werror
TARGET = hello
SRC_FILES = hello.c


all: ## Compile hello.c
	$(CC) $(CFLAGS) -o $(TARGET) $(SRC_FILES)

clean: ## Cleanup
	rm $(TARGET)

# Shameless stolen from -> https://brokenco.de/2019/04/22/self-describing-make.html
help: ## Display this help text
	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
