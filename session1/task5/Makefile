# Task 5 Makefile

CFLAGS = -g
EXECS = factorial vars


make:
	gcc $(CFLAGS) factorial.c -o factorial

clean:
	@rm -f $(EXECS)
	@rm -rf $(patsubst %,%.dSYM,$(EXECS))   # for clang on Macs

.PHONY: clean help
