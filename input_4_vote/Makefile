VERILOG = iverilog
TARGET = input_4_vote.vcd

$(TARGET) : input_4_vote.vvp
	vvp input_4_vote.vvp

input_4_vote.vvp: input_4_vote_tb.v input_4_vote.v
	$(VERILOG) -o input_4_vote.vvp input_4_vote_tb.v input_4_vote.v

clean:
	-del $(TARGET)