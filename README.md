# Samsungpdtraining
PD training 
# Nihar_Pd_training
This github repository summarizes the progress made in the samsung pd training. Quick links:

- [Day-0-Installation](#day-0-Installation)


## Day-0-Installation

	
 <details>
 <summary> icc2 tool </summary>

     
Below is the screenshot showing the successful launch icc2:
Synopsys ICC2 is an advanced IC design tool automating physical layout generation. It optimizes placement, routing, power, and timing, ensuring efficient and manufacturable chip designs. Hierarchical, multi-domain support enhances its utility.
<img width="1085" alt="snapshot2" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8553d133af27693fa09b05956ff915839704399f/snapshot2.png">


</details>


<details>

 
 <summary> lc tool </summary>

Below is the screenshot showing the successful launch lc:
Synopsys Library Compiler is an essential EDA tool for semiconductor design. It creates optimized cell libraries, enhancing chip performance, power efficiency, and area utilization. It's pivotal in crafting efficient building blocks for IC designs.
<img width="1085" alt="snapshot1" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/fec3cd79f23c12bd75fbffcdec0799ecf779cb5b/snapshot1.png">

</details>


<details>
 <summary> dc tool </summary>

Below is the screenshot showing the successful launch dc:
Synopsys Design Compiler (DC) is a prominent EDA tool for semiconductor design. It translates Register Transfer Level (RTL) descriptions into gate-level representations, optimizing for power, area, and performance. DC plays a crucial role in efficient chip synthesis and meeting design goals.
<img width="1085" alt="snapshot3" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e522a90d26319118b401e2a043af682d9953a5f9/snapshot3.png">
</details>



<details>
 <summary> pt tool </summary>

Below is the screenshot showing the successful launch pt:
Synopsys PrimeTime is a leading EDA tool for signoff static timing analysis. It ensures accurate timing predictions in IC designs, verifying performance and meeting critical design requirements. PrimeTime aids in identifying and addressing timing violations, contributing to reliable and high-performance chip development.

<img width="1085" alt="snapshot4" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c0557b0a5bd5348ceecca3631719d89546d6a5d7/snapshot4.png">
</details>


<details>
 <summary> yosys </summary>

Below is the screenshot showing the successful launch yosys:
Yosys is an open-source framework for RTL synthesis and formal verification of digital circuits. It transforms hardware descriptions written in languages like Verilog and VHDL into optimized netlists or other formats. Yosys is popular for its versatility, enabling various design transformations and analyses in the field of digital design automation.
<img width="1085" alt="snapshot4" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/94c49bedda1760744522b5223449e03c4983c3d8/yosys.png">
</details>



<details>
 <summary> gtkwave </summary>

Below is the screenshot showing the successful launch gtk wave:
GTKWave is an open-source waveform viewer software used in digital design and verification. It allows engineers to visualize and analyze simulation results from hardware description languages like Verilog or VHDL. GTKWave displays signal waveforms, enabling users to debug and understand the behaviour of their digital circuits during simulation.

<img width="1085" alt="snapshot4" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/cbc87d384d246852a8d32167efc9adb7f51a47ed/gtkwave.png">
</details>

<details>
 <summary> Summary </summary>
	
following tools are explored: dc shell, icc2 shell, pt shell, lc shell, yosys, gtkwave.

</details>	

## Day-1-Introduction to Verilog RTL Design and Synthesis
 <details>
 <summary> introduction to Verilog design and testbench </summary>
  Design:-
  The actual Verilog code or set of Verilog codes has the intended functionality to meet the required specifications.
	 
  Testbench:-
  Testbench is the setup to apply the stimulus to the design to check .its functionality.
   <img width="1085" alt="Design and verification" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9c4ca4c892766e1c6449047a02ca291b3302c1ce/Design%20and%20testbench.jpg">  
  </details>


  <details>
 <summary> Cloning directories </summary>
  The command to clone the files from GitHub is:- git clone link_url.git.  
  The below figure shows the cloning of vsdflow and sky libraries.	  
   <img width="1085" alt="clone sky" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b396e7227784d6031ced0b062d65fd4119d06d08/clone_sky.jpg">  
    <img width="1085" alt="vsdflow" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/41ef5e4854c4918f41047d7fe10b011a8461af69/clone_vsdflow.jpg">    
  </details>


 <details>
 <summary> iverilog and gtkwave </summary>

  verilog_files consists of all the Verilog design files and testbench for that design.
   <img width="1085" alt="verilog files" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/178397567e2b999cd43c646e5bf08ba328796fee/verilof_files.jpg">  
   we can observe output result in a better way from the gtkwave waveforms. As an example here we can see output waveforms for good_mux design. 
    <img width="1085" alt="gtkwave" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b03d17fe777d6a32d60cc6d5e6b36d5734b6f994/gtkwave_good_mux.jpg">  	  
  </details>


 <details>
 <summary> Example of one Design and its testbench </summary>
 The below figures are examples of the design and testbench code for the good_mux. And the command used to view is: vim file_nanw.v
 <img width="1085" alt="Design" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77a26d76b5c7408921b46946aeb61f47ffa7aac6/good_mux.jpg">  
 <img width="1085" alt="Testbench" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c11432dd91f9d8b3c0b69ad37090ee3b5ebf77c7/tb_new.jpg">  
	 	 
  </details>


 <details>
 <summary> Introduction to Yosys </summary>
   Yosys is an open-source framework for RTL synthesis and formal verification of digital circuits. It transforms hardware descriptions written in languages like Verilog and VHDL into optimized netlists or other formats. Yosys is popular for its versatility, enabling various design transformations and analyses in the field of digital design automation.Basically, it converts RTL code into gate level netlist. As an input it takes DESIGN and .lib file and gives netlist which is nothing but the file which consists the connections of gate.
   
	 	 
  </details>


 <details>
 <summary> Yosys </summary>
   1. To invoke the yosys, command is: yosys <br>
   2. To read the library file inside yosys, command is: read_library -lib ../library_path <br>
   3. To read the verilog file, command is : read_verilog file_name.v <br>
   4. To specify the module for synthesis :  synth -top file_name<br>
   5. To generate the netlist : abc -liberty ../library_path<br> 
   img width="700" alt="signals" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/849e349412ce2a859b4aa428cd9349bb118a253f/Signals.jpg "><br>

  
   6. For graphical view : show<br>
      img width="700" alt="graphical representation" src="img" alt="snapsrc="https://github.com/gohilnihar07/Samsungpdtraining/blob/8553d133af27693fa09b05956ff915839704399f/snapshot2.png">

   7. For writing netlist : write_verilog netlist_filename.v<br>
   8. To see the generated netlist : !vim filename_netlist.v
   img width="1085" alt="netlist" src="img" alt="snapsrc="https://github.com/gohilnihar07/Samsungpdtraining/blob/8553d133af27693fa09b05956ff915839704399f/snapshot2.png">




	 	 
  </details>
