# FULL_SUBTRACTOR

# Aim:
To simulate and synthesis full subtractor using vivado.

# Apparatus Required:
vivado software.

# Procedure:
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed. 

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it. 

STEP:5 Select the run simulation adn then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table. 

STEP:7 Select the Implementation in the Sources Window and select the required file in the Processes Window.

STEP:8 Select Check Syntax from the Synthesize XST Process. Double Click in the Floorplan Area/IO/Logic-Post Synthesis process in the User Constraints process group. UCF(User constraint File) is obtained. 

STEP:9 In the Design Object List Window, enter the pin location for each pin in the Loc column Select save from the File menu.

STEP:10 Double click on the Implement Design and double click on the Generate Programming File to create a bitstream of the design.(.v) file is converted into .bit file here.

STEP:12 Load the Bit file into the SPARTAN 6 FPGA 

STEP:11 On the board, by giving required input, the LEDs starts to glow light, indicating the output.

# Truth Table and Circuit Diagram
![image](https://github.com/RESMIRNAIR/FULL_SUBTRACTOR/assets/154305926/351addef-f7bb-4862-9817-616a41b4c882)
![image](https://github.com/RESMIRNAIR/FULL_SUBTRACTOR/assets/154305926/906152b8-63bc-4f70-9132-6b6b4420b22d)
![image](https://github.com/RESMIRNAIR/FULL_SUBTRACTOR/assets/154305926/7d480140-153a-4a7e-a6d2-5323c6bd4974)

# Program
module full_sub(a,b,bin,diff,borrow);

input a,b,bin;

output diff,borrow;

assign diff=a^b^bin;

assign borrow=(~a&b)|((~a|b)&bin);

endmodule

# Output
![image](https://github.com/Shaiksushma123/FULL_SUBTRACTOR/assets/159005642/d9049022-fbd1-4e96-b2d8-c1364b7a2cd0)

# Result:
Thus the verilog program for full subtractor has been simulated and verified successfully using logic truth table.


