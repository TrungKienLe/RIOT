APPLICATION = gnrc_sock_udp

BOARD ?= native

RIOTBASE ?= $(CURDIR)/../..

USEMODULE += gnrc_sock_check_reuse
USEMODULE += gnrc_sock_udp
USEMODULE += gnrc_ipv6
USEMODULE += ps

CFLAGS += -DDEVELHELP
CFLAGS += -DGNRC_PKTBUF_SIZE=200
CFLAGS += -DTEST_SUITES

QUIET ?= 1

include $(RIOTBASE)/Makefile.include

test:
	./tests/01-run.py
