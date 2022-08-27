SRC = $(wildcard *.tmasm)
BIN = $(addsuffix .tm,$(basename $(SRC)))

TMASM = tmasm

compile: $(BIN)

$(BIN): ./%.tm : ./%.tmasm
	$(TMASM) $< -o$@

clean:
	rm -r ./*.tm

all:
	@echo compile, clean
