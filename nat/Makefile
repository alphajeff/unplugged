SRC = nat
OBJ = $(SRC)-en.pdf
OBJ_CN = $(SRC)-zh-cn.pdf
TEX = xelatex

.PHONY: all

all: tex

image:
	$(MAKE) -C img

tex: $(OBJ) $(OBJ_CN)

%.pdf: %.tex image
	$(TEX) $<
	$(TEX) $<

clean:
	rm -f *.4ct *.4tc *.aux *.css *.dvi *.html
	rm -f *.idv *.lg *.log *.out *.pdf *.tmp *.xref *.cache *.zip *~
