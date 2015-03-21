#Compile for AR.Drone ARM: make ARM=1

ifdef ARM
	#arm-none-linux-gnueabi-gcc
CC      := arm-linux-gnueabi-gcc
TARGET  := helloworld_arm

else
CC      := gcc
TARGET  := helloworld
endif
SRCS    := helloworld.c

CCFLAGS = -std=gnu99  -static -Wall -Werror 
CCFLAGS+= -ggdb

.PHONY: all clean distclean 
all: $(TARGET)

$(TARGET):
	${CC} ${CCFLAGS} -o $@ $(SRCS)

clean:: 
	-rm -f ${TARGET}

distclean:: clean
