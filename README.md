# FULL_SUBTRACTOR
# Aim:
To simulate and synthesis full subtractor using vivado.
# Apparatus Required:
Vivado Xilinx 14.7 Spartan 6 FPGA
# Procedure:
```
STEP 1: Start the vivado software and select the name and the project.
STEP 2: Select the device family, device, package and speed.
STEP 3: Select new source in the new project and select verilog module as the source type.
STEP 4: Type the file name and module name and click next and then finish button. Type the code and save it.
STEP 5: Select the run simulation and then run behavioural simulation in the source window and click the check syntax.
STEP 6: Click the simulation to stimulate the program and give the inputs and verify the outputs as per the truth table.
STEP 7: Compare the output with the truth table.
```
# Truth Table and Circuit Diagram
![image](https://github.com/RESMIRNAIR/FULL_SUBTRACTOR/assets/154305926/351addef-f7bb-4862-9817-616a41b4c882)
![image](https://github.com/RESMIRNAIR/FULL_SUBTRACTOR/assets/154305926/906152b8-63bc-4f70-9132-6b6b4420b22d)
![image](https://github.com/RESMIRNAIR/FULL_SUBTRACTOR/assets/154305926/7d480140-153a-4a7e-a6d2-5323c6bd4974)
# Verilog Code:
```
module FS(a,b,c,difference,borrow);
input a,b,c;
output difference,borrow;
wire wl,w2,w4,w5,w6;
xor xl(w2,a,b);
xor x2 (difference,w2,c);
not nl(wl,a);
and al(w5,wl,b);
not n2(w4,w2);
and a2(w6,w4,c);
or ol (borrow,w5,w6);
endmodule
```
# Output:
![fullsubtractor](https://github.com/GauravSunehl/FULL_SUBTRACTOR/assets/166976407/7c04b52f-27e1-47d7-93fe-81b91b36efa7)
# Result:
Thus the verilog program for full subtractor has been simulated and verified successfully.

