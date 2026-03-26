CC = gcc
CFLAGS = -O2 -Wall -Wextra -pedantic
LDFLAGS = -lpthread

all: wsl-git-daemon

wsl-git-daemon: daemon.c
	$(CC) $(CFLAGS) -o $@ $< $(LDFLAGS)

install: wsl-git-daemon
	install -m 755 wsl-git-daemon /usr/local/bin/

clean:
	rm -f wsl-git-daemon

.PHONY: all install clean
