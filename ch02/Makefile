SIM = list_ch02_03_eq2_sim
SRC = list_ch02_01_eq1.v list_ch02_02_eq2.v list_ch02_03_eq2_tb.v
VCD = list_ch02_03_eq2_tb.vcd

all: compile run wave
compile:
	iverilog -o $(SIM) $(SRC)
run: compile
	./$(SIM)
wave: run
	gtkwave $(VCD) &
clean:
	rm -f $(SIM) $(VCD)
