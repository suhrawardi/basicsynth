###########################################################################
# Makefile for BasicSynth example02
#
# "make new" rebuilds all executables
# "make clean" removes the executable images from $(BSBIN)
#
# Dan Mitchell (http://basicsynth.com)
###########################################################################
include ../../BasicSynth.cfg

.PHONY: new clean

EXENAME=$(BSBIN)/example02$(EXE)

$(EXENAME): main.cpp $(CMNLIB)
	$(CPP) $(CPPFLAGS) -o $@ main.cpp $(CMNLIB) -lm

new: clean $(EXENAME)

clean:
	-rm -f $(EXENAME)

main.cpp: $(BSINC)/SynthDefs.h $(BSINC)/WaveFile.h
