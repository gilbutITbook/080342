book.txt:	chapter1.txt chapter2.txt chapter3.txt
		cat chapter1.txt chapter2.txt chapter3.txt > book.txt

# This rule will work only if asciidoctor is installed on your Linux system
%.html:		%.asciidoc
		asciidoctor -o $@ $<
