VESC_TOOL ?= vesc_tool

all: balance.vescpkg

balance.vescpkg: balance
	$(VESC_TOOL) --buildPkg "balance.vescpkg:balance.lisp:ui.qml:0"

balance:
	@echo About to make distribution files for balance
	$(MAKE) -C $@

clean:
	rm -f balance.vescpkg
	$(MAKE) -C balance clean

.PHONY: all clean balance
