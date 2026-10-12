SIM = list_ch01_07_eq2_sim
SRC = list_ch01_01_eq1.v list_ch01_04_eq2.v list_ch01_07_eq2_tb.v
VCD = list_ch01_07_eq2_tb.vcd

all: compile run wave
compile:
	iverilog -o $(SIM) $(SRC)
run: compile
	./$(SIM)
wave: run
	gtkwave $(VCD) &
clean:
	rm -f $(SIM) $(VCD)
