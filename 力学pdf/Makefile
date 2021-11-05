
.PHONY:all

ith:=$(shell ls pdf/*png)
all: $(ith:%=pdf/%/txt)

pdf/%/txt:
	mkdir -p pdf/$*
	str1=$(\begin{figure}[H])
	str2=$(\centering)
	str3=$(\includegraphics[width=16cm]{)$*$(})
	str3=$(\end{figure})
	str4=$(\newpage)
	@echo $(str1) >>lixue.tex
	@echo $(str2) >>lixue.tex
	@echo $(str3) >>lixue.tex
	@echo $(str4) >>lixue.tex
	touch $@

# Delete partial files when the processes are killed.
.DELETE_ON_ERROR:
# Keep intermediate files around
.SECONDARY:

