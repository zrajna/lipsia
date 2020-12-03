
LDLIBS = -lgsl -lgslcblas -lvia3.0 -lviaio3.0 -lm -fopenmp -lz
#CFLAGS  = -g
CFLAGS  += -fopenmp


PROG = vlisa_grouped_twosample
SRC = vlisa_grouped_twosample.c ../utils/BilateralFilter.c ../utils/Hotspot.c ../utils/FDR.c ../utils/ttest.c ../utils/quantile.c 
OBJ=$(SRC:.c=.o)

${PROG}: ${OBJ}

clean:
	-rm -f *.o *~ ../utils/*.o ${PROG}
