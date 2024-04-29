
TODAY
TODAY
github.com
https://github.com/RESMIRNAIR/ALU/assets/154305926/33dff162-59b3-44e2-886a-1ddd6e60979f
github.com
# ALU
#Aim:
To stimulate and synthesis 16bit ALU using Vivado.

# Software Required:
vivado 2023.2 software.

# Procedure:
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.
![image](https://github.com/RESMIR… Read more
1:32 PM
github.com
https://github.com/RESMIRNAIR/ALU/assets/154305926/33dff162-59b3-44e2-886a-1ddd6e60979f
github.com
# ALU
# Aim:
To stimulate and synthesis 16bit ALU using Vivado.

# Software Required:
vivado 2023.2 software.

# Procedure:
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.
# Block Diagram:
![image](https:/… Read more
1:33 PM
module bcd_to_7seg (bcd, seg);

input [3:0] bcd;

output reg [6:0] seg;

always @(bcd)

case

0: seg = 6'b0000001;

1: seg = 6'b1001111;

2: seg 6'b0010010;

3: seg = 6'b0000110;

4: seg = 6'b1001100;

5: seg = 6'b0100100;

6: seg 6'b0100000;

7: seg = 6'b0001111;

8: seg = 6'b0000000;

9: seg = 6'b0000100;

default: seg 6'b1111111;

endcase

endmodule
1:44 PM
github.com
https://github.com/RESMIRNAIR/BCD_7SEGMENT/assets/154305926/804ab8db-8637-45ac-b10f-80e77d818d61
github.com
#  BCD_7SEGMENT
# AIM
To design and simulate BCD 7 Segment using vivado.
# PROCEDURE

# BCD_7SEGMENT
![image](https://github.com/RESMIRNAIR/BCD_7SEGMENT/assets/154305926/804ab8db-8637-45ac-b10f-80e77d818d61)
# VERILOG CODE
~
//Verilog module.
module segment7(
     bcd,
     seg
    );
     
     //Declare inputs,outputs and internal variables.
     input [3:0] bcd;
     output [6:0] seg;
     reg [6:0] seg;

//always block for converting bcd digit into 7 segment format
    always @(bcd)
    begin
        case (bcd) //case statement
            0 : seg = 7'b0000001;
            1 : seg = 7'b1001111;
            2 : seg = 7'b0010010;
            3 : seg = 7'b0000110;
            4 : seg = 7'b1001100;
            5 : seg = 7'b0100100;
            6 : seg = 7'b0100000;
            7 : seg = 7'b0001111;
            8 : seg = 7'b0000000;
            9 : seg = 7'b0000100;
            //switch off 7 segment character when the bcd digit is not a decimal number.
            default : seg = 7'b1111111; 
        endcase
    end
    
endmodule
~
# OUTPUT
![326367924-68222d42-c4b3-48fa-a8ac-3d43947148aa](https://github.com/Douglas0207/BCD_7SEGMENT/assets/166375742/0caeba77-e567-4402-bfa4-43b338489cd5)

# RESULT
Thus the BCD 7 Segment is verified succcessfully.
2:15 PM


