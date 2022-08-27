SRC = $(wildcard *.tmasm)
BIN = $(addsuffix .tm,$(basename $(SRC)))

TMASM = tmasm

compile: $(BIN)

$(BIN): ./%.tm : ./%.tmasm
	$(TMASM) $< -o$@

clean:
	rm -r ./*.tm
	rm -r ./*.txt

all:
	@echo compile, clean
