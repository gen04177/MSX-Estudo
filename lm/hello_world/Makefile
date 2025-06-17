INFILE=hello.asm
OUTFILE=hello
PASMO=pasmo
RM=rm

.PHONY: default clean

default:
	${PASMO} -d \
             -v \
             -1 \
             --err \
            ${INFILE} ${OUTFILE}.rom |\
            tee ${OUTFILE}.log 2> ${OUTFILE}.err

clean:
	${RM} -f ${OUTFILE}.rom ${OUTFILE}.log ${OUTFILE}.err