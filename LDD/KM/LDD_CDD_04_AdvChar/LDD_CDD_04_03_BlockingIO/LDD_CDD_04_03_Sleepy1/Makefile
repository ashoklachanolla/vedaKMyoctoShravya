obj-m       := slpy.o

EXTRA_CFLAGS += -DDEBUG

KDIR        := /lib/modules/$(shell uname -r)/build
PWD         := $(shell pwd)

default:
	$(MAKE) -C $(KDIR) SUBDIRS=$(PWD) modules
clean:
	rm -f *.o *.ko Modules.symver* *~ *.mod.c
