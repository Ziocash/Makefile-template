bin_objects=$(patsubst %.c, %.o, $(wildcard ../src/*.c))

include mk/*.mk


.PHONY: all static clean

all: static

static: $(bin_objects)
	$(AR) rcs libcompiled.a $^

clean:
	$(RM) $(bin_objects) *.so *.a