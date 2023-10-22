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
   6. For graphical view : show<br>
   <img width="1085" alt="graph" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e0737761ed09a7cb5ce2025ffeb29826f6205bab/Graphical%20representation.jpg "><br>

   7. For writing netlist : write_verilog netlist_filename.v<br>
   8. To see the generated netlist : !vim filename_netlist.v
  <img width="700" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9ff00607aca0b62ecc9c1948ea4cd27dbb9690a3/Netlist.jpg">
	 	 
  </details>




## Day-2-Timing libs, hierarchical Vs flat synthesis and efficient flop coding styles

<details>
	<summary> Timing libs </summary>
	For opening a library,command:-  gvim /library_path <br>
	There are three corners basically which are process, voltage and temperature which can be identified from the library name itself. So basically we want our silicon to work across all the corners because those three corners basically decide, how my silicon is going to work. so we need to factor in these variations while we are designing our circuit, so our library is characterized to model these variations. there are different flavours of different cells and different flavours of the same cell are available.
	<img width="600" alt="lib" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ba497da455f34a15778288bda42c074152b1dcfb/lib%20file.jpg"><br>
	For going to cell, command: / cell <br>
	<img width="600" alt="lib" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ff2c84c8133be5cd98e1e9145ee1c6421c051583/info%20of%20leakage%20power%20for%20all%20input%20combi.%20for%20a%20cell.jpg"><br>
       The keyword cell is marked at the beginning of the cell definition. For each cell it will tell you what is the leakage power for all possible input combinations<br>
	<img width="600" alt="lib" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b966e8ec355ef31b6db07d4a74a964ce34ea0f5e/lib%20it%20gives%20info%20about%20area%20and%20power%20etc...jpg"><br>
      It gives you the number and power information ofthe  cell.<br>
	<img width="600" alt="lib" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/f5374386094a0c7aea0445849005114294307a2a/lib%20pin%20info.jpg"><br>
	For every pin it describes, what's the input capacitance of the pin, what's the power related to the pin, what's the delay associated with the pin, what's the power associated with the pin and timing information about the pin.<br> 
	For closing the cell, command:  :g// 
	In case you want to understand the functionality or behavior of any cell, command: :sp ../my_lib/verilog_model/sky130_fd_sc_hd_cellname. behavioral.v <br>
	For picking any particular cell, command: /cell .*cell_name <br>
	For separating the same screen, command: :vsp <br>
	From the same cell with two or three different flavours of information, we can observe the cell area information and from that, we can say, that the cell with the higher area(wider area cell) is a faster cell and the cell with the lesser area is slower cell and also wider cell consumes more power and having less delay, vice versa.<br>
</details>


<details>
	<summary> Hierarchical Vs Flat synthesis </summary>
To understand the difference between hierarchical synthesis vs flat synthesis, we will take the example of one design named multiple_modules.in the below figure from the design, we can see that there is one OR gate and one AND gate present.  <br>
<img width="600" alt="lib" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/f842bd4e9e471390f5c0069595dbec1ddfae5c24/multiple_modules.jpg"><br>
Now, let's see when we synthesize it how does it make difference, and by default, synthesis will be hierarchical synthesis.<br>
As we can see graphical representation of hierarchical synthesis in below figure from thatb we can say it's not showing the AND and OR gate but it's showing in the form of sub module1 and sub module2, so this is what basically hierarchical synthesis is, which infered the modules.<br>

<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c8721bed7184c2ad59e8ed67be9277f76e0428ee/hierarcies%20are%20preserved.jpg"><br>
	<img width="600" alt="lib" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d0422cfa563b5097a6555aa56bd367db5d62a346/hierarcy_synthesis_infered.jpg"><br>
 Here also in the below figure of generated netlist, we can see it preserves hierarchy.<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/36f6a31ab857072270000ae0c196a561623ca6d1/even%20in%20the%20generated%20netlist%20also%20we%20can%20see%20that%20the%20hierarcy%20preserves.jpg"><br>
 **flat synthesis**
 Now for flat synthesis after linking the design to the  library write, command : flatten <br>
 Can see the graphical representation for flat synthesis in below figure, <br>
 
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/10e33b875b7f2307c7e4a487ead123aeca51b57e/so%20in%20flatten%20synthesis%20we%20can%20directly%20see%20the%20structure%20completely.jpg"><br>
So, from the above figure, we can say that in flatten synthesis we can see the whole structure(every gate).<br>
 
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/84e741ae2c240337fe1a1057912da4482d490863/flat_synthesis_netlist.jpg"><br>
The single netlist will be generated of multiple_module, underneath we can see everything.<br>
**sub-module level synthesis**
We can do synthesis at sub-module level also, command: synth -top sub_module_name <br>
Basically in some cases, it's preferable to do synthesis at sub-module level,<br>
1. It's preferred when we have multiple instances of the same module. so, instead of synthesizing one sub-module many times, it's better to synthesize it once and then replicate it as many times as needed and then stitch it together in top module.<br>
2. Divide and conquer. like when your design is massive that case let's say your tool is not doing a good job, so instead of giving a massive design to the tool, give portion by portion to the tool so that it writes out a very optimize netlist and then you stitch it together at the top module.<br>
Can see the below netlist which is generated for sub-module,<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/196a5a276c197992349ef29e0ba40ade228e7de5/netlist%20for%20sub_module%20level%20synthesis.jpg"><br>

 </details>





 <details>
 <summary> Flop coding style, simulation and synthesis</summary>
	 We required flop beacause due to the diffferent propagation delay of gates at the output glitches may come, so to overcome glitch problem, in between combinational circuit we keep flipflop to avoid glitches.And to control the flop there is a set and reset which we can design synchronous or asynchronous based on our requirements.<br>
	
 **Below is the code for asynchronous reset D flip flop**,

module dff_asyncres ( input clk ,  input async_reset , input d , output reg q ); <br>
always @ (posedge clk , posedge async_reset) <br>
begin<br>
	if(async_reset)<br>
		q <= 1'b0;<br>
	else	<br>
		q <= d;<br>
end<br>
endmodule<br>

  After simulating we can see the GTK waveforms shown in below figure,<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d55b3cbadc3bd2f21be726ee820d50c6f7378d12/dff_asyncres_gtkwave.jpg"><br>
    Graphical representation after the synthesis is shown in below figure,<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/aafd51c97f0049b9515a5ff34e79354c27880450/netlist%20of%20asyncronous%20reset%20flop.jpg"><br>
        After synthesizing it we can see the netlist shown in below figure<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2bc4cd5129339a86ffddfd7386363ad4d1186ab9/netlist%20in%20coding%20way%20of%20asyncronous%20reset%20flop.jpg"><br>  


 **Below is the code for asynchronous set D flip flop**,<br>

 
module dff_async_set ( input clk ,  input async_set , input d , output reg q );<br>
always @ (posedge clk , posedge async_set)<br>
begin<br>
	if(async_set)<br>
		q <= 1'b1;<br>
	else	<br>
		q <= d;<br>
end<br>
endmodule<br>

  After simulating we can see the GTK waveforms shown in below figure,<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/fe76c34034e6fecb2d18f58b6b0f1a5906684718/dff_async_set_gtkwave.jpg"><br>
    Graphical representation after the synthesis is shown in below figure,<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ea21a9363cf71e8e6f749e425d1678af03efaf45/dff_async_set_graphical_repre.jpg"><br>
        After synthesizing it we can see the netlist shown in below figure<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/af09b0cb2e3a196d73efef7627697f961b61b0dc/dff_async_set_netlist.jpg"><br>  


 **Below code is for synchronous reset D flip flop**,<br>

module dff_syncres ( input clk , input async_reset , input sync_reset , input d , output reg q );<br>
always @ (posedge clk )<br>
begin<br>
	if (sync_reset)<br>
		q <= 1'b0;<br>
	else	<br>
		q <= d;<br>
end<br>
endmodule<br>


  After simulating we can see the GTK waveforms shown in below figure,<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/06093e21aeb5db2cc41d92ef2aa89d1f910d4ee6/dff_syncres_gtkwave.v.jpg"><br>
    Graphical representation after the synthesis is shown in below figure,<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8c05620a170fd4a001105f11391b99a7399df894/dff_syncres_graphical_repre.jpg"><br>
        After synthesizing it we can see the netlist shown in below figure<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/266e4e7550a818f7b9b065d4ef780871b6bb967e/dff_syncres_netlist.jpg"><br>  

</details>


 
<details>
<summary> Some special cases in optimization </summary>
It's not necessary that every time when you are doing some operations hardware is required but in some cases, just by rewiring signals, we are able to get the logic functionality implemented.<br>
Let's see some examples of special cases,<br>
	
1. y=2*a, where a[2:0] and y[3:0] (here the functionality that we actually need to implement is the multiplication)<br>
when we try to synthesize it, it shows<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/a56a95bb0978b390b045f5a1c7a937bed9d8db3d/mul_2%20.jpg"><br>
means, not needing any cell.<br>
Now, when we try to map it with a technology file, it says no need because there is actually nothing to map<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4f204fbdc94c9d3f9e866904e4fb99ac1844979b/mul_2_nothing%20to%20map.jpg"><br>
We can understand the same thing by graphical representation also after the synthesis,<br>
   <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0500353abc5f74c891f9eaa34bf391d0e5787d10/mul_2_post_synthesis%20view.jpg"><br>
	Netlist <br>
	<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/faccf7bfb4209ab0a9b6493a6dee561eac98c020/mult_2%20netlist.jpg">
	Similarly, if there is anything power of 2 then just upending with zero can solve. So we don't require any hardware for these cases rewiring signals gives the solution.<br>

       2. Let's suppose a[2:0] and y[5:0] are fixed, now do y=9*a
       When we try to synthesize it, it shows<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/f7c9ab6227dcbc91d862d45f4b0c13f0fb9d39f2/mult_8.jpg"><br>
 means, not needing any cell.<br>
	Now, when we try to map it with a technology file, it says no need because there is actually nothing to map<br>
	 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3c7ae27a9d6df143b5a8ae2f0ef14183bf24c8a9/mult_8%20nothing%20to%20map.jpg"><br>
	We can understand the same thing by graphical representation also after the synthesis,<br>
   <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/35ed660fb65432f6e4c6e4e0b91552533acd2d6a/mult%208%20after%20synthesis.jpg"><br>
	Netlist <br>
	<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e3de654333b11c12b2f5fc6b8ac91c0c78f6d098/mult_8%20netlsit.jpg"><br>
        So, there are some special cases like this, in which we can implement the logic functionality just by rewiring the signals.
</details>



## Day-3- Optimization of combinational and sequential circuits

<details>
	<summary> Combinational logic optimization techniques and examples </summary>
	Combinational logic optimization is a process in digital circuit design that aims to improve the performance, efficiency, and/or area utilization of a digital circuit composed of combinational logic gates. Combinational logic refers to a type of digital logic where the output is solely determined by the current input values, without any memory or feedback elements.<br>

The goal of combinational logic optimization is to reduce various metrics such as propagation delay, power consumption, and area occupation while maintaining the functionality of the circuit.Some common techniques used in combinational logic optimization are:<br>
<br>
1. Constant propagation technique:<br>
     It's a direct optimization technique.It identifies and removes redundant logic expressions that appear in multiple places within the circuit.<br>
     Example,<br>
     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c1b18ae69547d8ae05426147dce7071d42f424a9/DAY%203/Comb_const_propa_example.jpg"><br>
     If we realise it in the form of CMOS then we can clearly observe that this optimized version takes less area.<br>
     <br>
2. Boolean logic optimization: <br>
     This involves using Boolean algebra rules and laws to simplify logical expressions. Karnaugh maps and Quine-McCluskey methods can be used to find the minimal representation of logic functions.<br>
     Example, assign y=a?(b?c:(c?a:0)):(!c) <br>
     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/17922903b53a0439a60ec1edd1eafed0444c7b28/DAY%203/Comb_boolean_logic_opt_example.jpg"><br>
     Here also we can say that the optimized version will take less area.<br>
     <br>
It's important to note that optimization can involve trade-offs between different design parameters like area, power, timing, etc. So designers need to consider their specific requirements and constraints to strike the right balance.<br>
Modern digital design tools and software use a combination of these techniques to automatically optimize digital circuits, taking into account the target technology (e.g., CMOS, FPGA), design constraints, and objectives.
</details>


<details>
	<summary> Lab for combinational logic optimization </summary>
	Examples,<br>
	1. opt_chcek<br>
	  --> Verilog code for design opt_check,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d61f67c491ea76b8c03e5058d8a4a1c14b4d764e/DAY%203/opt_check_code.jpg"><br><br>
          --> Circuit diagram and expecting result after optimization,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4920039f9b096e15ba7a6fa7d817e48320a68a80/DAY%203/Comb_lab_opt_check1_example.jpg"><br>
	      so, we are expecting a AND gate to be generated after optimization. <br><br>															
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d8da7826348d54b0dcb876643f8027e09de61cfa/DAY%203/opt_check_statistics.jpg"><br>
	      Can see in the above statistics that only one AND will generate.<br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4c5c815820e85961aa1ef2ef5f1ac6706e6013e7/DAY%203/opt_check_graphical_rep.jpg"><br>
	      As can be seen in the above graphical representation it's generating only one AND gate as we expected.<br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4c5c815820e85961aa1ef2ef5f1ac6706e6013e7/DAY%203/opt_check_netlist.jpg"><br><br><br>
         2. opt_check<br>
	   --> Verilog code for design opt_check_2,<br>
         
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4c5c815820e85961aa1ef2ef5f1ac6706e6013e7/DAY%203/opt_check2_code.jpg"><br>
          --> Circuit diagram and expecting result after optimization,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4c5c815820e85961aa1ef2ef5f1ac6706e6013e7/DAY%203/Comb_lab_opt_check2_example.jpg"><br>
             so, we are expecting an OR gate to be generated after optimization. <br><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4c5c815820e85961aa1ef2ef5f1ac6706e6013e7/DAY%203/opt_check2_statistics.jpg"><br>
             Can see in the above statistics that only one OR will generate.<br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4c5c815820e85961aa1ef2ef5f1ac6706e6013e7/DAY%203/opt_check2_graphical_rep.jpg"><br>
             As can be seen in the above graphical representation it's generating only one OR gate as we expected.<br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4c5c815820e85961aa1ef2ef5f1ac6706e6013e7/DAY%203/opt_check2_netlist.jpg"><br><br><br>
       3. opt_check3<br>
          --> Verilog code for design opt_check3,<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/22ff3bb9af11858fa46b206b4dc0f9723d2b4bf0/DAY%203/opt_check3_code.jpg"><br><br>
          --> Circuit diagram and expecting result after optimization,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/22ff3bb9af11858fa46b206b4dc0f9723d2b4bf0/DAY%203/Comb_lab_opt_check3_example.jpg"><br>
              so, we are expecting three-input AND gate to be generated after optimization. <br><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/22ff3bb9af11858fa46b206b4dc0f9723d2b4bf0/DAY%203/opt_check3_statistics.jpg"><br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/22ff3bb9af11858fa46b206b4dc0f9723d2b4bf0/DAY%203/opt_check3_graphical_rep.jpg"><br>
              As can be seen in the above graphical representation it's generating only one OR gate as we expected.<br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/22ff3bb9af11858fa46b206b4dc0f9723d2b4bf0/DAY%203/opt_check3_netlist.jpg"><br><br><br>
   4. opt_check4<br>
       --> Verilog code for design opt_check,<br>
      
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/opt_check4_code.jpg"><br><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/opt_check4_statistics.jpg"><br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="900" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/opt_check4_graphical_rep.jpg"><br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/opt_check4_netlist.jpg"><br><br><br>
      
  5. multiple_module_opt<br>
       --> Verilog code for design multiple_module_opt,<br>    
       
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/multiple_module_opt_code.jpg"><br><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/multiple_module_opt_statistics.jpg"><br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="1000" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/multiple_module_opt_graphical_rep.jpg"><br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/multiple_module_opt_netlist.jpg"><br><br><br>

 6. multiple_module_opt2<br>
         --> Verilog code for design multiple_module_opt2,<br>
	 
  <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/multiple_module_opt2_code.jpg"><br><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/multiple_module_opt2_statistics.jpg"><br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="1600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/multiple_module_opt2_graphical_rep.jpg"><br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6e167bbef4831a119aed62c92d3ebaf8018ae6ab/DAY%203/multiple_module_opt2_netlist.jpg"><br><br><br>
</details>




<details>
	<summary> Sequential logic optimization techniques and examples </summary>
	Sequential logic optimization is the process of improving the performance, efficiency, and other characteristics of digital circuits that contain memory elements such as flip-flops, latches, and registers. Unlike combinational logic, where the output depends only on the current inputs, sequential logic circuits have an element of memory and store information about past inputs.<br>
        The goal of sequential logic optimization is to enhance various aspects of the design, such as speed, power efficiency, area utilization, and reliability, while ensuring that the functionality of the circuit is preserved. Some common techniques used in sequential logic optimization are:<br><br>
	1. Sequential constant propagation:<br>
	Sequential Constant Propagation (SCP) is an optimization technique used in compiler design to improve the efficiency of code execution by replacing variables with their constant values wherever possible. This technique falls under the category of data flow analysis and optimization, aiming to identify opportunities for substituting variables with their known constant values throughout the program's execution flow.<br>
	Example,<br>
	 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/473813b8a20f6fe2fe3c5cbb652cf0d7af3b6afb/DAY%203/Sequ_const_propa_example.jpg"><br><br>
	2. state optimization:<br>
         One of the primary goals is to reduce the number of states in a finite state machine (FSM) while preserving the desired functionality. This helps in reducing the complexity of the circuit and often leads to improved performance.<br><br>
	3. Cloning:<br>
	  Example,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/dd4e26ba8129a04a02b2a3f90e421c10fc6a5b5e/DAY%203/Seque_cloning_opt_example.jpg"><br><br>
        4. Retiming:<br>
	  Moving flip-flops within a circuit while maintaining the same functionality can optimize timing and pipeline stages. This can help balance critical paths and improve the overall speed of the circuit.<br>
       Example,<br>
       <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8e184d661e07b7a2732d262d6f3391ffa26f6497/DAY%203/Seque_retiming_opt_technique_example.jpg"><br><br>
       5. Clock gating:<br>
       Introducing clock gating to disable portions of the circuit during clock cycles when they are not needed. This reduces power consumption by preventing unnecessary state changes and logic operations.<br><br>
	6. State Assignment:<br>
	Assigning binary codes (state encodings) to different states of an FSM in a way that minimizes transitions between states can improve circuit performance and reduce area.<br><br>


It's important to emphasize that sequential logic optimization involves intricate interactions between the memory elements and the combinational logic. Designers need to carefully balance optimization goals while ensuring that the circuit's behavior and timing requirements are met. Advanced design automation tools play a crucial role in navigating the complexities of sequential logic optimization, as manual optimization can be extremely challenging and time-consuming for complex designs.

</details>


<details>
	<Summary> Lab for sequential logic optimization </Summary>
	Examples,<br>
	 1. dff_const1<br>
          --> Verilog code for design dff_const1,<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const1_code.png"><br><br>
          --> Circuit diagram and expecting result after simulation,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/Seque_lab_dff_check1_example.jpg"><br>
              so, we are expecting these waveforms to be generated after simulation. <br><br>
	--> Gtkwave waveforms,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const1_gtkwave.png"><br><br>
	     As expected waveforms have come.<br><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const1_statistics.png"><br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const1_graphical_rep.png"><br>
              As can be seen in the above graphical representation as we expected.<br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const1_netlist.png"><br><br><br>



  2. dff_const2<br>
          --> Verilog code for design dff_const2,<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const2_code.png"><br><br>
          --> Circuit diagram and expecting result after simulation,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/Seque_lab_dff_check2_example.jpg"><br>
              so, we are expecting these waveforms to be generated after simulation. <br><br>
	--> Gtkwave waveforms,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const2_gtkwave.png"><br><br>
	     As expected waveforms have come.<br><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const2_statistics.png"><br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const2_graphical_rep.png"><br>
              As can be seen in the above graphical representation as we expected.<br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const2_netlist.png"><br><br><br>


 3. dff_const3<br>
          --> Verilog code for design dff_const4,<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const3_code.png"><br><br>
          --> Circuit diagram and expecting result after simulation,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/Seque_lab_dff_check3_example.jpg"><br>
              so, we are expecting these waveforms to be generated after simulation. <br><br>
	--> Gtkwave waveforms,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const3_gtkwave.png"><br><br>
	     As expected waveforms have come.<br><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const3_statistics.png"><br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const3_graphical_rep.png"><br>
              As can be seen in the above graphical representation as what we expected.<br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const3_netlist.png"><br><br><br>


4. dff_const4<br>
          --> Verilog code for design dff_const4,<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const4_code.png"><br><br>
	--> Gtkwave waveforms,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const4_gtkwave.png"><br><br>
	     As expected waveforms have come.<br><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const4_statistics.png"><br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const4_graphical_rep.png"><br>
              As can be seen in the above graphical representation as what we expected.<br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const4_netlist.png"><br><br><br>



 5. dff_const5<br>
          --> Verilog code for design dff_const5,<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const5_code.png"><br><br>
	--> Gtkwave waveforms,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const5_gtkwave.png"><br><br>
	     As expected waveforms have come.<br><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const5_statistics.png"><br><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const5_graphical_rep.png"><br>
              As can be seen in the above graphical representation as what we expected.<br><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0dbed32a773272a3cccf1707246a939de8d2f651/DAY%203/dff_const5_netlist.png"><br><br><br>
</details>





<details>
	<summary> Optimizing unused outputs in a sequential process  </summary>
        Optimizing unused outputs in a sequential process typically involves improving the efficiency or effectiveness of a system by optimizing the outputs that are not directly used or observed in the process.<br>
	Here listing some things about how we should approach that,<br><br>
        1. Identify Unused Outputs: In any sequential process, there might be outputs that are generated but not actively used or monitored. These could be intermediate results, byproducts, or secondary outcomes. <br><br>
2. Assess Importance: Before optimizing unused outputs, it's crucial to assess whether these outputs have any potential value or significance. Sometimes, seemingly unused outputs might hold hidden insights or could be leveraged in unexpected ways.<br><br>
3. Process Analysis: Understand the sequential process thoroughly. This includes understanding the inputs, steps, transformations, and outputs at each stage. By mapping out the process, you can identify where unused outputs are generated.<br><br>
  The key is to approach the optimization systematically, with a clear understanding of the process and the potential impacts of changes.<br><br>

   Examples,:<br>
       1. Counter_opt<br>
        --> Verilog code for design counter_opt,<br>
         <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/233000f662f57d0d56036369b37c246838ccf42d/DAY%203/counter_opt.png"><br><br>
        --> Circuit diagram,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/233000f662f57d0d56036369b37c246838ccf42d/DAY%203/Unused_output.jpg"><br>
               Here, I'm not bothered about count[2] and count[1] because the final output only depends on count[0]. So we are expecting that the optimized result will have only one flop. <br><br>
	--> statistics,<br>
	     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/233000f662f57d0d56036369b37c246838ccf42d/DAY%203/counter_opt_statistics.png"><br>
             As expected it's generating only one flop.<br><br>
	--> Graphical representation after mapping,<br>
	     <img width="1300" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/233000f662f57d0d56036369b37c246838ccf42d/DAY%203/counterr_opt_graphical_rep.png"><br>
              As can be seen in the above graphical representation it's generating only one flop as we expected.<br><br>
	--> Generated netlist,<br>
<img width="600" alt="netlist"  src="https://github.com/gohilnihar07/Samsungpdtraining/blob/233000f662f57d0d56036369b37c246838ccf42d/DAY%203/counter_opt_netlist.png"> <br><br><br>
  2. Counter_opt2<br>
     --> Verilog code for design counter_opt2,<br>

     
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/233000f662f57d0d56036369b37c246838ccf42d/DAY%203/counter_opt2.png"><br><br>
        Here, since the output is dependent on all the three bits. So we are expecting that the output will generate three flops. <br><br>
	--> statistics,<br>
            <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/233000f662f57d0d56036369b37c246838ccf42d/DAY%203/counter_opt2_statistics.png.png"><br>
             As expected it's generating three flops.<br><br>
	--> Graphical representation after mapping,<br>
	     <img width="1600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/233000f662f57d0d56036369b37c246838ccf42d/DAY%203/counter2_opt_graphical_rep.png.png"><br>
              As can be seen in the above graphical representation it's generating three flops as we expected.<br><br>
	--> Generated netlist,<br>
  <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/233000f662f57d0d56036369b37c246838ccf42d/DAY%203/counter_opt2_netlist.png"><br><br><br>
      

 </details>



## DAY-4- GLS, blocking  Vs non-blocking and Synthesis-Simulation mismatch

<details>
	<summary> Gate-level simulation</summary>
 Gate-level simulation involves creating a simulation model of the circuit using the gate-level description. This model represents how the gates and flip-flops interact and respond to input signals. Simulation tools then simulate the propagation of signals through the gates, taking into account gate delays, to predict the behavior of the circuit in response to different inputs. This is important for verifying the correctness of the design, identifying potential timing issues, and ensuring that the circuit functions as intended.<br>
 In modern digital design, gate-level simulation is often complemented with higher-level simulations and formal verification techniques to provide a comprehensive validation of the design's correctness and functionality.<br><br>

--> Gate-level simulation using iverilog :-<br>
      <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/5b08dff1d7fcb3f0176aa1dffbd990a516afd290/DAY%204/IMG_20230829_113705.jpg"> <br>
      Here, the design file is nothing but the netlist generated from our sythesis. and since the primary input and primary output remains same for RTL code and netlist file So, we can use the same testbench as what we used for RTL verification.and Gate-level models consists information about all the cell name like what it means and all. if the gate-level models are delay annotated, then we can use GLS for timing validation also along with functional validation.      
	
</details>




<details>
	<summary> Synthesis simulation mismatch</summary>
	A synthesis simulation mismatch refers to discrepancies or differences between the behavior of a digital design as simulated before and after synthesis. This mismatch can occur due to various reasons, and it's important to identify and resolve these issues to ensure the correctness of the synthesized design. Here are some common reasons for synthesis simulation mismatches:<br><br>
 1. Missing sensitivity list:-<br>
 Example, Let's say my aim is to create mux,<br>
```ruby
module bad_mux (input i0 , input i1 , input sel , output reg y);
always @ (sel)
begin
	if(sel)
		y <= i1;
	else 
		y <= i0;
end
endmodule
```
<br>		
Now, if i will write my code like this then, it won't generate mux but it will generate double edge flop.<br><br>


instead if i will write like this<br>
```ruby
module good_mux (input i0 , input i1 , input sel , output reg y);
always @ (*)
begin
	if(sel)
		y <= i1;
	else 
		y <= i0;
end
endmodule
```
If we write always like this, always will evaluated when any signal changes then, it will generate mux.<br>

So,always write sensitivity list carefully.
<br><br>

2.Blocking Vs non-blocking statements <br>
In Verilog, blocking and non-blocking statements are two different ways of assigning values to variables within procedural blocks like always and initial blocks. These statements control the sequencing and timing of assignments, and understanding their differences is crucial for writing correct and predictable RTL code.<br><br>
(I)Blocking Statements:<br>
Blocking assignments (=) are executed sequentially in the order they appear in the code. When a blocking assignment is encountered, the execution of the current procedural block is paused until the assignment is completed.<br><br>
(II)Non-blocking statements:<br>
Non-blocking assignments (<=) are used to model concurrent behavior within procedural blocks. Non-blocking assignments are scheduled to occur at the end of the current time step, allowing all non-blocking assignments within a procedural block to update simultaneously without affecting the rest of the logic in the block.<br><br>

--> Cavets with blocking statements,<br>
Example 1, My aim is to generate like below <br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b5edaaf3ece9d1d762432f13bdbdd93d34d946aa/DAY%204/IMG_20230829_113637.jpg"> <br><br>
 If i will write my code like this,<br>
 ```ruby
 module code(input clk, rst, d, output reg q);
 reg q0;
 always @ (posedge clk, posedge rst)
 begin
	if(rst)
        begin
		q0 = 1'b0;
                q = 1'b0;
        end
 else 
        begin
		q0 = d;
                q = q0;
        end
 end	
endmodule<br>
```
It will not generate as we expected and also it will generate only one flop.<br><br>

 But,if i will write my code like this,<br>
 ```ruby
 module code(input clk, rst, d, output reg q);
 reg q0;
 always @ (posedge clk, posedge rst)
 begin
	if(rst)
        begin
		q0 = 1'b0;
                q = 1'b0;
        end
 else 
        begin
		q = q0;
                q0 = d;
        end
 end	
endmodule<br>
```
It will generate as what we expected.<br><br>

Example 2, my aim is to make this,<br>
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4addd2303879fa24e83f32ca80c919bc74f72bcd/DAY%204/IMG_20230829_150045.jpg"> <br>
```ruby
module blocking_caveat (input a , input b , input  c, output reg d); 
reg q0;
always @ (*)
begin
	d = q0 & c;
	q0 = a | b;
end
endmodule
```
The problem with the above code is that will take an old value of q0 so it will give false results.<br><br>
```ruby
module blocking_caveat (input a, input b, input  c, output reg d); 
reg q0;
always @ (*)
begin
        q0 = a | b;
	d = q0 & c;
	
end
endmodule
```
here q0 will take the current value, so Ouput will get the correct results.<br>
Use non-blocking statements for writing sequential circuits to avoid such mistakes and if you are using blocking statements then be very careful while writing it.<br><br>


3. Non-standard verilog coding can lead to a synthesis simulation mismatch. So use proper coding guidelines to write the clear RTL code and avoid non-synthesizable constructs.<br><br>
4. Optimization: Synthesis tools perform various optimizations to enhance area, power, and timing characteristics. These optimizations can alter the logic structure of the design, potentially leading to differences in behaviour. Redundant logic might be removed, and signal paths might be altered to achieve better performance.<br><br>

5. Timing and delays: Synthesis tools account for gate delays, interconnect delays, and other physical characteristics of the target technology during the synthesis process. This can lead to timing differences between the original design's simulation and the post-synthesis simulation. Signals that were once perfectly synchronous in simulation might experience timing issues after synthesis.

</details>


<details>
	<summary>Labs on GLS and synthesis simulation mismatch </summary>
       Command for Gate-level simulation:<br>
       iverilog path_gate_level_model.v path_verilogg_file_lib.v netlist_name.v design_name.v<br><br>
       Example 1,<br>
       --> Verilog code for ternary_operator_mux design,<br>
       <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a5d7a6d10b5a5afa81fb678b1b3fd628680dd63/DAY%204/Ternary_operator_mux_code.v.jpg"> <br><br>
       --> RTL level simulation result,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a5d7a6d10b5a5afa81fb678b1b3fd628680dd63/DAY%204/Ternary_operator_mux_gtkwave.v.jpg"> <br>
	As expected when the value of sel is 1 output follows i1 and when the value of sel is 0 output follows i0.<br><br>
       --> Graphical representation,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4b31172b2d88320fa615931dba80531ef2953f87/DAY%204/Ternary_operator_mux_graphical_rep_2_v.jpg"> <br>
	As expected it's generating one 2x1 mux,<br><br>
	--> generated netlist,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a5d7a6d10b5a5afa81fb678b1b3fd628680dd63/DAY%204/Ternary_operator_mux_netlist.v.jpg"> <br>
	Now, this generated netlist we will use for performing gate-level simulation or functional validation.<br><br>
       --> Gate-level simulation result,<br>
         To perform the gate level simulation we can use the same testbench which we had used for the RTL simulation because the primary input and primary outputs won't change.<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a5d7a6d10b5a5afa81fb678b1b3fd628680dd63/DAY%204/Ternary_operator_mux_gtkwave_GLS_.v..jpg"> <br><br>
	So as we can see our gate-level simulation result is the same as the RTL simulation, so everything is fine.<br><br><br>
 Example 2,<br>


       
 --> Verilog code for bad_mux design,<br>
       <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ec8497d1fb7b25ee10d748dbcad0d95c048c8e41/DAY%204/good_mux_code.png"> <br>
       We are writing code for mux but can see in the Verilog code sensitivity list only consists of select.<br><br>
       --> RTL level simulation result,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ec8497d1fb7b25ee10d748dbcad0d95c048c8e41/DAY%204/bad_mux_gtkwave.jpg"> <br>
	Since the sensitivity list does not consist of all the important parameters it's not working as mux but it's working like a double-edge flipflop in which it will evaluate only when there is a change in sel input.<br><br>
       --> Graphical representation,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4b31172b2d88320fa615931dba80531ef2953f87/DAY%204/bad_mux_graphical_rep_2_v.jpg"> <br><br>
       --> generated netlist,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ec8497d1fb7b25ee10d748dbcad0d95c048c8e41/DAY%204/bad_mux_netlist.jpg"> <br>
	This generated netlist we will use for performing gate-level simulation.<br><br>
       --> Gate-level simulation result,<br>
         To perform the gate level simulation we can use the same testbench that we had used for RTL simulation because the primary input and primary outputs won't change.<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ec8497d1fb7b25ee10d748dbcad0d95c048c8e41/DAY%204/bad_mux_gtkwave_GLS.jpg"> <br>
	We can clearly see that it's working like a mux, like when there is a change in a or b and depending on the select input value it's evaluating the output result. So here since the RTL simulation and gate-level simulation results are not the same so we can say it's a case of synthesis simulation mismatch.<br><br><br>

Example 3,<br>
--> Verilog code for good_mux design,<br>

 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ff63e66e2fde64acbc82d6191b9ed8611d6c68af/DAY%204/good_mux_code.png"> <br>
  We are writing code for Mux and we can also see that we have  written the Verilog code sensitivity list very carefully.<br><br>
       --> RTL level simulation result,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ff63e66e2fde64acbc82d6191b9ed8611d6c68af/DAY%204/good_mux_gtkwave.png"> <br>
	Since the sensitivity list includes all the important parameters which are needed to be considered, it's working as a mux.<br><br>
       --> Graphical representation,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ff63e66e2fde64acbc82d6191b9ed8611d6c68af/DAY%204/good_mux_graphical_rep.png"> <br><br>
       --> generated netlist,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ff63e66e2fde64acbc82d6191b9ed8611d6c68af/DAY%204/good_mux_netlist.png"> <br>
	This generated netlist we will use for performing gate-level simulation.<br><br>
       --> Gate-level simulation result,<br>
         To perform the gate level simulation we can use the same testbench which we had used while RTL simulation because the primary input and primary outputs won't change.
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/ff63e66e2fde64acbc82d6191b9ed8611d6c68af/DAY%204/good_mux_GLS_gtkwave.png"> <br>
	so as we can see our gate-level simulation result is same as the RTL simulation, so everything is fine.<br><br><br>
Example 4,<br>
--> Verilog code for blocking_caveat design,<br>
       
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4041b7cfe699ff0dc49af57eadd78ef42fbc4169/DAY%204/blocking_caveat_code.v.jpg"> <br>
       Here, we have used the blocking statements which say first will be evaluated based on the past x value and current c value, then the x will be evaluated based on a and b values.<br><br>
       --> RTL level simulation result,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4041b7cfe699ff0dc49af57eadd78ef42fbc4169/DAY%204/blocking_caveat_gtkwave.v.jpg"> <br>
	As we can see in the above waveforms when the value of a and b is zero and c is one it should be supposed to give zero as the output result but it's giving one because x is the past value or it mimics a delay.<br><br>
       -->Graphical representation,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4b31172b2d88320fa615931dba80531ef2953f87/DAY%204/blocking_caveat_graphical_rep_2_.v.jpg"> <br><br>
       --> generated netlist,<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4041b7cfe699ff0dc49af57eadd78ef42fbc4169/DAY%204/blocking_caveat_netlist.v.jpg"> <br>
	This generated netlist we will use for performing gate-level simulation.<br><br>
       --> Gate-level simulation result,<br>
         To perform the gate-level simulation, we can use the same testbench we used for RTL simulation because the primary input and outputs won't change.<br>
        <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/4041b7cfe699ff0dc49af57eadd78ef42fbc4169/DAY%204/blocking_caveat_gtkwave_GLS.v.jpg"> <br>
	As we can see in the above waveforms when the value of a and b is zero and c is one it should give zero as the output result and it's giving zero. So here there is no delay in the value of x.<br>
        Here due to a  problem in the order of blocking statements inside the RTL code their result does not match the Gate-level simulation result. so it's a case of synthesis simulation mismatch.

</details>


## DAY-5- DFT

     
## DAY-6- Introduction to Logic synthesis

<details> 
	<summary> Basics of digital logic design and logic synthesis </summary>
   
-->  Digital circuit:-<br><br>
 
 A digital circuit is an electronic system designed to process digital signals or binary data, which is characterized by discrete values, usually represented as 0s and 1s. These circuits serve as the foundational elements of digital electronics and find extensive application in various electronic devices and systems, including but not limited to computers, smartphones, televisions, and numerous other electronic appliances. These descriptions are typically formulated within the behavioral model of a design, often implemented in hardware description languages (HDL) like VHDL or Verilog. The specification expressed through these programming languages forms the Register-Transfer Level (RTL) representation of the design.<br>
 Digital circuits are built upon several fundamental concepts that form the basis for understanding and designing digital electronic systems. Here are some essential concepts in digital circuits:<br><br>

- Binary Number System<br>
- Logic Gates<br>
- Truth table<br>
- Combinational Logic<br>
- sequential Logic<br>
- Combinational circuits<br>
- Sequential circuits<br>
- State machines<br>
<br><br><br>


--> Logic synthesis:-<br><br>
ogic synthesis is a crucial step in digital circuit design, where a high-level representation of a digital circuit is transformed into a lower-level implementation using basic logic gates, flip-flops, and other standard components. The goal of logic synthesis is to optimize the design for factors like performance, power consumption, and area (size) while preserving the functionality described in the high-level design.<br><br>

Here is an overview of the key aspects of logic synthesis:<br>

1. High-Level Description: Logic synthesis starts with a high-level description of the digital circuit, often expressed using a hardware description language (HDL) like VHDL or Verilog. This description represents the desired functionality of the circuit in an abstract form.<br>

2. Technology Library: Logic synthesis relies on a technology library that contains information about the available logic gates, flip-flops, and other components that can be used to implement the circuit. The library includes details about gate delays, power consumption, and other characteristics of the components.<br>

3. Mapping: During logic synthesis, the high-level description is mapped to the components available in the technology library. This mapping involves selecting the appropriate gates and flip-flops to implement the desired logic functions and storage elements.<br>

4. Optimization: Logic synthesis tools perform various optimizations to improve the circuit's performance and efficiency.
<br>These optimizations can include:<br>

- Logic Optimization: Reducing the number of logic gates used to implement a function, which can lead to smaller and faster circuits.<br>

- Timing Optimization: Ensuring that signals meet specified timing constraints, such as setup and hold times, to ensure correct operation at a desired clock frequency.<br>

- Power Optimization: Minimizing power consumption, especially in battery-powered devices, by optimizing the design for low power usage.<br>

- Area Optimization: Balancing the trade-off between circuit size (area) and performance. Smaller circuits might be more power-efficient but could be slower.<br>

5. Technology Mapping: Selecting the most appropriate gates and components from the technology library to implement the logic functions efficiently.<br>

6. Timing Analysis: Logic synthesis tools perform timing analysis to ensure that the synthesized design meets the required timing constraints, especially in sequential circuits with clock signals.<br>

7. Output Generation: Logic synthesis tools generate output files that describe the synthesized digital circuit. These files can be used for further simulation, verification, or for programming FPGAs or manufacturing ASICs.<br>

8. Iterative Process: Logic synthesis is often an iterative process where designers make adjustments to the high-level description, technology library, or constraints and rerun the synthesis tool until the desired results are achieved.
<br><br>

Logic synthesis is a critical step in digital circuit design, as it bridges the gap between high-level design concepts and the actual hardware implementation. It enables designers to create efficient, optimized, and manufacturable digital circuits.<br><br><br>


</details>
  

  <details>
	  <summary> Introduction to Design compiler(DC)</summary><br><br>
	--> What is Design compiler?<br>
	  Design Compiler, developed by Synopsys, is a pivotal tool in digital circuit design. It transforms high-level Register-Transfer Level (RTL) descriptions, often coded in VHDL or Verilog, into gate-level representations. Leveraging semiconductor technology libraries, it optimizes designs for performance, area, and power consumption. It conducts vital timing analysis, respecting user-defined constraints, and handles complex sequential logic efficiently. Its support for hierarchical designs and scripting enhances productivity. Design Compiler generates gate-level netlists in various formats and interfaces with physical design tools, streamlining the transition from logic synthesis to physical implementation, making it indispensable in ASIC and FPGA design for achieving efficient and reliable digital circuits.<br><br><br>

   --> Common terminologies associated with design compiler(DC) :-<br><br>
   '- SDC :-<br>
   Synopsys Design Constraints(SDC) are guidelines specifying timing, area, power, and other requirements for digital circuit designs. They ensure that synthesized designs meet desired performance criteria and functional behavior during the synthesis and implementation process, crucial for efficient and reliable chip development using Synopsys tools.<br><br>

   -.lib :-<br>
   This information includes data such as gate delay, power consumption, and functionality. .lib files are essential for synthesizing digital designs and ensuring they meet timing and other constraints during the design process. They are provided by semiconductor manufacturers and used by EDA tools to optimize and implement digital circuits efficiently.<br><br>

   - DB :-<br>
   Same as .lib but in a different format.Basically, DC understand libraries in .db format.<br><br>

   - DDC :-<br>
   Synopsys proprietary format for storing the design information. DC can write out and read in DDC.<br><br><br>



   --> Basic DC setup diagram:-<br>
     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/674773a15de5a3131a0a0ffbf6db95aae49a61f8/DAY-6/DC_setup.jpg"> <br>

--> DC synthesis flow:-<br>

 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/674773a15de5a3131a0a0ffbf6db95aae49a61f8/DAY-6/DC%20synthesis%20flow.jpg"> <br>

  </details>







  <details> 
	   <summary> Labs on DC </summary>
	  
  --> First for invoking DC compiler we need to enable C shell and then invoke dC shell with the below commands,<br><br>
	  csh <br>
          dc_shell <br><br>

	 

  --> Then we need to set the target library and link library else it will returns an imaginary pointer library namely your library.<br><br>

  --> Example,<br>

    
  - Verilog code for the design,<br>
  
 ```ruby  
  module lab1_flop_with_en ( input res , input clk , input d , input en , output reg q);
  always @ (posedge clk , posedge res)
  begin
      if(res)
	      q <= 1'b0;
	 else if(en)
	       q <= d;	
  end
  endmodule
 ```
 
 <br><br>
-->  Below is the picture of the output window after compiling. It produces the netlist file, which includes the seqgen library as displayed in the figure. However, it doesn't contain the .db file because we haven't configured the link and target library settings.<br>
   
 
<img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b0a0e0eed5dad950f5e688ea0512f5e4ba0dc8ec/DAY-6/1.jpg"> <br>


-->  Now first we will set the link_library and target_library then link and compile it and then we will write out the netlist by the following commands,<br>

```ruby
    read_verilog <path of design file>
    set target_library <path of .db>
    set link_library { * $path of .db }
    link
    compile
    write -f verilog -out <net_filename>
```

<br><br><br>

--> Below result we can see after compilation,<br>

 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b0a0e0eed5dad950f5e688ea0512f5e4ba0dc8ec/DAY-6/compilatio_complete.png"> <br><br>


 --> Generated netlist,<br>

 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/527beac68a2fc17dda042dade143a2eb9f09c0d5/DAY-6/can%20see%20the%20netlist%20file%20created%20by%20using%20sky130.png"> <br><br>
 Since, we have set the target and link library so we can see in the netlist that it's using cells from the sky130.<br><br>
 

 
 **design vision**

 --> Design Vision, part of Synopsys' EDA suite, is essential for digital circuit design. It analyzes RTL descriptions, performs logic synthesis, manages constraints, and conducts timing analysis. This ensures correctness, optimization, and adherence to constraints before the physical implementation, streamlining and improving the reliability of the design process.<br><br>

 - To launch design vision,<br>
 
   ```ruby
     csh
     design_vision
   ```
 - For writing out the DDC in DC shell command,<br>
      **write -f ddc -out <filename_name>**

  - Next, you can initiate the graphical user interface (GUI) and open the previously generated .ddc file. This .ddc file holds session-specific tool memory information in Synopsys' proprietary format, exclusively accessible by Synopsys tools. When reading the .db file, it automatically includes the linked .db file, as demonstrated in the figure below,<br>
   <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b0a0e0eed5dad950f5e688ea0512f5e4ba0dc8ec/DAY-6/after%20opening%20design%20vision%20we%20will%20see%20something%20like%20this%20view.png"> <br><br>

  - For viewing the schematic of the design,<br>
     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b0a0e0eed5dad950f5e688ea0512f5e4ba0dc8ec/DAY-6/3.jpg"> <br><br>


  - Gate-level implementation,<br>
  <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/527beac68a2fc17dda042dade143a2eb9f09c0d5/DAY-6/lab_1_schematic.png"> <br><br>
     


  **.synopsys_dc.setup**

  - Imagine a scenario with multiple indispensable .db files where manually configuring each one is impractical. To address this, you can create a file named .synopsys_dc.setup in your workspace's home directory. <br>

  -  When invoking dc_shell, it checks for the .synopsys_dc.setup file in the user's home directory. The priority order is as follows: if the file exists in the user's home directory, it takes precedence, and the installed (default) setup is disregarded. If not found, the installed setup is used. This file streamlines tool setup by automatically configuring all necessary .db files, eliminating repetitive tasks during dc_shell invocation.<br>

   
  </details>




  <details>
	  <summary> Tcl scripting </summary>
	  Tcl(Tool Command Language) is a dynamic and interpreted scripting language initially crafted as a simple yet powerful scripting tool. Renowned for its user-friendly syntax, versatility, and expandability, Tcl enjoys broad usage across diverse domains and applications.<br><br>
-Basic tcl commands,<br>
-Variable assign,<br>
	  
   ```ruby
     set a 10
     set b 10
     set a [expr $a + $b]
   ```

- If else,<br>
	  
    ```ruby
    if { condition } {
    <statements>
    } else {
    <statements>
    }
   ```


- for loop,<br>
	  
```ruby 
for {<looping variable>} {condition} {incr/decr} {
<statements>
}
```


- while loop,<br>
	  
   ```ruby
   while {<condition>} {
   <statements>
   }
   ```



- Foreach,<br>

```ruby
 foreach var list{
statement
}
```

- Foreach in collection,<br>

```ruby
foreach_in_collection var collection {
statement
}
```
<br><br><br>

**Examples,** <br>

**1. set variable**<br>
  <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/87397a2368ff49e151c66e70846d0a2c7ec8cd8f/DAY-6/tcl_setting_variable.png"> <br><br>

**2. while loop**<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/87397a2368ff49e151c66e70846d0a2c7ec8cd8f/DAY-6/tcl_running_while_loop1.png"> <br><br>

  
**3. for loop**<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/87397a2368ff49e151c66e70846d0a2c7ec8cd8f/DAY-6/tcl_running_for_loop.png"> <br><br>


**4. set list**<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/87397a2368ff49e151c66e70846d0a2c7ec8cd8f/DAY-6/for_setting_the_list.png"> <br><br>


**5. Foreach for looping through the list**<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/87397a2368ff49e151c66e70846d0a2c7ec8cd8f/DAY-6/for_looping_through_the_list.png"> <br><br>


**6. Command for collection of all cells present in .lib for AND cell**<br>

```ruby
  get_lib_cells */*and*
```

**7. collection of AND cells present in library**<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/87397a2368ff49e151c66e70846d0a2c7ec8cd8f/DAY-6/collection%20of%20AND%20cells%20present%20in%20library.png"> <br><br>


**8. foreach in collection, looping through**<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/87397a2368ff49e151c66e70846d0a2c7ec8cd8f/DAY-6/looping%20through%20my%20collection%20of%20AND%20cells.png"> <br><br>


**Creating a small script**<br>
--> first launch gvim within dc_shell,<br>
    **command: sh gvim &**

**9. Script for printing multiplication**<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/42d1492b3aa9a2a53863d7811e1c1b55f124fc92/DAY-6/myscript_for_multiplication.png"> <br><br>
  -Output of script,<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/42d1492b3aa9a2a53863d7811e1c1b55f124fc92/DAY-6/printing_multiplication_table_through_script.png"> <br><br>


 **10. script for printing list**<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/42d1492b3aa9a2a53863d7811e1c1b55f124fc92/DAY-6/script%20for%20list%20and%20looping%20through%20my%20list.png"> <br><br>
 -Output of script,<br>
 <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/42d1492b3aa9a2a53863d7811e1c1b55f124fc92/DAY-6/by%20script%20looping%20through%20my%20list.png"> <br><br>
 

  </details>




## DAY-7 Basics of STA

<details>
	<summary> Introduction to STA </summary>

-->  Static Timing Analysis (STA) is a fundamental technique in the field of digital integrated circuit design. STA is used to evaluate and ensure that a digital circuit operates correctly with respect to timing requirements. Here's a some key concepts of STA:<br><br>

 1. Timing paths: In a digital circuit, there are paths from input to output that define the maximum and minimum delay paths. These paths include combinational logic gates and interconnects.<br>

     
      2. Clock Domains: Many digital circuits have multiple clock domains with their own clock signals. STA must account for interactions between these domains.<br>


      3. Setup and Hold Time: Setup time is the minimum time data must be stable before the clock edge, while hold time is the minimum time data must remain stable after the clock edge for correct operation.<br>

      4. Clock-to-Q Delay: This represents the time it takes for the output of a flip-flop or latch to respond to a clock edge.<br>

      5. Slack: Slack is the difference between the time available for a signal to propagate and the time it actually takes. Negative slack indicates a violation of timing constraints.<br>

      6. Max Delay and Min Delay: STA calculates the maximum and minimum delay for each path in the circuit to ensure that signals meet their setup and hold time requirements.<br>

      7. Clock Skew: Clock skew refers to the variation in arrival times of the clock signal at different elements of the circuit. Reducing clock skew is crucial to achieving better timing performance.<br>

      8. Propagation Delay: The time it takes for a signal to propagate from one point in the circuit to another. This includes both combinatorial logic delay and interconnect delay.<br><br>

      In summary, Static Timing Analysis is a critical step in ensuring that digital integrated circuits meet their performance requirements. It helps designers verify and optimize the timing behavior of the circuit, allowing for correct and reliable operation.<br><br><br>


**-->Water bucket analogy to understand delay :-**  <br>

In the analogy, the water tap represents the inflow of current in digital circuits, while the bucket symbolizes the load capacitance, which stores electrical charge. Filling the bucket illustrates the process of charging the load capacitance, and the time it takes to fill it depends on both the current flow rate (from the tap) and the capacitance's size (the bucket's capacity). This analogy helps understand how delay in digital circuits is modeled, with delay being analogous to the time it takes to fill the bucket to a certain charge level, where it depends on the flow rate (current) and the capacitance (load) characteristics.<br>


- Increasing Load Capacitance (Bigger Bucket) in a digital circuit leads to longer delay times, as it takes more time to charge the larger capacitance. Conversely, increasing the Inflow of Current (Higher Flow Rate) reduces delay times, analogous to a faster fill rate when the tap flows more water into the bucket.<br>

- Digital circuit optimization balances load capacitance (bucket size) and current inflow (tap flow rate) to meet timing constraints.<br><br>




**Timing arcs:-**

Timing arcs, also known as timing paths or timing arcs, are essential components of static timing analysis (STA) in digital circuit design. They represent the paths through which signals propagate within a digital circuit.Here are some key aspects of timing arcs:<br><br>

    
 Signal Propagation Paths: Timing arcs represent the paths through which digital signals traverse the circuit, including logic gates, interconnects, flip-flops, and latches.<br>
 Signal Delays: Timing arcs account for the delays introduced by logic gates, interconnects, and flip-flops along the signal path. These delays affect the overall performance of the circuit.<br>
 Critical Paths: Some timing arcs are critical paths that have the most significant impact on circuit performance. These paths must be carefully analyzed and optimized to meet timing constraints.<br>
  Setup and Hold Times: Timing arcs assess whether data signals meet setup and hold time requirements at flip-flops. Setup time specifies how early data must be stable before a clock edge, while hold time defines how long data must remain stable after the clock edge.<br>
  Clock-to-Q Delays: Timing arcs calculate the time it takes for data to propagate from the input of a flip-flop to the output (Q) in response to a clock edge, ensuring it occurs within specified limits.<br>
  Clock Domain Crossings: In multi-clock domain designs, timing arcs may involve crossing clock domain boundaries, requiring special consideration and synchronization techniques.<br>
  Max Frequency Constraints: Timing arcs are used to assess whether the circuit can operate at a specified maximum clock frequency while meeting timing requirements.<br><br>

  Understanding and managing these key aspects of timing arcs is crucial for designing digital circuits that operate reliably and meet their timing requirements.<br><br><br>


**--> Timing paths**:-<br><br>



 **1.Reg to reg timing paths**<br>
Reg-to-Reg timing paths encompass the flow of signals between two sequential elements, usually flip-flops or latches, within a digital circuit.<br>

Constraints: These paths are predominantly governed by clock-related parameters, encompassing the clock period (maximum delay), setup time (maximum delay), and hold time (minimum delay).<br>

Objective: Reg-to-Reg paths serve the critical function of guaranteeing the dependable transfer of data between registers within designated clock cycles, all while adhering to the essential setup and hold time prerequisites. This ensures the accuracy and reliability of data propagation through the circuit.<br><br>


**2.Input to reg timing paths**<br>

Description: In2Reg paths encompass the journey of signals originating from external input pins and transitioning into registers within the digital chip.<br>

Constraints: These paths are subject to constraints related to external input delay, input transition time, and clock period. These constraints are essential to ensure that incoming input signals align with the timing requirements when they are captured by the registers.<br>

Objective: The disciplined management of In2Reg paths serves the crucial purpose of ensuring that external input signals are accurately sampled and adhere to the requisite setup time criteria as they enter the chip. This guarantees the integrity and reliability of the input data within the digital system.<br><br>


**3.Reg to output timing paths**<br>

Description: Reg2Out paths encompass the route taken by signals as they journey from a register within a digital chip to an external output pin.<br>

Constraints: These paths are rigorously governed by various factors, including external output delay, output load, and clock period. These constraints are fundamental in guaranteeing that the output signal adheres to the specified timing requirements.<br>

Objective: The precise control of Reg2Out paths serves the essential purpose of ensuring that output signals are launched accurately and consistently meet the necessary timing criteria. This consideration extends to external influences, such as board-level delays and load, to ensure the reliability of the signal as it leaves the digital chip.<br><br>


**4.input to output timing paths**<br>

In Static Timing Analysis (STA), the "Input to Output" timing path refers to the path that traces the journey of a signal from an input pin of a digital chip or circuit to an output pin. This path is crucial to ensuring that the output signal meets the required timing constraints.<br>
Ideally we don't want this paths.<br><br><br>

- In digital design, remember that we must control not just how slow signals can be (setup) but also how fast they can change (hold). Achieving both setup and hold requirements is vital to make sure data is captured and sent accurately in a synchronized digital system.<br>
- Designers rely on these rules and special tools to check if a digital circuit works well and consistently in various situations, making sure it follows the timing rules for signals going in and out.<br><br>


</details>


<details>
	<summary> Timing .lib </summary>
 
-->	A Timing .lib (Library) file, often referred to as a Liberty file, is a vital asset in digital design and static timing analysis (STA). This file serves as an encyclopedia of essential information about the timing properties and functionality of standard cells (like logic gates) and other components within digital integrated circuit designs. Here are the critical aspects of a Timing .lib file:<br><br>

1. Cell Library Information: Within this file, you'll discover details about the available cells in the library. This includes their names, types (e.g., AND, OR, Flip-Flop), and unique attributes. Essentially, it's a catalog of the fundamental building blocks that designers employ to craft digital circuits.<br>

2. Timing Models: Timing .lib files outline precise timing models for each cell. These models provide insights into various aspects, including delay, transition times, power consumption, and more. The primary timing characteristics covered encompass:<br>

Cell Delay: This reflects the time needed for a signal to traverse the cell, accounting for both internal logic and interconnect delays.<br>

Rise and Fall Delays: These factors account for delays associated with signal transitions, be it rising or falling edges.<br>

Slew Rate: It specifies how quickly the voltage of the signal changes at the cell's output.<br>

Setup and Hold Time: These parameters define the stability requirements for input data concerning the clock edge, crucial for proper capture by flip-flops or latches.<br>

Clock-to-Q Delay: For flip-flops, this metric details the delay from the clock edge to the data output.<br>

Power Consumption: Information on power consumption, covering static and dynamic power, is included, facilitating power analysis.<br>

3. Constraints and Corner Cases: Timing .lib files often encompass data for diverse operational conditions or process corners. These variations, spanning typical, worst-case, or best-case scenarios, account for manufacturing process discrepancies and temperature extremes.<br>

4. Library Characterization: Statistical data, such as mean and standard deviation, may be incorporated into the .lib file. This data accounts for manufacturing variations and enables statistical STA (SSTA).<br>

5. Interconnect Models: In addition to cell-specific timing models, .lib files may introduce interconnect models that describe the behavior of wires and routing resources. This encompasses attributes like resistance, capacitance, and propagation delays.<br><br>

In essence, Timing .lib files are the linchpin that bolsters the reliability, efficiency, and success of digital design endeavors, serving as an essential resource for designers and their indispensable companions in the world of EDA tools.<br><br><br>

  <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3054a6e9a4c03e8dc8ec03194a52ea95be8ced46/DAY%207/.lib%20file.jpg"> <br><br>


--> .lib also contains leakage power , area , timing sense of each different flavours of gate cells.<br>
          <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3054a6e9a4c03e8dc8ec03194a52ea95be8ced46/DAY%207/.lib%20contains%20area%2C%20leakage%20power.jpg"> <br><br>

   **--> Lookup table :-** <br>
  - A Look-Up Table (LUT) in a Liberty file is like a recipe card for a specific type of digital building block. This recipe explains how this block behaves and how fast it works. These recipes are kept in Liberty files, which are like big libraries of these building blocks used by computer chip designers. These designers use these recipes, found in the Liberty files, to put together their digital creations, making the whole process faster and more efficient.<br><br>
   
   index1 -> input transition <br>

   index2 -> output load capacitance<br>
   Example,
       <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3054a6e9a4c03e8dc8ec03194a52ea95be8ced46/DAY%207/lookup%20table.jpg"> <br><br>



  **unateness**<br>

 - Unateness is a fundamental concept in digital logic that helps us understand how a specific variable affects the behavior of a Boolean function. It's all about figuring out if changing the value of an input variable will reliably change the function's output in a certain way.<br>

Here are the two main types of unateness:<br><br>

**1. Positive Unate (PU):** <br>

- Think of a variable as positively unate if, no matter what you do with the other variables, increasing its value from 0 to 1 will always make the function's output go up.<br>

**2. Negative Unate (NU):** <br>

- Now, imagine a variable as negatively unate if, regardless of what the other variables are doing, increasing its value from 0 to 1 will always make the function's output go down.<br>

 **3.Binate (BI) or Non Unate:** <br>
- A variable is considered binate with respect to a function if its behavior is not strictly positive unate or negative unate. In other words, there are cases where increasing the variable value may increase the output, and there are cases where increasing the variable value may decrease the output.<br><br>

In summary, unateness is a concept used to characterize the behavior of variables in Boolean functions and is an important consideration in digital logic design and optimization. It helps determine how changes in variables affect the behavior of logical functions and can guide design decisions to improve circuit performance and simplify logic expressions.<br><br>


**--> Example for unateness,** <br>

 **1. AND gate unateness** <br>
     <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3054a6e9a4c03e8dc8ec03194a52ea95be8ced46/DAY%207/AND%20gate%20unateness.jpg"> <br><br>

 **2. DFF negedge triggered unateness** <br>
   <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3054a6e9a4c03e8dc8ec03194a52ea95be8ced46/DAY%207/unateness%20of%20Dff%20negative%20edge%20triggered.jpg"> <br><br>

 **3. DLatch Poslevel triggered unateness**<br>
   <img width="600" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3054a6e9a4c03e8dc8ec03194a52ea95be8ced46/DAY%207/unateness%20of%20Dlatch%20positive%20level%20triggered.jpg"> <br><br>

</details>

<details>
	<summary>Lab on .lib</summary>

 **Examples,** <br>
  --> Print the list of cells from the collection,<br>
	  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/a7f6b727946cfa8714ea2ade74d96f7cef87409e/DAY%207/LAB_printing%20the%20list%20of%20and%20gate%20in%20.lib.jpg"> <br><br>

--> Getting functionality of a cell in dc_shell,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/a7f6b727946cfa8714ea2ade74d96f7cef87409e/DAY%207/LAB_getting%20functinality%20of%20cells.jpg"> <br><br>
   --> prints the pins along with the direction of and2_0 gate,<br>
         <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/a7f6b727946cfa8714ea2ade74d96f7cef87409e/DAY%207/LAB_prints%20the%20pins%20along%20with%20direction%20of%20and2_0%20gate.jpg"> <br><br>

  --> A below tcl Script takes the list of cells as input and prints the output pins along with its functionality,<br>

  ```ruby
  set mylist [list sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2_1 \
 sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2_2 \
 sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2_4 \
 sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2_8 \
 sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2b_1 \
 sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2b_2 \
 sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand2b_4 \
 sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand3_1 \
 sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand3_2 \
 sky130_fd_sc_hd__tt_025C_1v80/sky130_fd_sc_hd__nand3_4 ];

 foreach var $mylist {
  foreach_in_collection var_pins [get_lib_pins ${var}/* ] {
      set pin_name [get_object_name $var_pins];
      set pin_dir [get_lib_attribute $pin_name direction];
      if { $pin_dir == 2 } {


          set pin_func [get_lib_attribute $pin_name function];

          echo $pin_name $pin_dir $pin_func ;
       }
     }
   }
   ```

--> Output result of script,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/a7f6b727946cfa8714ea2ade74d96f7cef87409e/DAY%207/LAB_output%20of%20the%20script.jpg"> <br><br>
    
</details>



## DAY-8 Advanced constraints

<details>
	<summary> Clock Terminologies </summary>


 --> Clock generator :-<br>
       
In Very Large Scale Integration (VLSI) design, a clock generator is a crucial component that plays a vital role in ensuring that the digital circuits and components within an integrated circuit (IC) operate synchronously and with precise timing. Here are some key aspects of clock generators in VLSI:<br><br>

Clock Distribution: VLSI chips often contain numerous digital components, such as flip-flops, registers, and logic gates. These components rely on a common clock signal to ensure synchronized operation. The clock generator generates this clock signal and distributes it across the chip.<br>

Clock Tree Synthesis: Clock tree synthesis is the process of designing the distribution network for the clock signal. It involves determining the optimal routing of clock lines and inserting buffer stages as needed to ensure that the clock signal reaches all parts of the chip with minimal skew (timing variation) and delay.<br>

Clock Skew: Clock skew refers to the variation in arrival times of the clock signal at different points on the chip. Excessive clock skew can lead to timing violations, where certain parts of the chip may receive the clock signal too early or too late. Clock generators are designed to minimize clock skew.<br>

Frequency and Duty Cycle Control: In VLSI design, clock generators allow designers to specify the clock frequency and duty cycle to meet the specific requirements of the chip. These parameters are critical for ensuring that the digital circuits within the chip operate at the desired speed and timing.<br>

Phase-Locked Loops (PLLs): PLLs are commonly used in VLSI clock generators to generate stable and precise clock signals. PLLs can lock onto an external reference clock and generate a stable output clock signal with a desired frequency and phase relationship.<br>

Clock Gating: VLSI clock generators may incorporate clock gating logic. Clock gating allows designers to enable or disable the clock signal to specific parts of the chip, conserving power when those parts are not in use.<br>

Clock Domain Crossing (CDC) Management: In complex VLSI designs, there may be multiple clock domains with different clock frequencies. Clock generators ensure that signals crossing between different clock domains are properly synchronized to avoid metastability issues.<br>

Low Jitter: Jitter refers to the variation in the timing of clock edges. Low jitter clock generators are essential in high-performance VLSI designs, especially in applications where precise timing is critical, such as high-speed communication interfaces.<br>

Clock Fail-Safe Mechanisms: In some cases, VLSI clock generators may incorporate fail-safe mechanisms to detect and handle clock-related faults, ensuring the reliable operation of the chip.<br>

Customization: VLSI designers often have the flexibility to customize the clock generator's settings, including the choice of PLL parameters, clock distribution strategies, and clock gating logic, to optimize the chip's performance and power consumption.<br><br>


In summary, clock generators in VLSI play a pivotal role in ensuring the proper operation of digital circuits by generating, distributing, and managing clock signals with precision, low skew, and low jitter. They are a critical component of the overall clocking architecture of VLSI chips, helping to meet the stringent timing requirements of modern integrated circuits.<br><br>


--> Types of clock generator:-<br><br>
- Crystal Oscillator<br>
- Voltage-Controlled Oscillator (VCO)<br>
- Phase-Locked Loop (PLL)<br>
- Delay-Locked Loop (DLL)<br>
- Ring Oscillator<br>
<br>

--> Clock Distribution:-<br>

Once generated, clock signals need to be distributed to various parts of the IC while maintaining their timing integrity. Clock trees are used for this purpose, which involves a hierarchical network of buffers and repeaters to ensure the clock signal reaches all parts of the chip with minimal skew.<br><br>

-> Clock skew:-<br>  is a phenomenon in digital design and VLSI (Very Large Scale Integration) circuits where clock signals, which are supposed to be synchronized and have the same edge (rising or falling), arrive at different parts of the circuit at slightly different times.<br>
       Positive and Negative Skew: Clock skew can be further categorized into positive skew and negative skew based on whether clock signals arrive later or earlier than the ideal clock edge, respectively.
<br>
Positive Skew: Positive skew occurs when clock signals arrive at different destinations later than the ideal clock edge. It can lead to setup time violations.<br>
- Ts + Skew ≤ Tcq + Tcomb + Tst <br>
Negative Skew: Negative skew occurs when clock signals arrive earlier than the ideal clock edge at different destinations. Negative skew can result in hold time violations.<br>
- Tc2q + Tcomb ≥ Thold + Tskew <br><br>

-> Setup and Hold Time Violations:- <br>
Clock skew can lead to setup time violations, where data may not be stable for the required setup time before a clock edge arrives at some elements but is stable for too long at others. Conversely, hold time violations can occur when data remains stable for too long after the clock edge.<br><br>

-> Clock jitter:-<br> 
it refers to the fluctuation or lack of precision in the timing of a clock signal, which leads to deviations of the actual clock signal edges from their expected, evenly spaced positions. Clock jitter can arise from various sources and can exert notable effects on the operational efficiency and dependability of digital systems.<br><br>

-> Clock latency:-<br> 
it denotes the temporal delay or propagation delay encountered by a clock signal as it traverses from its origin to different points within an integrated circuit (IC) or digital system. It denotes the duration required for the clock signal to navigate through various components, interconnections, and buffers before it reaches its intended destination.<br><br>

- Source latency:<br> also recognized as clock source latency, pertains to the delay or latency that arises from the clock generation circuitry at its inception, preceding the distribution of the clock signal to other segments of the integrated circuit (IC) or digital system.<br>
- Network latency:<br> concerning a clock, it typically denotes the delay or temporal discrepancy that arises when transmitting a clock signal through a network or communication medium.<br><br>

</details>





<details>
	<summary> Lab on some useful command for constraining design </summary>
	
--> The Verilog code for the design we will use to perform our lab is,<br>
	 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/694db1eb2787833f0992cd829838516e2bdf2a9f/DAY8/8.2.1_lab8_circuit.v.png"> <br><br>
--> Going through each collection of ports,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/694db1eb2787833f0992cd829838516e2bdf2a9f/DAY8/2_going_through%20the%20each%20collection%20of%20port.png"> <br><br>
--> it_shows the direction of rst port,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/694db1eb2787833f0992cd829838516e2bdf2a9f/DAY8/2_it_shows%20the%20direction%20of%20rst%20port.png"> <br><br>
--> small script for port name with it's direction,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/694db1eb2787833f0992cd829838516e2bdf2a9f/DAY8/2_port%20name%20with%20it's%20direction.png"> <br><br>
--> For viewing all the cells in design,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/694db1eb2787833f0992cd829838516e2bdf2a9f/DAY8/2_for%20viewing%20all%20the%20cells%20in%20design.png"> <br><br>
--> for viewing a particular cell U9 is hierarchical or not,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/694db1eb2787833f0992cd829838516e2bdf2a9f/DAY8/2_for%20viewing%20a%20particular%20cell%20U9%20is%20hierarchical%20or%20not.png"> <br><br>
--> It will show all the physical cells,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/694db1eb2787833f0992cd829838516e2bdf2a9f/DAY8/2_it%20will%20show%20all%20the%20physical%20cells.png"> <br><br>

--> ref name basically shows the name of the cell in .lib,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e95ffb895ec43535edfe1b888de69a4781930135/DAY8/2_ref_name%20is%20basically%20shows%20the%20name%20of%20the%20cell%20in%20.lib.png"> <br><br>
--> Small script which will show cell name with its ref name,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e95ffb895ec43535edfe1b888de69a4781930135/DAY8/2_it%20will%20show%20cell%20name%20with%20it's%20ref%20name.png"> <br><br>
--> After writing out the DDC format for it and reading that DDC file in design vision, we can see the schematic view for lab8_circuit,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e95ffb895ec43535edfe1b888de69a4781930135/DAY8/2_can%20see%20the%20schematic%20view%20for%20lab8_circuit.png"> <br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e95ffb895ec43535edfe1b888de69a4781930135/DAY8/2_can%20see%20the%20schematic%20view%20for%20lab_circuit_2.png"> <br><br>
--> small script to see the direction and all the pins connected to net n5 in the design vision,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e95ffb895ec43535edfe1b888de69a4781930135/DAY8/2_can%20see%20the%20direction%20and%20all%20the%20pins%20connected%20to%20net%20n5%20in%20design%20vision.png"> <br><br>


--> Going through a collection of pins one by one,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0d16d628a556e469d87635e5a70016715f33fc3d/DAY8/2_2%20going%20through%20collection%20of%20pins%20one%20by%20one.png"> <br><br>
--> Command for viewing the direction of any particular pin,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0d16d628a556e469d87635e5a70016715f33fc3d/DAY8/2_2%20for%20viwing%20the%20direction%20of%20any%20particular%20pin.png"> <br><br>
--> Command to check for any particular pin whether it's a clock pin or not,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0d16d628a556e469d87635e5a70016715f33fc3d/DAY8/2_2%20to%20check%20for%20any%20particular%20pin%20whether%20it's%20clock%20pin%20or%20not%20.png"> <br><br>
--> This script will not work because the clock can only for an input port,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0d16d628a556e469d87635e5a70016715f33fc3d/DAY8/2_2%20this%20script%20will%20not%20work%20because%20clock%20can%20only%20for%20input%20port%20.png"> <br><br>
--> Writing a small script for what all pins in my collection are clock pins considering first that's an input pin actual pin,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/0d16d628a556e469d87635e5a70016715f33fc3d/DAY8/2_2%20writing%20small%20script%20for%20what%20all%20pins%20in%20my%20collection%20are%20clock%20pins%20considering%20first%20that's%20a%20input%20pin%20actual%20pin.png"> <br><br>
 
--> creating a clock,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df71eeefecff0c5bc08a085f1724c7f95a8ae725/DAY8/2_3%20creating%20a%20clock.png"> <br><br>
--> command to see the period of any particular clock,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df71eeefecff0c5bc08a085f1724c7f95a8ae725/DAY8/2_3%20command%20to%20see%20the%20period%20of%20any%20particular%20clock.png"> <br><br>
--> command to see, if any particular clock is generated or not,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df71eeefecff0c5bc08a085f1724c7f95a8ae725/DAY8/2_3%20command%20to%20see%20any%20particular%20clock%20is%20generated%20or%20not.png"> <br><br>
--> command to get the report for clocks,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df71eeefecff0c5bc08a085f1724c7f95a8ae725/DAY8/2_3%20command%20to%20get%20the%20report%20for%20clocks.%20png"> <br><br>
--> name of clocks,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df71eeefecff0c5bc08a085f1724c7f95a8ae725/DAY8/2_3%20name%20of%20clocks.png"> <br><br>
--> the script result in which it's showing at each register pin which clock is reaching,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df71eeefecff0c5bc08a085f1724c7f95a8ae725/DAY8/2_3%20the%20script%20result%20in%20which%20it's%20showing%20at%20each%20register%20pin%20which%20clock%20is%20reaching.%20png"> <br><br>
--> This script will also tell us at each register pin which clock is reaching,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df71eeefecff0c5bc08a085f1724c7f95a8ae725/DAY8/2_3%20this%20script%20will%20also%20tell%20us%20at%20each%20register%20pin%20which%20clock%20is%20reaching.%20png"> <br><br>
--> clock can also be created on any pin, the tool will accept it but it means less. can see in the below case we have created a clock on the D pin of the register which is not at all meant to receive the clock. *Never create a clock on some pin*,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df71eeefecff0c5bc08a085f1724c7f95a8ae725/DAY8/2_3%20clock%20can%20also%20be%20created%20on%20any%20pin%2C%20tool%20will%20accept%20it%20but%20it%20meaning%20less.%20can%20see%20in%20below%20case%20we%20have%20created%20a%20clock%20on%20D%20pin%20of%20register%20which%20is%20not%20at%20all%20meant%20to%20receive%20the%20clock.%20*never%20create%20clock%20on%20some%20pin*.%20png"> <br><br>
--> In case you created any wrong clock, the command to remove the clock is,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df71eeefecff0c5bc08a085f1724c7f95a8ae725/DAY8/2_3%20in%20case%20you%20created%20any%20wrong%20clock%2C%20the%20command%20to%20remove%20the%20clock%20is.%20png"> <br><br>
 -->creating a clock which will have the first 5nsec for low and then from 5 to 10 nsec high,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/88ac16b43f8a8304f7cd22d52ec4abfe93e6980b/DAY8/2_3%20creating%20a%20clock%20which%20will%20have%20first%205nsec%20for%20low%20and%20the%20from%205%20to%2010%20nsec%20high.%20png"> <br><br>
--> report for the created clock which will have the first 5nsec for low and then from 5 to 10 ns high,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/88ac16b43f8a8304f7cd22d52ec4abfe93e6980b/DAY8/2_3%20%20report%20for%20created%20clock%20which%20will%20have%20first%205nsec%20for%20low%20and%20the%20from%205%20to%2010%20nsec%20high.%20png"> <br><br>
--> creating a clock for 25% duty cycle,<br>
   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/88ac16b43f8a8304f7cd22d52ec4abfe93e6980b/DAY8/2_3%20creating%20a%20clock%20for%2025%25%20duty%20cycle.%20png"> <br><br>
--> This kind of clock can also be useful in some cases like there are some protocol which is in the starting phase and don't want the clock to be high but after some time it is required to be high so in those cases this type of clock is required,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/88ac16b43f8a8304f7cd22d52ec4abfe93e6980b/DAY8/2_3%20this%20kind%20of%20clock%2C%20can%20also%20be%20useful%20in%20some%20cases.%20png"> <br><br>

</details>



<details>
	<summary> Constraining design for Reg to Reg path</summary>

 --> We know the reg-to-reg path is constrained by the clock, so first create a clock else it will show the path is unconstrained. Now if we generate report after creating clock it looks like,<br>
	<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9131b001f2ccc5a0c0b0759f3b54bc9d44986e2e/DAY8/2_4%20after%20creating%20the%20clock%20the%20path%20is%20constrained%20and%20it's%20showing%20timing%20is%20met.%20png"> <br>
 
 --> Can see after creating a clock, the path is constrained and timing is met.<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9131b001f2ccc5a0c0b0759f3b54bc9d44986e2e/DAY8/2_4%20after%20creating%20the%20clock%20the%20path%20is%20constrained%20and%20it's%20showing%20timing%20is%20met.%20png"> <br><br>

 --> Modeling one by one practical effort of the clock,<br>
     <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9131b001f2ccc5a0c0b0759f3b54bc9d44986e2e/DAY8/2_4%20modeling%20one%20by%20one%20practical%20effort%20of%20clock.%20png"> <br><br>

--> In the report also we can also see that we have modeled clock latency and clock uncertainty,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9131b001f2ccc5a0c0b0759f3b54bc9d44986e2e/DAY8/2_4%20now%20in%20report%20also%20we%20can%20see%20that%20we%20have%20modeled%20clock%20latency%20and%20clock%20uncertainity.%20png"> <br><br>

--> Report for hold analysis,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9131b001f2ccc5a0c0b0759f3b54bc9d44986e2e/DAY8/2_4%20after%20modeling%20report%20for%20hold%20time%20analysis.%20png"> <br><br>
</details>


<details> 
<summary> Constraining for input and output paths </summary>

--> First, let model for inputs,<br>
--> modeling the input delay for max(setup),<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c580120e431720c350f9049c6695f3aad63e326a/DAY8/2_5%20modeling%20the%20input%20delay%20for%20max(setup).%20png"> <br><br>
--> After modeling input delay we can see now the proper path is reported,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c580120e431720c350f9049c6695f3aad63e326a/DAY8/2_5%20after%20modelling%20input%20delay%20we%20can%20see%20now%20properly%20path%20is%20reported.%20png"> <br><br>

--> command to see report in a more organized manner,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c580120e431720c350f9049c6695f3aad63e326a/DAY8/2_5%20command%20to%20see%20report%20in%20more%20organized%20manner.%20png"> <br><br>
--> It will say path unconstrained because we haven't yet constrained for min(hold),<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c580120e431720c350f9049c6695f3aad63e326a/DAY8/2_5%20it%20will%20say%20path%20unconstarined%20because%20we%20haven't%20yet%20constrained%20for%20min(hold).%20png"> <br><br>
--> Constraining for min(hold),<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c580120e431720c350f9049c6695f3aad63e326a/DAY8/2_5%20constraining%20for%20min(hold).%20png"> <br><br>
 --> Can see here in the report, that we haven't yet modeled for input transition,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c580120e431720c350f9049c6695f3aad63e326a/DAY8/2_5%20can%20see%20here%20we%20havn't%20yet%20modelled%20for%20input%20transition.%20png"> <br><br>

--> modeling for input transition,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c580120e431720c350f9049c6695f3aad63e326a/DAY8/2_5%20modelling%20for%20input%20transition.%20png"> <br><br>

--> We can see here in the report that, after modeling for input transition we can see available margin is going down,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/c580120e431720c350f9049c6695f3aad63e326a/DAY8/2_5%20after%20modelling%20for%20input%20transition%20we%20can%20see%20available%20margin%20is%20going%20down.%20png"> <br><br>

--> Now, we will model for an output path,<br>
--> Modeling for output delay,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7aaf0a9017f54e9d1305579a4684f7dad6053c29/DAY8/2_5%20modelling%20for%20output%20delay.%20png"> <br><br>

--> Can see the report after modeling output delay,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7aaf0a9017f54e9d1305579a4684f7dad6053c29/DAY8/2_5%20can%20see%20the%20report%20after%20modelling%20output%20delay.%20png"> <br><br>

--> Setting load for output,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7aaf0a9017f54e9d1305579a4684f7dad6053c29/DAY8/2_5%20setting%20load%20for%20output%20.%20png"> <br><br>

--> After setting load for output can see the difference in arrival time in the report,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7aaf0a9017f54e9d1305579a4684f7dad6053c29/DAY8/2_5%20after%20setting%20load%20for%20output%20can%20see%20the%20difference%20in%20arrival%20time%20in%20report.%20png"> <br><br>

--> Can set the load for min also and see the corresponding report for that,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7aaf0a9017f54e9d1305579a4684f7dad6053c29/DAY8/2_5%20can%20set%20the%20load%20for%20min%20also%20and%20see%20the%20corresponding%20report%20for%20that.%20png"> <br><br>

--> After setting load for output can see the difference in arrival time in the report for min,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7aaf0a9017f54e9d1305579a4684f7dad6053c29/DAY8/2_6%20after%20setting%20load%20for%20output%20can%20see%20the%20difference%20in%20arrival%20time%20in%20report%20for%20min.%20png"> <br><br>



-->  The output OUT_Y is constrained with the clock leaving the module. It's logically the same but physically not because there will be a routing delay. For every flop we have modeled the routing delay by using the clock uncertainty and clock latency command but at the output clock there is nothing modeled. So to model this we are going to do something called Generated clocks.<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/21f4f61704a272da0523d0617053696c7dcc0775/DAY8/IMG_20230913_024934.jpg"> <br>
--> Generated clocks are always created w.r.t master clocks(clocks at clock source or at primary IO pins).<br>
<br>
--> How the clocks are propagated:-<br>
   ->  Once a clock is created on a pin/port, DC will propagate that clock downstream based on the timing arcs. all the timing arcs from the definition point will see the clock propagation by default.<br><br>


--> Now, we will look at how to specify the constraints for generated clocks (because since this out_clk may see further routing delay it's better to annotate this clock separately),<br>
--> Command for creating a generated clock,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7fb9bb75d67e07afe5044d453f34ed2a218f9114/DAY8/3_2%20creating%20generated%20clock.%20png"> <br><br>
--> can see report,<br>
<img width="800" alt="netlist" src="DAY8/3_2 can see report.png"> <br><br>
--> it's showing timing w.r.t MYCLK only but i want the capture to be w.r.t MYGEN_CLK,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7fb9bb75d67e07afe5044d453f34ed2a218f9114/DAY8/3_2%20it's%20showing%20timing%20w.r.t%20MYCLK%20only%20but%20i%20want%20the%20capture%20to%20be%20w.r.t%20MYGEN_CLK%20.png"> <br><br>
--> Modeling for MYGEN_CLK,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7fb9bb75d67e07afe5044d453f34ed2a218f9114/DAY8/3_2%20modeling%20for%20MYGEN_CLK%20.png"> <br><br>
--> lab8_circuit_modified.v,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7fb9bb75d67e07afe5044d453f34ed2a218f9114/DAY8/3_2%20lab8_circuit_modified.png"> <br><br>
--> lab8_cons.tcl script which includes every command so I don't need to give everything explicitly every time,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7fb9bb75d67e07afe5044d453f34ed2a218f9114/DAY8/3_2%20lab8_cons.tcl%20script%20which%20includes%20every%20command%20so%20i%20don't%20need%20to%20give%20everything%20explicitely%20everytime.png"> <br><br>
--> sourcing and linking that script,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7fb9bb75d67e07afe5044d453f34ed2a218f9114/DAY8/3_2%20sourcing%20and%20linking%20that%20script.png"> <br><br>
--> can see, the min and max load for OUT_Y is also modelled because we mentioned that in script,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/12e0826d4fb0e6fb8779970d8a03b0a591103806/DAY8/3_2%20can%20see%2C%20the%20min%20and%20max%20load%20for%20OUT_Y%20is%20also%20modelled%20because%20we%20mentioned%20that%20in%20script.png"> <br><br><br>


--> Input delay:- <br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/1d2b47c540ecd92ba26043ec65e3513c865f1945/DAY8/1.jpg"> <br>
negative delay for max is relaxing and positive delay for max is tightening.<br><br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/1d2b47c540ecd92ba26043ec65e3513c865f1945/DAY8/2.jpg"> <br>
positive delay for min is relaxing and negative delay for min is tightening.<br><br>

--> We need to constraint IO for this combo logic case,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/1d2b47c540ecd92ba26043ec65e3513c865f1945/DAY8/3.jpg"> <br><br>

The command for constraining combo logic is,<br>

```ruby
 set_max_latency 1.0 -from [get_ports IN_C] -to [gte_ports OUT_Z]
 set_max_latency 1.0 -from [get_ports IN_D] -to [gte_ports OUT_Z]
```

--> Another way to constrain that pure combo logic is, By creating something called a Virtual clock(it is just an imaginary clock for budgeting the timing).<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/5c1153af3089d15fdafbfa23bfe8ed0fcc7538c4/DAY8/5.jpg"> <br><br>

 ```ruby
  create_clock -name MY_VCLK -period 5
```

( No clock definition point in command inferred virtual clock.)<br>

```ruby
 set_ouput_delay -max 2.5 -clock MY_VCLK [get_ports OUT_Z]
 set_ouput_delay -max 1.5 -clock MY_VCLK [get_ports IN_C]
 set_ouput_delay -max 1.5 -clock MY_VCLK [get_ports IN_D]
```

Can see in this case also available time for optimization of combo logic is 1ns.<br><br>



--> We need to constraint IO for this case,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3c7bcd41a93476d6a5a6e233f81d9fbf4c27b34e/DAY8/6.jpg"> <br>

```ruby
 set_input_delay -max 2 -clock CLK [get_ports IN_A]  #for FF1 to IN_A
 set_input_delay -max 3 -clock CLK -clock_fall -add [get_ports IN_A]   #for FF2 to IN_A
```

<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3c7bcd41a93476d6a5a6e233f81d9fbf4c27b34e/DAY8/7.jpg"> <br>

```ruby
   set_output_delay -max 2 -clock CLK [get_ports out_y]
   set_output_delay -max 3 -clock CLK -clock_fall -add [get_ports out_y]
```

<br>

--> Lab on the above cases of IO constraints by the design lab14_circuit.v :-<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/1d2b47c540ecd92ba26043ec65e3513c865f1945/DAY8/4.jpg"> <br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7278a544e36f8e685a414cae7a9b6202b3179be6/DAY8/4.2%20lab14_circuit.v.png"> <br><br>
--> It says the path is unconstrained because I haven't yet constrained,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7278a544e36f8e685a414cae7a9b6202b3179be6/DAY8/4.2%20says%20path%20is%20unconstrained%20because%20i%20haven't%20yet%20constrained.png"> <br><br>
--> Some basic commands,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7278a544e36f8e685a414cae7a9b6202b3179be6/DAY8/4.2%20some%20basic%20commands.png"> <br><br>
--> Small script for fanout
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7278a544e36f8e685a414cae7a9b6202b3179be6/DAY8/4.2%20script%20for%20fanout.png"> <br><br>
--> Fanout,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7278a544e36f8e685a414cae7a9b6202b3179be6/DAY8/4.2%20fanout.png"> <br><br>
--> Fanin,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7278a544e36f8e685a414cae7a9b6202b3179be6/DAY8/4_2%20fanin.png"> <br><br>
--> Timing is violated before compile ultra, <br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7278a544e36f8e685a414cae7a9b6202b3179be6/DAY8/4_2%20timing%20is%20violated%20before%20compile%20ultra.png"> <br><br>
--> After compile ultra, we can see our timing is met because it is optimized in such a way that there won't be any violations,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7278a544e36f8e685a414cae7a9b6202b3179be6/DAY8/4_2%20after%20compile%20ultra%20timing%20is%20met.png"> <br><br>

--> After writing out in ddc format, we are going to design vision and read that ddc file to see the schematic,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/5444e1f81e8bb5a26acc4500d050549d2228665f/DAY8/4_2%20schematic.png"> <br><br>




--> Constraining the same design in another way, which is by the virtual clock,<br>
--> Creating the virtual clock,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e3d9a883c055d4ab4d348bc93639f31a1440acb5/DAY8/4_3%20virtual%20clock.png"> <br>
--> constraining for virtual clock,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e3d9a883c055d4ab4d348bc93639f31a1440acb5/DAY8/4_3%20constraining%20for%20virtual%20clock.png"> <br>
--> In the report one path is violated, but after compiling ultra that path won't be violated anymore Basically that path has met.

</details>  




## DAY-9 Optimizations

<details>
	<summary> Introduction </summary> <br>


--> VLSI design optimization is vital for efficient integrated circuits. It enhances power efficiency, space usage, timing precision, and manufacturability, ensuring high-performance ICs.<br>
 <br>
 
 **--> Optimization goals:-** <br><br>

**Cost-Based Optimization:** Striving for an optimal balance between performance and cost, ensuring that cost constraints are met without overemphasizing a single goal, which can compromise others.<br><br>

**Performance Optimization:** <br>

- Speed: Enhancing operational speed by minimizing delays, optimizing critical paths, and ensuring compliance with specified timing requirements.<br>

- Throughput: Elevating system throughput through efficient data flow optimization and the elimination of circuit bottlenecks.<br><br>

**Power Optimization:** <br>

- Dynamic Power: Minimizing dynamic power consumption to extend battery life in portable devices and reduce power dissipation in data centers.<br>

- Static Power: Reducing static power (leakage power) to lower overall power consumption during standby or idle IC states.<br><br>

**Synthesis Goals:** <br>

- Meet Timing: Ensuring that the IC design adheres to specified timing constraints.<br>

- Meet Area: Optimizing the utilization of the physical chip area.<br>

- Meet Power: Achieving power efficiency targets within the design.<br><br>
</details>



<details> 
<summary>Combinational Logic optimization </summary> 
	
- It squeezes the logic to get the most optimized design in terms of area and power. There are various techniques for optimizing the circuit.<br>
- The goal of combinational logic optimization is to reduce various metrics such as propagation delay, power consumption, and area occupation while maintaining the functionality of the circuit.<br><br>
	
**--> Common techniques used for combinational logic optimization are:-** <br>

*-> Constant propagation,* <br>
  It's a direct optimization technique. It identifies and removes redundant logic expressions that appear in multiple places within the circuit.<br>
Example,<br>
	 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/1fb31a2873013a2d80d629724f9a578444e30aab/day9/IMG_20230914_233024.jpg"> <br>
  So, we are saving power and area by boolean logic optimization.<br><br>

*-> Boolean logic optimization,* <br>
 This involves using Boolean algebra rules and laws to simplify logical expressions. Karnaugh maps and Quine-McCluskey methods can be used to find the minimal representation of logic functions.<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/063215b65d21844fcaa75543ea55c6a2536542a1/day9/IMG_20230914_232955.jpg"> <br><br>

*-> Resource sharing,* <br>
Resource sharing optimization in digital design minimizes redundancy, efficiently utilizing resources like logic gates to enhance performance and reduce area.<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/063215b65d21844fcaa75543ea55c6a2536542a1/day9/IMG_20230914_232941.jpg"> <br>
 we know that compared to mux multiplier is going to take a huge area. so this design is optimized for area and power,<br><br>

*-> Logic sharing,* <br>
Logic-sharing optimization in digital design minimizes duplications, improving resource utilization by consolidating common logic elements to enhance performance and efficiency.<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d3df29e372a69ac91e2a55dc18d97176550fbc67/day9/IMG_20230914_232921.jpg"> <br>
 Here, we can say the optimized one will take less area and power.<br><br>

*-> Balanced vs preferential implementation,* <br>
Consider the below equation<br>

y = a & b & c & d & e <br>

It can be implemented in two ways based on the constraints, as shown in the figure,
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7b51061434854ff8c936c43222cded8e4697ff06/day9/C5.jpg"> <br>

 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7b51061434854ff8c936c43222cded8e4697ff06/day9/C6.jpg"> <br>
 Now, the DC will select that totally depends on the delay acceptable from any input to output, how much delay is acceptable. so which implementation is to pick, all this are decided by constraints.<br><br>
	
	
</details>



<details>
	<summary> Sequential logic optimization </summary> 
	Sequential logic optimization is the process of improving the performance, efficiency, and other characteristics of digital circuits that contain memory elements such as flip-flops, latches, and registers. <br>
	The goal of sequential logic optimization is to enhance various aspects of the design, such as speed, power efficiency, area utilization, and reliability, while ensuring that the functionality of the circuit is preserved. <br> <br>

 **--> common techniques used for sequential logic optimization are:-** <br>

 *-> Sequential constant propagation,* <br>
 Sequential Constant Propagation (SCP) is an optimization technique used in compiler design to improve the efficiency of code execution by replacing variables with their constant values wherever possible.<br>
 Examples,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b95bd568836096dac2b79ae3bc2bc72c3197dc70/day9/S1.jpg"> <br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b95bd568836096dac2b79ae3bc2bc72c3197dc70/day9/S2.jpg"> <br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b95bd568836096dac2b79ae3bc2bc72c3197dc70/day9/S3.jpg"> <br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b95bd568836096dac2b79ae3bc2bc72c3197dc70/day9/S4.jpg"> <br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b95bd568836096dac2b79ae3bc2bc72c3197dc70/day9/S5.jpg"> <br>
<br>


*-> Optimization of unloaded outputs,* <br>
  Optimizing unused outputs in a sequential process typically involves improving the efficiency or effectiveness of a system by optimizing the outputs that are not directly used or observed in the process.<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b95bd568836096dac2b79ae3bc2bc72c3197dc70/day9/S6.jpg"> <br>
  Can see the output which are not at all getting used, need not be kept,it can be knocked out.<br><br>


   **--> Controlling sequential optimization in DC:-** <br>

   --> For propagating sequential constant, <br>
   
   ```ruby
    compile_seqmap_propagate_constants
   ```

  If we set it true then only it will propagate sequential constant else it will not.<br>
<br>

  --> For deleting unloaded output cells, <br>
   
   ```ruby
    compile_delete_unloaded_sequential_cells
   ```

  If we set it true then only it will delete unloaded output cells. else it will not delete. <br> <br>
<br>

 --> For cloning registers, <br>
   
   ```ruby
    compile_register_replication
   ```

 It can basically create replica or copy of flop to decrease the routing delay and meet the timing. <br><br>
<br>

    
</details>
         



<details>
	<summary> Lab for combinational logic optimization</summary> 
        Examples,<br>

 1.opt_check<br>
	
--> Verilog code for design,<br>

```ruby
module opt_check (input a , input b , input c , output y1, output y2);
wire a1;
assign y1 = a?b:0;
assign y2 = ~((a1 & b) | c);
assign a1 = 1'b0;
endmodule
```
        

 --> expecting optimization result,<br>
       
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/36a1a2713db3a595192575c71c0ec67142d77638/day9/LC1.jpg"> <br><br>


 --> Can see the below timing report, which is showing the path is unconstrained because we haven't yet constrained,<br>
     
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/36a1a2713db3a595192575c71c0ec67142d77638/day9/1_read_timing.png"> <br><br>

 --> Now, we can see timing is met after compilation,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/36a1a2713db3a595192575c71c0ec67142d77638/day9/2_timing_aftercompile.png"> <br><br>


 --> Can see the schematic it has optimized our design as we expected,<br>
    
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/4_GUI.png"> <br><br>



2.opt_check2<br>
   
 --> Verilog code for design,<br>
  
```ruby
module opt_check2 (input a , input b , output y);
assign y = a?1:b;
endmodule
```
	
     

 --> expecting optimization result,<br>
       
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/36a1a2713db3a595192575c71c0ec67142d77638/day9/LC2.jpg"> <br><br>



--> Now, we can see timing is met after compilation,<br>
     
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/36a1a2713db3a595192575c71c0ec67142d77638/day9/9_optcheck4_timinng_post_compile.png"> <br><br>

--> Can see the schematic it has optimized our design as we expected,<br>
    
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/6_GUI.png"> <br><br>



 3.opt_check3<br>
 
 --> Verilog code for design,<br>


 ```ruby
 module opt_check3 (input a , input b, input c , output y);
 assign y = a?(c?b:0):0;
 endmodule
 ```

 
      
	
--> expecting optimization result,<br>
       
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/LC3.jpg"> <br><br>


--> Now, we can see timing is met after compilation,<br>
     
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/7_optcheck3_timinng_post_compile.png"> <br><br>

--> Can see the schematic it has optimized our design as we expected,<br>
    
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/8_GUI.png"> <br><br.>



 
4.opt_check4 <br>
 
 --> Verilog code for design,<br>


 ```ruby
 module opt_check4 (input a , input b , input c , output y);
 assign y = a?(b?(a & c ):c):(!c);
 endmodule
 ```
	
	
      

--> The below is the timing report,<br>
 
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/9_optcheck4_timinng_post_compile.png"> <br>
we can see it's taking 80ps from A to Y (WITH XNOR)<br> <br>

--> Constraining the path,<br>

 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/10_set_delay_timing_violate.png"> <br><br>
--> Constraining the path,<br>

 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/10_set_delay_timing_violate.png"> <br><br>

--> Timing report after constraining path,<br>
 
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/11_change_xnor_timing_violate_up.png"> <br>
  can see till there is vilation in path, to solve that we will do compile_ultra.<br><br>

--> Timing report aftering compiling ultra,<br>
  
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/12_timing_after_compile.png"> <br><br>
  now we can see vilations are solved. <br><br>

  
--> Can see the schematic ,<br>
    
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/13_GUI.png"> <br><br>


5. Resource sharing optimization,<br>
 
--> The verilog code for the design we will use is,<br>


```ruby
 module_resource_sharing_mult_check (input [3:0] a,b,c,d,output [7:0]y, input sel);
 assign y=sel?(a*b) :(c*d);
 endmodule
 ```
    
  
    
--> Expecting optimization,<br>

 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/IMG_20230914_232941.jpg"> <br><br>

 
-->  After reading file and compiling ultra write it out in ddc format and then seeing it's schematic in design vision,<br>

 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/15_GUI.png"> <br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/16_GUI_mux.png"> <br>
 
 can see mux is at the back side. <br><br>
 
 
--> Below is the area report of the design without giving constrains,<br>

  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/17_report_area.png"> <br><br>


--> Timing report without giving constraints,<br>

 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/18_timing_pastcompile.png"> <br><br>


--> constraining my design,<br>

 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/19_set_delay_timing_violate.png"> <br><br>


--> Timing report after optimizing design,<br>
 
   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/20_timing_post_compile.png"> <br><br>


--> Area report after constraining from input to ouput paths,<br>

   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/21_area_report_2.png"> <br><br>

--> Area report for sel to out y constrained,<br>

   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/25_area_report_3.png"> <br>
   Can see, and we can compare are with previous case it's almost 3 timesarea so we can say to met the constraint now it has used two multiplier instead one.<br><br>


--> Same thing can also be noticed in schematic,<br>

 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/24_GUI.png"> <br><br>

 --> Now we will constraint that max area can't be larger than 800. can see timing report for that,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/26_timing_report_postareaconstraint.png"> <br><br>



--> Area report for this case,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2c91064365dcce6b04754499e0f3dd285dcf2f30/day9/27_area_report4.png"> <br>
 Can see it has optimized it based on constraints.<br><br>

</details>



<details> 
<summary> Lab for sequential logic optimization </summary> 
	
Examples,<br>

1. dff_const1,<br>

--> verilog code for the design,<br>

  ```ruby
    module dff_const1(input clk, input reset, output reg q);
always @(posedge clk, posedge reset)
begin
	if(reset)
		q <= 1'b0;
	else
		q <= 1'b1;
end

endmodule
```

<br>

--> Expecting after optimization,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/LS1.jpg"> <br><br>

--> cells of design,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/28_seq_dff_const1_cells.png"> <br><br>

-->schematic for design,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/29_dff_c1_GUI.png"> <br><br>




2. dff_const2,<br>

--> verilog code for the design,<br>

  ```ruby
   module dff_const2(input clk, input reset, output reg q);
always @(posedge clk, posedge reset)
begin
	if(reset)
		q <= 1'b1;
	else
		q <= 1'b1;
end

endmodule
```

<br>

--> Expecting after optimization,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/LS2.jpg"> <br><br>

--> schematic after optimization,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/29_dff_c1_GUI.png"> <br><br>

--> now if we don't want to do optimization then by setting seuential propagation constant as false we can prevent it from optimization, can see in below schematic,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/30_dff_c2_GUI.png"> <br><br>




3. dff_const3,<br>

--> verilog code for the design,<br>

  ```ruby
 module dff_const3(input clk, input reset, output reg q);
 reg q1;

 always @(posedge clk, posedge reset)
 begin
	if(reset)
	begin
		q <= 1'b1;
		q1 <= 1'b0;
	end
	else
	begin
		q1 <= 1'b1;
		q <= q1;
	end
 end

 endmodule
```

<br>

--> Expecting after optimization,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/LS3.jpg"> <br><br>

--> schematic for the design,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/33_dff_c3_GUI.png"> <br><br>




4. dff_const4,<br>

--> verilog code for the design,<br>

  ```ruby
  module dff_const4(input clk, input reset, output reg q);
reg q1;

always @(posedge clk, posedge reset)
begin
	if(reset)
	begin
		q <= 1'b1;
		q1 <= 1'b1;
	end
	else
	begin
		q1 <= 1'b1;
		q <= q1;
	end
end
endmodule
```

<br>

--> Expecting after optimization,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/LS4.jpg"> <br><br>

--> restricting optimization,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/32_dff_c2_restrict_optimisation.png"> <br><br>
 
--> schematic for restricting optimization,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/34_dff_c5_GUI_constrained.png"> <br>
 i have set the constraints as false so that variables will retain in tool memory so it's not removing that flop.<br><br>

--> schematic for optimized one,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/85d2d0620a81670a50fe1d6818dd2cc7930fdeea/day9/34_dff_c4_GUI_unconstrained.png"> <br><br>

</details>





<details>
	<summary>Special optimizations</summary>


 **Register retiming optimization**
  Register retiming is a technique used to optimize the performance of digital circuits by arranging the registers in circuit without chnaging it's functionality.<br>
  The primary goal of register retiming is to minimize the critical path delay, which is the longest parth in the circuit from input to an output.<br>
  
   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/SO_RR_1.jpg"> <br>
   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/SO_RR_2.jpg"> <br>
   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/SO_RR_2.jpg"> <br>
   Basically DC is doing here best possible split. and this is called register retiming.<br>
   the disadvantage of register retiming is we won't be able to understand the value coming t intermediate stage but if we won't do register retiming then we will get sub-optimal logic. SO, be very careful in selecting when to use register retiming and when to not.<br><br>

   *-->Lab example on register retiming*

   --> verilog code for the design,<br>

   ```ruby
  module check_reg_retime (input clk , input [3:0] a, input [3:0] b , output [7:0] c , input reset);

wire [7:0] mult;
assign mult = a * b;
reg [7:0] q1;
reg [7:0] q2;
reg [7:0] q3;




always @ (posedge clk , posedge reset)
begin
	if(reset)
	begin
		q1 <= 8'b0;
		q2 <= 8'b0;
		q3 <= 8'b0;
	end
	else
	begin
		q1 <= mult;
		q2 <= q1;
		q3 <= q2;
	end
end
assign c = q3;

endmodule
 ```
   
  --> view,<br>
   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/SO_RR_L_1.jpg"> <br><br>

  --> Timing report,<br>
   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/44_retime_timing_pastclock.png"> <br><br>

  --> Constraining design for timing,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/45_retime_clocks.png"> <br><br>


--> timing report after constraining design,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/46_retime_timig_report.png"> <br><br>

--> timing report after compiling ultra,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/49_retime_timing_report_input_post_compile.png"> <br><br><br>



**Boundary optimization**

It refers typically to optimizing boundary7 of a digital design for improvement of power, performance and area.<br>

<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/SO_BO_1.jpg"> <br>
the DC may dissolve this boundary to optimize it.so after synthesizing it there will not be hierarchy call sub module in the netlist.<br>

The advantage of boundry optimization is, i will get optimal logic.but there is one drawback too, that this may going to create a problem for us in terms of functional design-verification. <br><br>

So, for preventing from optimization,<br>

```ruby
  set_boundary_optimization <design> <true/false>
```

*-> Lab for boundary optimization*
Example,<br>
check_boundary,<br>

--> verilog code for design,<br>

```ruby
module check_boundary (input clk , input res , input [3:0] val_in , output reg [3:0] val_out);
wire en;
internal_module u_im (.clk(clk) , .res(res) , .cnt_roll(en));

always @ (posedge clk , posedge res)
begin
	if(res)
		val_out <= 4'b0;
	else if(en)
		val_out <= val_in;	
end
endmodule


module internal_module (input clk , input res , output cnt_roll);
reg [2:0] cnt;

always @(posedge clk , posedge res)
begin
	if(res)
		cnt <= 3'b0;
	else
		cnt <= cnt + 1;
end

assign cnt_roll = (cnt == 3'b111);

endmodule
```
<br><br>



--> view of our design,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/SO_BO_L_1.jpg"> <br><br>

--> cells of the design,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/37_boundary_cell_nohier.png"> <br><br>

--> GUI with no hierarchy,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/38_boundary_GUI_nohier.png"> <br><br>


--> preventing from optimization ,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/41_boundary_GUI_withhier.png"> <br><br>

--> GUI with hierarchy
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/41_boundary_GUI_withhier.png"> <br><br><br>




**Isolating output ports**
Isolating output ports is very important in some cases because exteranal load variations may affect out internal paths and due to that there may be a possiblity also that internal paths may get fail so to prevent internal paths from getting fail we isolate the output port via buffer. so there won't be any affect on internal paths.<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/SO_isolating_output_port_1.jpg"> <br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/b38747db50d9cc29f08293a82bb0d61b46a17734/day9/SO_isolating_output_port_2.jpg"> <br><br>


*Lab on isolating output ports* <br>
Example,<br>
 
--> verilog code for design,<br>

```ruby
module check_boundary (input clk , input res , input [3:0] val_in , output reg [3:0] val_out);
wire en;
internal_module u_im (.clk(clk) , .res(res) , .cnt_roll(en));

always @ (posedge clk , posedge res)
begin
	if(res)
		val_out <= 4'b0;
	else if(en)
		val_out <= val_in;	
end
endmodule


module internal_module (input clk , input res , output cnt_roll);
reg [2:0] cnt;

always @(posedge clk , posedge res)
begin
	if(res)
		cnt <= 3'b0;
	else
		cnt <= cnt + 1;
end

assign cnt_roll = (cnt == 3'b111);

endmodule
```
<br><br>
--> schamatic before isolating the output port,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/52_isolate_GUI_without_isolate.png"> <br><br>
--> Timing report before isolating the output port,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/54_isolate_timing_report_past_isolate.png"> <br><br>
--> Timing report after isolating the ouput port,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/58_isolate_timing_report_post_isolate.png"> <br><br>
--> Can see in schematic also,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/60_isolate_GUI_post_isolate.png"> <br><br>




**Multi-cycle paths**

--> Muticycle paths are encountered in digital designs when specific timing requirement or constrains permit longer propagation delays.<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/SO_MSP.jpg"> <br><br>


*Lab on multi-cycle paths*
Example,<br>
--> verilog code for design,<br>

```ruby
module check_boundary (input clk , input res , input [3:0] val_in , output reg [3:0] val_out);
wire en;
internal_module u_im (.clk(clk) , .res(res) , .cnt_roll(en));

always @ (posedge clk , posedge res)
begin
	if(res)
		val_out <= 4'b0;
	else if(en)
		val_out <= val_in;	
end
endmodule


module internal_module (input clk , input res , output cnt_roll);
reg [2:0] cnt;

always @(posedge clk , posedge res)
begin
	if(res)
		cnt <= 3'b0;
	else
		cnt <= cnt + 1;
end

assign cnt_roll = (cnt == 3'b111);

endmodule
```
<br><br>

--> compiling the design,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/61_mcp_compile_link_compile.png"> <br><br>
-->sourcing the script,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/62_mcp_source_timing_report.png"> <br><br>
-->timing report after optimizing design,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/64_timing_report_post_-compile.png"> <br><br>
-->setting up multicycle path,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/65_setmcp_timing_report_post_-compile.png"> <br><br>
-->timing report after setting up ,multicycle path,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/65_setmcp_timing_report_post_-compile.png"> <br><br>
--> hold timing report,<br><br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/73_timing_delay_min_from_inputs.png"> <br><br>
-->timing reports to pro_reg[*]/D from all_inputs,
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/73_timing_delay_min_from_inputs.png"> <br><br>
--> timing report after isolating the output,
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/76_timing_report_last.png"> <br><br>


**False paths**

<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/SO_FP_1.jpg"> <br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/df3177e8a85ab0cfba6237b5ff0dccf47c97311e/day9/SO_FP_2.jpg"> <br>
Basically if there will be no relation between two clock then that will be declared as false path.

</details>




## DAY-10 QOR

<details>
	<summary> Intoduction to propagation delay and concepts associated with it</summary>
	 Propagation delay refers to the time it takes for a signal to travel from the input of a logic gate or circuit to its output, after accounting for various delays within the circuit. <br>
	Let's take example of below CMOS inverter gate to understand it in more details,<br>
	<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8d6d09ac00282153a53f3b73f34db50b57857511/1.jpg"> <br>
        Is A rise to Y fall and A fall to Y rise delay are same ? <br>
	No. <br>
        Because, Rise-to-fall and fall-to-rise propagation delays differ due to the intrinsic characteristics of NMOS and PMOS transistors. NMOS transistors switch faster during falling transitions due to higher electron mobility, while PMOS transistors have faster rising transitions due to lower hole mobility, creating an inherent asymmetry in CMOS circuitry. <br>
	Basically for any circuit, all the different inputs are going to give us different timing arc combinations. <br><br><br>
 

 **--> Timing paths** <br>
*--> Let's understand the timing paths by one example,* <br> 
       <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8d6d09ac00282153a53f3b73f34db50b57857511/2.jpg"> <br> <br>

       
  1. DFFA(clk-Qr) -> INV(Ar) -> INV(Yf) -> AND (Af) -> AND (Yf) -> DFFC(f) <br>

  -> The above " Max delay from DFFA to C " path is having 1.65ns delay. <br><br>

  2. DFFA(clk-Qf) -> INV(Af) -> INV(Yr) -> AND (Ar) -> AND (Yr) -> DFFC(r) <br>

  -> The above " Min delay from DFFA to C " path is having 1.5ns delay. <br><br>

  3. DFFB(clk-Qr) -> AND (Br) -> AND (Yr) -> DFFC(r) <br>

  -> The above " Max delay from DFFB to C " path is having 1.15ns delay. <br><br>

  4. DFFB(clk-Qf) -> AND (Bf) -> AND (Yf) -> DFFC(f) <br>

  -> The above " Min delay from DFFB to C " path is having 1.0ns delay. <br><br><br>


*--> Now let's understand, For a particular command which path tool will report out of above,* <br><br>

   - report_timing -from DFFA/clk -to DFFC/D -delay_max  <br>
   -> This will report path number 1 which is "Max delay from DFFA to C". <br><br>

   - report_timing -from DFFA/clk -to DFFC/D -delay_min  <br>
   -> This will report path number 2 which is "Min delay from DFFA to C". <br><br>

   - report_timing -delay min -to DFFC/D  <br>
   -> This will report path number 4 which is "Min delay from DFFB to C". <br><br>

   - report_timing -delay max -to DFFC/D  <br>
   -> This will report path number 1 which is "Max delay from DFFA to C". <br><br>

   - report_timing -delay_type max -rise_to DFF_C/D  // basically, it says what is the maximum rise delay to DFF C. <br>
   -> This will report path number 2 which is "Min delay from DFFA to C". <br><br>

   - report_timing -delay_type max -fall_to DFF_C/D  // basically, it says what is the maximum fall delay to DFF C. <br>
   -> This will report path number 1 which is "Max delay from DFFA to C". <br><br>

   - report_timing -delay_type min -rise_to DFF_C/D  // basically, it says what is the minimum rise delay to DFF C. <br>
   -> This will report path number 3 which is "Max delay from DFFB to C". <br><br>

   - report_timing -delay_type min -fall_to DFF_C/D  // basically, it says what is the minimum fall delay to DFF C. <br>
   -> This will report path number 4 which is "Min delay from DFFB to C". <br><br><br>


*--> Continuing the same example by considering that clock period be 5ns,*  <br>   
   
   - report_timing -delay_type max -to DFF_c/D <br>
   -> This will report path number 1 which is "Max delay from DFFA to C". which has 1.65ns arrival time.<br><br>

     Clock period = 5ns , setup of DFFC = 0.5ns <br>
     Data at DFFC needs to be stable by = 5-0.5 => 4.5ns (Required time) <br>
     Setup check = Required time - Arrival time <br>
                 = 4.5ns - 1.65ns <br>
                 = 2.85ns <br> <br>
     
   - report_timing -delay_type min -to DFF_c/D <br>
   -> This will report path number 4 which is "Min delay from DFFB to C". which has 1.0ns arrival time.<br><br>

     Hold of DFFC => 0.1ns (Required time) <br>
     Setup check = Arrival time - Required time <br>
                 = 1.0ns - 0.1ns <br>
                 = 0.9ns <br> <br>
     


   **--> Max_paths and nworst** <br>
   - Let's take one example to understand above two terms, <br>
   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8d6d09ac00282153a53f3b73f34db50b57857511/3.jpg"> <br>

   - Now when i say just simply "report_timing" the worse failing path or worst slack path will get reported. in this example that path is, the path with -1.2ns slack. <br><br>
   
   - report_timing -max_paths2 ,<br>
     Basically max_paths means maximum this much path we can select for worst. Per end point it will pick one worst path. Because by default nwrost option is 1. For this example it will select path having slack of -1.0ns and path having of -1.2ns <br><br>

   - report_timing -max_paths2 -nworst2,<br>
     Basically, nworst suggest how many maximum worst path per end point it can select. For this example it will pick path with slack -1.2ns and -1.1ns. <br><br>

   
</details>




<details> 
<summary> Lab on timing report </summary> <br>

 *--> Let's first understand, what are the ways to identify whether it's setup check report or hold check report,* <br>
 
   --> The verilog code of design,<br>
   ```ruby
   
module lab8_circuit (input rst, input clk , input IN_A , input IN_B , output OUT_Y , output out_clk , output reg out_div_clk);
reg REGA , REGB , REGC ; 

always @ (posedge clk , posedge rst)
begin
	if(rst)
	begin
		REGA <= 1'b0;
		REGB <= 1'b0;
		REGC <= 1'b0;
		out_div_clk <= 1'b0;
	end
	else
	begin
		REGA <= IN_A | IN_B;
		REGB <= IN_A ^ IN_B;
		REGC <= !(REGA & REGB);
		out_div_clk <= ~out_div_clk; 
	end
end

assign OUT_Y = ~REGC;

assign out_clk = clk;

endmodule
   ```
   --> Constraint tcl file,<br>
   
```ruby
create_clock -name MYCLK -per 10 [get_ports clk];

set_clock_latency -source 2 [get_clocks MYCLK];
set_clock_latency 1 [get_clocks MYCLK];
set_clock_uncertainty -setup 0.5 [get_clocks MYCLK];
set_clock_uncertainty -hold 0.1 [get_clocks MYCLK];

set_input_delay -max 4 -clock [get_clocks MYCLK] [get_ports IN_A];
set_input_delay -max 4 -clock [get_clocks MYCLK] [get_ports IN_B];
set_input_delay -min 1 -clock [get_clocks MYCLK] [get_ports IN_A];
set_input_delay -min 1 -clock [get_clocks MYCLK] [get_ports IN_B];

set_input_transition -max 0.4 [get_ports IN_A];
set_input_transition -max 0.4 [get_ports IN_B];
set_input_transition -min 0.1 [get_ports IN_A];
set_input_transition -min 0.1 [get_ports IN_B];

create_generated_clock -name MYGEN_CLK -master MYCLK -source [get_ports clk] -div 1 [get_ports out_clk];
create_generated_clock -name MYGEN_DIV_CLK -master MYCLK -source [get_ports clk] -div 2 [get_ports out_div_clk]; 

set_output_delay -max 4 -clock [get_clocks MYGEN_CLK] [get_ports OUT_Y];
set_output_delay -min 1 -clock [get_clocks MYGEN_CLK] [get_ports OUT_Y];

set_load -max 0.4 [get_ports OUT_Y];
set_load -min 0.1 [get_ports OUT_Y];
```


   --> timing report (t1),<br>
   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/1.%20t1.rpt%20.png"> <br>
     Clues to identify which check it is, are by path type or by launch and edge and capture edge timing difference or by setup time or hold time which one is written in the report, or by whether there is "data required -data arrival" or "data arrival - data required". So, by any on of these clue we can identify whether it's setup check report or it's hold check report. <br><br><br>


*--> To observe, how slack and other delay and all are varying for input fall transition and input rise transition,* <br>

  --> timing report "-from IN_A" (t1),<br>
     <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/2.%20t1.rpt_from%20IN_A%20.png"> <br><br>
  --> timing report "-from IN_A" (t1) Vs timing report "-rise_from IN_A" (t2),<br>
     <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/3.%20t1.rpt%20vs%20t2.rpt_rise_from%20IN_A%20.png"> <br>
      Since, the t1 and t2 report both are not ending at the same point so we can't make a pure comparison. <br><br>

  --> timing report "-from IN_A" (t1) Vs timing report "-rise_from IN_A -to REGA_reg/D" (t3), <br>
    <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/4.%20t1.rpt%20vs%20t3.rpt%20.png"> <br>
     we have generated this t3 timing report because the t1 report is ending at REGA_reg/D pin so to compare purely in t3 report we have set end point same as t1 report. we can clearly observe that how slack and other delays of cells in path and all are changing for the input A rise and input A fall transitions. <br><br><br>
     
  
  --> As i mentioned the clues earlier from that we can say this report is for hold chcek, <br>
   <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/5.%20can%20say%20it's%20for%20hold%20check.png"> <br><br>

  --> To see what is the contribution of this particular U15/Y cell in max path,<br>
    <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/6.png"> <br>
   in max path this particular cell delay can be minimum also because what matters is overall delay of path.<br><br>

   --> To see what is the contribution of this particular U15/Y cell in min path,<br>
    <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/7.for%20min%20.png"> <br>
   simillary here also, in min path this particular cell delay can be maximum also because what matters is overall delay of path.<br><br>
	
</details>



<details>
 <summary> Lab on checking design for HFN and transition </summary> 
	
--> we will check about whether my design is correctly loaded into DC or am i missing something in constraints or something, so is there any utility available in the tool to check whether we loaded the design is constraints correctly all these things we will see. <br>
--> verilog code for the design, <br>
	
  
```ruby
   
module lab8_circuit (input rst, input clk , input IN_A , input IN_B , output OUT_Y , output out_clk , output reg out_div_clk);
reg REGA , REGB , REGC ; 

always @ (posedge clk , posedge rst)
begin
	if(rst)
	begin
		REGA <= 1'b0;
		REGB <= 1'b0;
		REGC <= 1'b0;
		out_div_clk <= 1'b0;
	end
	else
	begin
		REGA <= IN_A | IN_B;
		REGB <= IN_A ^ IN_B;
		REGC <= !(REGA & REGB);
		out_div_clk <= ~out_div_clk; 
	end
end

assign OUT_Y = ~REGC;

assign out_clk = clk;

endmodule
```
--> check_design, <br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/9.%20check_design.png"> <br><br>
--> checking timing,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/10.%20check_timing.png"> <br>
 it's going to check whether my design is proper or not , my design is constrained properly or not. <br><br>

 --> reporting constraints, <br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/11.%20reporting%20constraints%20.png"> <br>
 If we don't source any constraints then defaults constraints which are there in the tool memory that will be loaded.<br><br>

 --> checking timing after sourcing my constraints,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/13.%20check%20timing%20.png"> <br>
  it showing that out_clk and out_div_clk are not constrained but that is fine because i can't constrained clock with anything.<br><br>

--> reporting constraints after sourcing my constraints,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/14.%20reporting%20constraints.png"> <br>
  since we have sourced our constraints so it's not showing default constraints.<br><br>


**--> Lab on high fanout net(HFN) examples,** <br>

-->  Verilog code for design(mux_generate_128_1.v),<br>
```ruby
 module mux_generate (input [127:0]i , input [6:0] sel  , output reg y);
integer k;
always @ (*)
begin
for(k = 0; k < 128; k=k+1) begin
	if(k == sel)
		y = i[k];
end
end
endmodule
```

--> reading verilog file,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/15.%20reading%20%20verilog%20file.png"> <br>
 it's interpriting as latch but when you synthesized it, there won.t be any latch.<br><br>
--> check_design, <br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/16.%20check_design.png"> <br><br>
--> viewing generated netlist,<br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/17.%20can%20see%20all%20the%20cells%20are%20combinational.png"> <br>
 Can see all are combinational cells here there is no any sequential cells.<br><br>

 --> To see wethere there is sequential cells or not,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/18.%20filtering%20sequential%20cells.png"> <br>
  It won't show any cells because there is not any sequential cell.<br><br>
 --> To see whether there is any combinational cells or not,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/19.%20filtering%20combinational%20cells.png"> <br><br>
 --> timing report to see capacitance,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/20.%20report%20timing%20for%20cap.%20png"> <br>
    can see there is so much of fanout so very large capacitance.<br><br>
 --> checking timing,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/21.%20check_timing.%20png"> <br><br>
    can see the end points is not constrained.<br><br>
 --> setting the maximum delay from all inputs to all outputs,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/22.%20setting%20%20max%20delay.%20png"> <br><br>
 --> seeting maximum capacitance for our design,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/23.%20setting%20%20max%20capacitance.%20png"> <br><br>
 --> Below command is to check all violating constraints,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/24.%20reporting%20for%20all%20violations.%20png"> <br>
     we can see path is violating for timing and many nets are violating for capacitance. and we havne't yet modelled any leakage power so by default DC will target default leakage power which is in DC tool memory, that's here saying slack violation for power.<br><br>
 --> after compiling ultra, check_timing,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/25.%20checking%20timing%20after%20seeting%20max%20delay%20and%20max%20capacitance.%20png"> <br>
  Now we can unconstrained end points are not coming because i have set max delay.<br><br>
 --> reporting constraints,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/26.%20reporting%20constraints.%20png"> <br>
  Can see now, max capacitance, max transition, max delay everything has met.<br><br>
  --> reporting for capacitance and nets,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/27.%20reporting%20timing%20after%20setting%20max%20delay%20and%20max%20capacitance.%20png"> <br>
  Can see now, everywhere the max capacitance is less than 0.025, can also see now fanout gets broken and the high fanout nets gets buffered to properly meet that criteria.<br><br><br>
   

 *-->one more lab example on HFN,*
 In below diagram we can see that en will go to 128 pins so load on enable is humungous and so capacitance.<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8d6d09ac00282153a53f3b73f34db50b57857511/4.jpg"> <br><br>
 --> Verilog code for the design "en_128.v",<br>
```ruby
module en_128 (input [127:0] x , output [127:0] y , input en);
	assign y[127:0] = en ?x[127:0]:128'b0;
endmodule
```
<br><br>
 --> report timing,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/28.%20report%20timing%20for%20en_128.%20png"> <br><br>
 --> report timing for capacitance,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/29.%20timing%20report%20for%20cap.%20png"> <br>
   Can see, enable fanout is 128, which is very high, so the capacitance is huge.<br><br>
 --> setting max capacitance limit,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/30.%20setting%20max%20cap.%20png"> <br><br>
 --> reporting constraints,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/31.%20reporting%20constraints.%20png"> <br>
    Capacitance is violating by huge amount because we haven't yet compiled ultra after setting max capacitance,<br><br>
 --> compile ultra,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/32.%20compile%20ultra.%20png"> <br>
    Now the nets will get broken and buffered.<br><br>
 --> report timing for capacitance after optimizing,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/33.%20report%20timing%20for%20cap%20.%20png"> <br>
   Now we can see it has only 17 fanout. earlier it had 128 fanout.<br><br>
 --> writing out ddc file for it,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/34.%20writing%20out%20ddc.%20png"> <br><br>
 --> Can see the schematic,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/35.%20schematic.%20png"> <br><br>
 Can see now, enable is driving only selectively few bits.Basically we are dividing and conquring the problem, so the high fanout net gets split, such that single pin is not having the burden of such a large heavily loaded net.<br><br>
 --> reporting timing,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/36%20timing%20report%20for%20transition.%20png"> <br>
 can see, trans is still bad here. there is something called set_max_transition. <br><br>
 --> setting limit to maximum transition,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/37.%20setting%20max%20transition%20limit.%20png"> <br><br>
 --> reporting constraints,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/37.%20reporting%20constraints.%20png"> <br>
  Can see the transition constraints violated.<br><br>
 --> After compiling ultra reporting constraints,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/39.%20reporting%20constraints%20after%20compile%20ultra.%20png"> <br>
    we can see there is no more violations.<br><br>
 --> reporting timing to see transition values now,<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/40.reporting%20timing%20for%20transition.%20png"> <br>
  we can see, transition is limited to 150ns. now it may have use different kind of buffer to limit the transition time or something.<br><br>
 --> reporting timing from en to y[116],<br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/9662a1b76d7bbf1e6e08913ec50c992825acd708/DAY-10/41.reporting%20timing%20from%20en%20to%20y%5B116%5D.%20png"> <br>
  we can see, transition is only 66ps. it has broken this net and adjusted this net is such a way that transition is not that bad. earlier the data arrival time due to high transition time was 442 ps and but now it has 254 ps. Earlier it was weak buffer so the output transition was very bad and it's strong buffer now(drive strength two) so transition time is less now.
 
</details>


## DAY-11 SOC

<details>
	<summary> Introduction to SoC</summary>
	A System on Chip (SoC) is a compact, integrated electronic circuit that encapsulates multiple essential components of a computer or electronic system onto a single semiconductor chip. It combines a microprocessor or CPU with various peripherals like memory, input/output interfaces, and often specialized hardware for specific functions.<br><br>

SoCs are prevalent in modern electronics, from smartphones and tablets to embedded systems and IoT devices. Their compactness and power efficiency make them ideal for diverse applications. SoC design involves intricate hardware and software integration, ensuring seamless operation and optimized power consumption.<br><br>

SoCs play a crucial role in enabling the proliferation of advanced technologies, offering high-performance computing in a compact form factor while minimizing energy consumption and production costs.<br><br>


</details>



<details>
	<summary> Dimensity 1300 </summary>
 --> The chipset used in Oneplus nord 2T is dimensity 1300. <br><br>
	
**--> CPU Architecture:-** <br>
	The Dimensity 1300’s octa-core CPU features four premium Arm Cortex-A78 processors, including an ‘ultra-core’ operating up to 3GHz. Built using the TSMC N6 (6nm-class) production process, the Dimensity 1300 is an incredibly efficient chip design for extended everyday battery life.<br>
- 1X Ultra Core: Arm Cortex-A78 up to 3GHz <br>
- 3X Super Cores: Arm Cortex-A78 up to 2.6GHz<br>
- 4X Efficiency Cores: Arm Cortex-A55 up to 2GHz<br>
- 9-core Arm Mali <br><br><br>

 **-> Graphics :-** <br>
 - It features a total of 8 high-performing ARM Cortex processors, each capable of reaching a maximum clock speed of 3GHz. Additionally, the chipset is equipped with a robust 9-core ARM Mali-G77 MC9 GPU, which efficiently handles graphics processing and also enhances gaming experiences, and accelerates day-to-day tasks.<br>
 *- GPU Type*<br>
Arm Mali-G77 MC9<br>

 *- Video Encoding*<br>
H.264, H.265 / HEVC<br>

 *- Video Playback*<br>
H.264, H.265 / HEVC, VP-9, AV1<br><br><br>

 **-> Connectivity:-** <br>

*- Cellular Technologies* <br>
2G / 3G / 4G / 5G Multi-Mode, 4G Carrier Aggregation (CA), 5G Carrier Aggregation (CA), CDMA2000 1x/EVDO Rev. A (SRLTE), EDGE, 4G FDD / TDD, 5G FDD / TDD, GSM, TD-SCDMA, WDCDMA<br>

*- Specific Functions* <br>
SA & NSA modes; SA Option2, NSA Option3 / 3a / 3x, NR TDD Band, NR FDD Band, DSS, NR DL 2CC, 200 MHz bandwidth, 4x4 MIMO, 256QAM NR UL 2CC, 2x2 MIMO, 256QAM VoNR / EPS fallback<br>

*- Peak Downlink Speed* <br>
4.7Gbps<br>

*- Peak Uplink Speed*<br>
2.5Gbps<br>

*- GNSS*<br>
GPS L1CA+L5 / BeiDou B1I+ B2a / Glonass L1OF / Galileo E1 + E5a / QZSS L1CA+ L5 / NavIC<br>

*- Wi-Fi Antenna*<br>
2T2R<br>

*- Wi-Fi*<br>
Wi-Fi 6 (a/b/g/n/ac/ax)<br>

*- Bluetooth Version*<br>
5.2<br><br><br>



**--> 5G connectivity:-** <br>
 Built into the chip, the 5G modem offer deeply engrained power saving enhancements, super-fast 5G NR performance and range with mixed-duplex 5G carrier aggregation, and true dual 5G SIM capability. ‘5G Elevator Mode’ & ‘5G HSR Mode’ specialist enhancements ensure seamless 5G experiences with immediate recovery time and reliably faster speeds, respectively.<br>
- MediaTek 5G UltraSave power saving enhancement suite<br>
- 2CC Carrier Aggregation (200MHz) across FDD+TDD<br>
- True dual 5G SIM (5G SA + 5G SA)<br>
- Dual VoNR<br><br><br>

**--> Display :-** <br>
  The Dimensity 1300 supports super-fast refresh rate displays, giving users impressive, zero-lag visuals in gaming, plus notably improved everyday experiences from smoother scrolling of webpages, social streams, and animations in apps.<br><br>
*- Max Display Resolution* <br>
2520 x 1080 <br>

*- Max Refresh Rate*<br>
168Hz <br><br><br>

**--> Camera :-** <br>
New AI-camera enhancements include improved night shot photography and HDR capabilities for great image clarity. ‘Staggered’ 4K HDR video recording uses real-time 3-exposure fusion to provide 40% greater dynamic range versus standard 4K HDR video capture. <br><br>
*-Max Camera ISP* <br>
32MP + 16MP, 200MP <br>

*- Max Video Capture Resolution* <br>
3840 x 2160 <br>

*- Camera Features* <br>
HDR-ISP (3+2) / Video HDR / Video NR / Video Bokeh / Video EIS / AI-Shutter / AI-AE / AI-AF / AI-AWB / AI-NR HDR / AI-HDR / AI-FD <br> <br> <br>

**--> AI Performance :-** <br>
The Dimensity 1300 boosts AI benchmark scores from the six-core APU 3.0 by up to 10%, giving greater capacity for AI tasks. The MediaTek APU 3.0 features an advanced multi-tasking scheduler to maximize performance and efficiency while handling a wide range of simultaneous tasks.<br><br><br>

**--> Memory and storage :-** <br>
*- Memory Type*<br>
LPDDR4x<br>

*- Max Memory Frequency*<br>
4266Mbps<br>

*- Max Memory Size*<br>
16GB<br>

*- Storage Type*<br>
UFS 3.1<br><br><br>

</details>


<details>
	<summary> Semiconductor manufacturing process</summary> <br>
	
**- Design and Layout:** Engineers start by planning how the computer chip will look using special computer programs. They decide where all the tiny parts, like transistors, should go.<br>

**- Mask Creation:** They make precise templates called photomasks that show where the chip's patterns should be. These guides are used during the making process.<br>

**- Wafer Preparation:** A special flat piece of super-clean silicon, like a shiny rock, is used. They put a thin layer on it to protect it.<br>

**- Photolithography:** They shine light through the masks onto the silicon to make the patterns.<br>

**- Etching:** Chemicals are used to remove extra stuff from the silicon, leaving only the desired patterns.<br>

**- Ion Implantation:** Tiny bits are added to the silicon to make it work right.<br>

**- Deposition:** They add more layers of materials like metal or insulation in a careful way.<br>

**- Chemical Mechanical Polishing (CMP):** They make sure everything is even and smooth.<br>

**- Lithography and Etching (Repeated):** They repeat the process to build up all the chip's layers.<br>

**- Annealing:** The chip gets heated up to work perfectly.<br>

**- Testing and Inspection:** They check it many times to make sure it's perfect.<br>

**- Dicing:** They cut it into tiny pieces, and each piece becomes a computer chip!<br>

**- Packaging:** The chips are put in special cases and connected to other things so they can do their jobs.<br>
</details>


## DAY-12 BabySOC Modelling
<details>
	<summary> Introduction</summary>
	
**-->RVMYTH:-**	<br>
It's RISC-V based myth. it pronounced as "risk-five," represents an Instruction Set Architecture (ISA) rooted in the principles of Reduced Instruction Set Computing (RISC). This ISA establishes a fundamental set of instructions known as the core integer ISA, which is a mandatory component in all RISC-V implementations. Moreover, RISC-V incorporates optional extensions to augment its capabilities. The core integer instruction set can be distinguished by various characteristics, including the width of integer registers, the scope of its addressable memory, and the quantity of available integer registers. Notably, RISC-V encompasses two primary core integer variants, denoted as RV32I and RV64I.<br>

*->RV32I:-*
32-Bit Iteration: RV32I corresponds to the 32-bit iteration of the RISC-V architecture. In this variant, the CPU's data and address registers are both 32 bits wide.<br>
Address Capacity: RV32I boasts a 32-bit virtual address space, empowering it to access up to 2^32 distinct memory locations, equivalent to a memory capacity of 4 gigabytes.<br>
Register Bank: RV32I supplies 32 general-purpose registers (often referred to as integer registers) dedicated to executing arithmetic operations and manipulating data.<br>
Instruction Repertoire: This iteration defines a specific set of instructions tailored for 32-bit RISC-V processors, encompassing arithmetic, logic, memory load and store, as well as control flow instructions.<br>

*->RV64I:-*
64-Bit Version: RV64I signifies the 64-bit embodiment of the RISC-V architecture. Within this iteration, both data and address registers expand to 64 bits in width.<br>
Expanded Address Space: RV64I introduces a vastly expanded virtual address space compared to RV32I. It has the capability to address up to 2^64 unique memory locations, an address space of astronomical proportions.<br>
Register Complement: RV64I also furnishes 32 general-purpose registers (integer registers) akin to RV32I. However, these registers are 64 bits wide, permitting more comprehensive data manipulation and accommodating 64-bit data types.<br>
Instruction Set: Similar to RV32I, RV64I lays out a specific set of instructions; nevertheless, these instructions operate on 64-bit data.<br>

In summary, RISC-V serves as an open and versatile ISA adhering to RISC principles. It encompasses both 32-bit (RV32I) and 64-bit (RV64I) core integer variants, each tailored to specific computing needs and offering distinct advantages in terms of addressable memory, register width, and data processing capabilities.<br><br>



**-->PLL(Phase-Locked loop):-** <br>
--> PLL stands for "Phase-Locked Loop," which is an electronic circuit used in various applications to generate or synchronize signals of a specific frequency. A PLL consists of several components, including a voltage-controlled oscillator (VCO), a phase comparator, a feedback loop, and a divider.<br><br>
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/2b5e4a03b0b30f485a094292705935d43a21925d/DAY-12/PLL.jpg"> <br>
*--> Here's a brief overview of how a Phase-Locked Loop works:* <br>

Reference Signal: The PLL takes an input signal called the "reference signal" or "reference clock." This signal represents the desired output frequency that the PLL will attempt to generate or synchronize with.<br>

Phase Comparator: The phase comparator compares the phase of the reference signal with the phase of the output signal generated by the VCO.<br>

Control Voltage: Based on the phase difference between the reference signal and the VCO output, the phase comparator generates a control voltage.<br>

Voltage-Controlled Oscillator (VCO): The VCO is a key component of the PLL. It generates an output signal with a frequency that can be adjusted by varying the control voltage applied to it. When the PLL is locked, the VCO's output frequency matches the desired output frequency.<br>

Feedback Loop: The control voltage from the phase comparator is fed back to the VCO through a filter and amplifier. This feedback loop continuously adjusts the VCO's frequency until it matches the frequency of the reference signal.<br>

Divider (Optional): In some PLL applications, a divider is used to divide the output frequency of the VCO, providing a divided output signal at a lower frequency. This can be useful when precise frequency division is required.<br>

PLLs are used in a wide range of applications, including clock generation, frequency synthesis, data recovery, modulation and demodulation, and clock synchronization in communication systems, digital circuits, and various electronic devices. They are essential for maintaining stable and synchronized signals in many electronic systems.<br><br>



**-->DAC (Digital to analog converter):-** <br>
A Digital-to-Analog Converter (DAC) is an electronic device or circuit that converts digital data (usually in the form of binary numbers) into analog signals, typically voltage or current. It plays a crucial role in many electronic systems, especially in applications where digital data needs to be converted into a continuous, analog signal for various purposes, such as audio playback, video generation, motor control, and more.<br>

*-> Here's how a DAC works,* <br>

Digital Input: The input to a DAC is a digital signal, often represented as a binary number. Each bit in the digital input corresponds to a different "level" or "step" in the analog output.<br>

Conversion Process: The DAC takes the digital input and uses it to determine the appropriate analog output voltage or current. This process involves mapping the digital values to specific analog voltage levels.<br>

Analog Output: The result is an analog output signal that varies continuously based on the digital input. This analog signal can be used to control various physical processes or to generate analog audio or video signals.<br>

*-->There are different types of DACs, including:* <br>

Binary Weighted DAC: In this type, the weight of each bit in the digital input is proportional to its significance. For example, the most significant bit (MSB) might have the largest weight, and each subsequent bit's weight is halved. <br>

R-2R Ladder DAC: This type of DAC uses a ladder network of resistors to convert digital inputs into analog outputs. It's known for its simplicity and linearity. <br>

Delta-Sigma DAC: These are often used in high-precision applications. They use oversampling and noise-shaping techniques to achieve high-resolution conversions. <br>

Flash DAC: Also known as a parallel DAC, it's very fast but can be expensive and power-hungry due to the number of components required. <br>

DACs are used in a wide range of applications, including music players (to convert digital audio data into analog audio signals for speakers or headphones), instrumentation (for measurement and control tasks), communication systems (to modulate signals), and many other areas where the conversion of digital data into analog form is needed. <br><br>


</details>






 <details>
	 <summary> Priority Decoder2_4 </summary>

**--> Verilog code for design,** <br>
```ruby
module priority_decoder_2_4 (en,a,b,y);
input en,a,b;
output reg [3:0]y;

always @(en,a,b)
begin
if(en==0)
begin
if(a==1'b0 & b==1'b0) 
   y=4'b0001;
else if(a==1'b0 & b==1'b1)
  y=4'b0010;
else if(a==1'b1 & b==1'b0)
  y=4'b0100;
else if(a==1'b1 & b==1'b1)
 y=4'b1000;
else y=4'bxxxx;

end 
else
y=4'b1111;
end

endmodule
```

**--> Verilog code for testbench,**
<br>
```ruby
module tb_decoder_2_4;

reg a,b,en;

wire [3:0]y;

priority_decoder_2_4 DUT(en,a,b,y);

initial
begin

en=1; a=1'bx; b=1'bx;
#5 en=0; a=0; b=0;
#5 en=0; a=0; b=1;
#5 en=0; a=1; b=0;
#5 en=0; a=1; b=1;
end

initial
begin
$monitor("en=%b a=%b b=%b y=%b", en,a,b,y);
$dumpfile("tb_decoder_2_4.vcd");
$dumpvars;
#50 $finish;
end


endmodule
```

<br><br>

**--> Simulation result,** <br><br>
<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d4bc04214bce2102aaa4b5fddb3a14cba1be6cbb/DAY-12/GTKWAVE.png"> <br>
 </details>


<details>
	<summary> BabySoC modelling</summary>
	
**--> Simulation result of Myth core module,** <br>
*->Commands to perform simulation,* <br>
```ruby
 iverilog mythcore_test.v tb_mythcore_test.v 
 ./a.out
gtkwave tb_mythcore_test.vcd
```
<br>

<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d4bc04214bce2102aaa4b5fddb3a14cba1be6cbb/DAY-12/GTKWAVE_myth_core.png"> <br><br>
The RVMyth processor generates 10-bit digital output codes.Its core function involves incrementing a 10-bit binary value by 1, while an additional 11th bit serves as a sign flag, directing either increment or decrement operations based on its state, thus facilitating dynamic arithmetic processing.<br><br>

**--> Simulation result of PLL module,** <br>
*->Commands to perform simulation,* <br>
```ruby
iverilog rvmyth_pll.v rvmyth_pll_tb.v avsd_pll_1v8.v pll_tb.v
./a.out
gtkwave test.vcd
```
<br>

<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d4bc04214bce2102aaa4b5fddb3a14cba1be6cbb/DAY-12/2_pll_simulation.png"> <br> <br>


**--> Simulation result of DAC module,** <br>
*->Commands to perform simulation,* <br>
```ruby
iverilog avsddac.v avsddac_tb_test.v
./a.out
gtkwave avsddac_tb_test.vcd
```
<br>

<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d4bc04214bce2102aaa4b5fddb3a14cba1be6cbb/DAY-12/1_dac_simulation.png"> <br> <br>
**--> Simulation result of Interfacing mythcore and PLL module,** <br>
*->Commands to perform simulation,* <br>
```ruby
iverilog rvmyth_pll.v rvmyth_pll_tb.v
./a.out
gtkwave test1.vcd
```
<br>

<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d4bc04214bce2102aaa4b5fddb3a14cba1be6cbb/DAY-12/4_pll_rvmyth.png"> <br> <br>
**--> Simulation result of Interfacing mythcore and DAC module,** <br>
*->Commands to perform simulation,* <br>
```ruby
iverilog rvmyth_avsddac.v rvmyth_avsddac_TB.v
./a.out
gtkwave rvmyth_avsddac.vcd
```
<br>

<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d4bc04214bce2102aaa4b5fddb3a14cba1be6cbb/DAY-12/3_dac_rvmyth.png"> <br> <br>
**--> Simulation result of Main core module,** <br>
*->Commands to perform simulation,* <br>
```ruby
iverilog vsdbabysoc.v testbench.v avsdpll.v avsddac.v mythcore_test.v
./a.out
gtkwave dump.vcd
```
<br>

<img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/d4bc04214bce2102aaa4b5fddb3a14cba1be6cbb/DAY-12/GTKWAVE%20_3%20MAIN.png"> <br> <br>

</details>



## DAY-14 Post-synthesis simulation (GLS)
<details>
	<summary> Introduction </summary>
   Synthesis in VLSI design flow involves converting a high-level hardware description (usually in HDL) into a gate-level netlist. It optimizes logic for area, power, and timing. Key steps: design entry, synthesis, technology mapping, and optimization. Output is gate-level netlist ready for physical design and verification stages. <br><br>

**--> Pre-synthesis simulation:-**
Pre-synthesis simulation is a phase in digital circuit design and verification that occurs before the synthesis process. This simulation step involves simulating the behavior of a digital design at a higher abstraction level, typically at the register-transfer level (RTL) or even at the algorithmic level, before converting it into gate-level logic.<br>
Here's an overview of pre-synthesis simulation:<br>

Design Entry: Before pre-synthesis simulation can begin, you need a digital circuit design described at a higher level of abstraction. This design can be created using a hardware description language (HDL) like Verilog or VHDL, or it can be specified using a higher-level modeling language like SystemVerilog, C/C++, or MATLAB/Simulink.<br>

Behavioral or RTL-Level Design: In pre-synthesis simulation, you work with a design that represents the functionality of the digital circuit but doesn't specify the actual gates, flip-flops, or interconnections on a physical chip. This level of abstraction focuses on describing the data flow and control flow within the circuit.<br>

Simulation Tools: There are various simulation tools and environments for pre-synthesis simulation, including ModelSim, XSIM, and many others. These tools allow you to simulate the behavior of the design described in the HDL or modeling language.<br>

Testbench Development: Similar to gate-level simulation, you need to create a testbench for pre-synthesis simulation. The testbench includes test vectors, stimuli, and a simulation environment that applies inputs to the RTL design and monitors its outputs. Testbenches are essential for verifying the correctness of the circuit's functionality.<br>

Simulation Run: Once the testbench is ready, you can run the pre-synthesis simulation. During the simulation, the tool evaluates the behavior of the RTL-level design, processes input data, and produces output results based on the specified design description.<br>

Analysis and Debugging: After the simulation run, you analyze the results to ensure that the RTL-level design behaves as expected. You check for functional correctness, timing issues, and other design parameters. If any issues are identified, you can debug the RTL code to make necessary adjustments.<br>

Performance and Resource Estimation: Pre-synthesis simulation can also provide estimates of the design's performance and resource utilization. This information can be valuable for making design decisions and optimizations before proceeding to synthesis.<br>

Iterative Process: Similar to gate-level simulation, pre-synthesis simulation is often an iterative process. You may need to modify the RTL-level design, update the testbench, and rerun simulations until the design meets its specifications.<br>

Synthesis: Once the pre-synthesis simulation is successful, you can proceed to the synthesis step, where the RTL-level design is converted into gate-level logic that can be implemented on a physical chip.<br>

Pre-synthesis simulation helps identify and address design issues at a higher level of abstraction, allowing for quicker design exploration and debugging. It is an important step in the overall digital design flow, particularly for complex digital systems and integrated circuits.<br><br>


**-->Post-synthesis simulation:-**
Post-synthesis simulation is a crucial step in the digital circuit design and verification process that occurs after the synthesis stage. In post-synthesis simulation, you verify the behavior of a digital design at the gate-level, where the design has been transformed into actual logic gates, flip-flops, and interconnections.<br>
Here's an overview of post-synthesis simulation:<br>

Design Entry: Before post-synthesis simulation can begin, you need a digital circuit design described at a higher level of abstraction, typically in a hardware description language (HDL) like Verilog or VHDL.<br>

Synthesis: The design is synthesized to convert it from the RTL (Register-Transfer Level) description to a gate-level representation. This synthesis process generates a netlist, which is a list of actual logic gates, flip-flops, and their interconnections that implement the design's functionality.<br>

Simulation Tools: Post-synthesis simulation requires gate-level simulation tools. These tools, like Cadence's NC-Sim or Synopsys' VCS, take the gate-level netlist and simulate the behavior of the digital circuit.<br>

Testbench Development: As in pre-synthesis simulation, you need to create a testbench for post-synthesis simulation. The testbench includes test vectors, stimuli, and a simulation environment that applies inputs to the gate-level design and monitors its outputs.<br>

Simulation Run: You run the post-synthesis simulation, during which the tool evaluates the behavior of the gate-level design. Inputs are applied to the circuit, logic gates are evaluated, flip-flops change state, and the tool provides output waveforms and logs.<br>

Analysis: After the simulation run is complete, you analyze the results to ensure that the gate-level design behaves as expected. You check for correct functionality, timing violations, power consumption, and other design parameters.<br>

Timing Analysis: Post-synthesis simulation is particularly important for timing analysis. You verify that the design meets its timing requirements and that signals propagate through the logic gates within the specified clock cycles.<br>

Power Analysis: Post-synthesis simulation can also provide estimates of the design's power consumption, which is essential for power-aware design considerations.<br>

Debugging: If the simulation reveals any issues or unexpected behavior, you need to debug the design. Debugging at the gate level can be more challenging than at higher levels of abstraction, as you are dealing with the actual hardware implementation.<br>

Iterative Process: Like pre-synthesis simulation, post-synthesis simulation is often an iterative process. You may need to make design changes based on simulation results, update the testbench, and run simulations again until the design meets its specifications.<br>

Verification: Successful post-synthesis simulation is a critical step in verifying that the gate-level design correctly implements the intended functionality of the digital circuit.<br>

Post-synthesis simulation is a critical part of the digital design flow, as it ensures that the synthesized gate-level design meets the desired specifications and performs as expected before proceeding to physical implementation, such as FPGA programming or ASIC fabrication.<br>
 <br>
	
</details>


<details>
	<summary>Post-synthesis simulation of Priority decoder 2x4 </summary>
	The combinational circuit that change the binary information into 2N output lines is known as Decoders. The binary information is passed in the form of N input lines. The output lines define the 2N-bit code for the binary information. In simple words, the Decoder performs the reverse operation of the Encoder. At a time, only one input line is activated for simplicity. The produced 2N-bit output code is equivalent to the binary information. <br>
      In the 2 to 4 line decoder, there is a total of three inputs, i.e., A0, and A1 and E and four outputs, i.e., Y0, Y1, Y2, and Y3. For each combination of inputs, when the enable 'E' is set to 1, one of these four outputs will be 1. <br>

 **- Generated netlist after synthesis:-**
 <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/6c83bc5c8d1ba9649bec7249ed8c1ff1bcf77a61/DAY-13/2_netlist_decoder.png"> <br>

 **- Commands for simulation:-**
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a47a81049275b18773aae54f01b163812d27ebf/DAY-13/3_post_synthesis_simulation_decoder.png"> <br>

 **- Result:-**
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a47a81049275b18773aae54f01b163812d27ebf/DAY-13/4_post_synthesis_simulation_decoder_result.png"> <br>
  Can observe here it's giving outputs based on priority
  
 **- Schematic:-**
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a47a81049275b18773aae54f01b163812d27ebf/DAY-13/schematic%20for%20decoder%20.png"> <br>
	
</details>

<details>
	<summary>Post-synthesis simultion of BabySOC </summary>
	
 **--> Mythcore:-**

 *-Commands for simulation:-*
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a47a81049275b18773aae54f01b163812d27ebf/DAY-13/5_command_for_post_synthesis_simulation_myth_core.png"> <br>

 *-Result:-*
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a47a81049275b18773aae54f01b163812d27ebf/DAY-13/1_post_synthesis_mythcore.png"> <br>


 **--> BabySOC:-**

 *-Commands for simulation:-*
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a47a81049275b18773aae54f01b163812d27ebf/DAY-13/6_post%20synthesis%20simulation%20for%20main%20module.png"> <br>

 *-Result:-*
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/7a47a81049275b18773aae54f01b163812d27ebf/DAY-13/7_post%20synthesis%20simulation%20for%20main%20module_result.png"> <br>
 
</details>



## DAY-14 Synopsys DC And Timing analysis

<details>  <summary> Introduction </summary>
In chip designing, PVT corners refer to specific combinations of Process (P), Voltage (V), and Temperature (T) that represent the extreme conditions under which an integrated circuit (IC) must operate. Designing ICs to perform reliably and within specifications across a wide range of PVT conditions is critical because variations in these parameters can significantly impact the performance, power consumption, and reliability of the chip. PVT corners are used to account for these variations and ensure the chip meets its specifications under worst-case scenarios.<br>

*--> There are typically three primary PVT corners in chip designing,* <br>

*- Slow Process, Low Voltage, High Temperature (SLOW, LV, HT):* <br>

This corner represents the worst-case scenario where the manufacturing process is slow (meaning that transistors are relatively slow), the supply voltage is low, and the operating temperature is high. In this corner, the chip should still meet its performance and reliability requirements.<br>
*- Fast Process, High Voltage, Low Temperature (FAST, HV, LT):* <br>
This corner represents the opposite extreme, where the manufacturing process is fast, the supply voltage is high, and the operating temperature is low. Here, the chip should still meet its performance and reliability requirements.<br>

*- Nominal Process, Nominal Voltage, Nominal Temperature (NOM, NOM, NOM):* <br>

This corner represents the typical or nominal operating conditions for the chip. It assumes that the process, voltage, and temperature are all at their standard values. Most of the chip's performance and power specifications are defined under these conditions.
Designing for PVT corners involves extensive simulation and testing to ensure that the chip can operate and meet its specifications under these extreme conditions. This includes considering factors like voltage scaling, temperature management, and circuit design variations. By accounting for these PVT corners, chip designers can improve the overall robustness and reliability of the IC, ensuring that it performs as expected across a wide range of operating conditions.<br>

Additionally, designers may also consider additional corners or intermediate corners between these extremes to cover a broader range of operating conditions, especially if the chip is intended for use in a variety of applications with different requirements. Managing PVT variations is a complex but essential aspect of modern chip design to ensure that electronic devices function reliably in diverse environments.
<br><br>

**--> Why it's PVT Corners plays very important role,** <br>
PVT (Process, Voltage, Temperature) variations are critically important for the proper working of chips, especially in terms of timing, because they can significantly impact the performance and functionality of integrated circuits. <br>
Here's why PVT variations matter for timing in chip design:<br>

*- Process Variation:-*<br>
Process variations can lead to differences in transistor characteristics, gate delays, and interconnect resistances. These variations can affect the propagation delay of signals through the chip. In the slowest PVT corner (slow process, low voltage, high temperature), signal propagation is at its slowest, and this can lead to timing violations if not properly accounted for.<br>

*- Voltage Scaling:-* <br>
Voltage scaling is a common technique to manage power consumption in chips. When you lower the supply voltage, it can reduce power consumption but also increase signal propagation delay. Designing for different voltage levels and ensuring that timing requirements are met under various voltage conditions is essential for power-efficient chip design.<br>

*- Temperature Effects:-* <br>
Temperature can have a significant impact on the speed of transistors and other components on the chip. Higher temperatures can lead to increased leakage currents and reduced performance. In high-temperature conditions, circuits may need to operate at lower clock frequencies or require additional cooling to meet timing constraints.<br>

*- Reliability Considerations:-* <br>
Extreme temperature conditions, especially high temperatures, can affect the long-term reliability of a chip. Timing violations and excessive power dissipation can lead to electromigration and thermal stress, which can ultimately affect the lifespan of the chip. Designing to accommodate PVT variations helps ensure both short-term and long-term chip reliability.<br>


*- Yield and Manufacturing Variability:-* <br>
Semiconductor manufacturing processes are subject to inherent variations. Different chips from the same manufacturing process may have slightly different characteristics. Designing chips to operate reliably across a range of PVT conditions helps improve yield by ensuring that a larger percentage of manufactured chips meet their specifications.<br>

*- Real-world Conditions:-* <br>
Electronic devices operate in a wide range of real-world conditions, and PVT variations are inevitable. Chips need to perform reliably in different environmental temperatures, supply voltage fluctuations, and manufacturing process variations. Designing for PVT ensures that the chip functions as expected in practical scenarios.<br><br>
In summary, considering PVT variations in chip design, particularly in relation to timing, is crucial for ensuring that the chip operates reliably and meets its performance specifications across a wide range of conditions. This robustness is essential for electronic devices to function correctly in various applications and environments, from consumer electronics to critical infrastructure and automotive systems.
</details>



<details> <summary> LAB </summary>
--> First we will delete all the lines from the .lib with the error stated. After deleting the lines ,We will convert .lib file into .db file because we know all the Synopsys tool doesn't take file in .lib format, so we will convert by using followinf commands, <br>

```ruby
read_lib <library_name>
write_lib <library_name> -f db -o <name_of_the_db_file>
```

--> Below constraints file we will be using for our analysis,<br>

```ruby
 set_units -time ns
create_clock -name MYCLK -per 2 [get_pins {pll/CLK}];

set_clock_latency -source 1 [get_clocks MYCLK]
set_clock_uncertainty -setup 0.5 [get_clocks MYCLK]; 
set_clock_uncertainty -hold 0.4 [get_clocks MYCLK]; 

set_input_delay -max 1 -clock \[get_clocks MYCLK] [all_inputs];
set_input_delay -min 0.5 -clock \[get_clocks MYCLK] [all_inputs];
set_output_delay -max 1 -clock \[get_clocks MYCLK] [all_outputs];
set_output_delay -min 0.5 -clock \[get_clocks MYCLK] [all_outputs];

set_input_transition -max 0.2 \[all_inputs];
set_input_transition -min 0.1 \[all_inputs];

set_max_area  800;

set_load -max 0.2 \[all_outputs];
set_load -min 0.1 \[all_outputs];
```

**--> Now we will analyze the setup and hold for different operating conditions of PVT,** <br>

*1. Operating conditions,* <br>
    Process- SS <br>
    voltage- 28 <br>
    Temperature- 40C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/da09bb9d916867dbb0b25b15ee6a172c79d96b6a/DAY-14_FINAL/1.%20script%20for%20ss_040C_1v28.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/da09bb9d916867dbb0b25b15ee6a172c79d96b6a/DAY-14_FINAL/2.%20wns%20and%20tns%20%20ss_040C_1v28.png"> <br><br>

 *2. Operating conditions,* <br>
    Process- SS <br>
    voltage- 35 <br>
    Temperature- 40C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/da09bb9d916867dbb0b25b15ee6a172c79d96b6a/DAY-14_FINAL/3.%20script%20ss_040C_1v35.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/da09bb9d916867dbb0b25b15ee6a172c79d96b6a/DAY-14_FINAL/4.%20wns%20and%20tns%20ss_040C_1v35.png"> <br><br>

 *3. Operating conditions,* <br>
    Process- SS <br>
    voltage- 40 <br>
    Temperature- 40C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800" alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/da09bb9d916867dbb0b25b15ee6a172c79d96b6a/DAY-14_FINAL/5.%20script%20for%20ss_040C_1v40.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/da09bb9d916867dbb0b25b15ee6a172c79d96b6a/DAY-14_FINAL/6.%20wns%20and%20tns%20for%20ss_040C_1v40.png"> <br><br>

 *4. Operating conditions,* <br>
    Process- SS <br>
    voltage- 44 <br>
    Temperature- 40C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/da09bb9d916867dbb0b25b15ee6a172c79d96b6a/DAY-14_FINAL/7.%20script%20for%20ss_040C_1v44.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/da09bb9d916867dbb0b25b15ee6a172c79d96b6a/DAY-14_FINAL/8.%20wns%20and%20tns%20for%20ss_040C_1v44.png"> <br><br>

 *5. Operating conditions,* <br>
    Process- ff <br>
    voltage- 56 <br>
    Temperature- 40C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/da09bb9d916867dbb0b25b15ee6a172c79d96b6a/DAY-14_FINAL/9.%20script%20for%20ss_040C_1v56.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/da09bb9d916867dbb0b25b15ee6a172c79d96b6a/DAY-14_FINAL/10.%20wns%20and%20tns%20for%20ff_040C_1v56.png"> <br><br>

 *6. Operating conditions,* <br>
    Process- ff <br>
    voltage- 65 <br>
    Temperature- 40C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3d2918d21b527409fba3644697e322bb2aea69ec/DAY-14_FINAL/11.%20script%20for%20ff_040C_1v65.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3d2918d21b527409fba3644697e322bb2aea69ec/DAY-14_FINAL/12.%20wns%20and%20tns%20for%20ff_040C_1v65.png"> <br><br>

*7. Operating conditions,* <br>
    Process- ff <br>
    voltage- 76 <br>
    Temperature- 40C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3d2918d21b527409fba3644697e322bb2aea69ec/DAY-14_FINAL/13.%20script%20for%20ff_040C_1v76.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/3d2918d21b527409fba3644697e322bb2aea69ec/DAY-14_FINAL/14.%20wns%20and%20tns%20for%20ff_040C_1v76.png"> <br><br>


 *8. Operating conditions,* <br>
    Process- ss <br>
    voltage- 40 <br>
    Temperature- 100C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/15.%20script%20for%20ss_100C_1v40.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/16.%20wns%20and%20tns%20for%20ss_100C_1v40.png"> <br><br>


 *9. Operating conditions,* <br>
    Process- ss <br>
    voltage- 60 <br>
    Temperature- 100C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/17.%20script%20for%20ss_100C_1v60.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/18.%20wns%20tns%20for%20ss_100C_1v60.png"> <br><br>


 *10. Operating conditions,* <br>
    Process- ff <br>
    voltage- 65 <br>
    Temperature- 100C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/19.%20script%20for%20ff_100C_1v65.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/20.%20wns%20and%20tns%20for%20ff_100C_1v65.png"> <br><br>

 *11. Operating conditions,* <br>
    Process- ff <br>
    voltage- 95 <br>
    Temperature- 100C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/21.%20script%20for%20ff_100C_1v95.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/22.%20wns%20and%20tns%20for%20ff_100C_1v95.png"> <br><br>

 *12. Operating conditions,* <br>
    Process- SS <br>
    voltage- 76 <br>
    Temperature- 40C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/23.%20script%20for%20ss_n40c_1v76.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/24.%20WNS%20AND%20TNS%20for%20ss_n40c_1v77.png"> <br><br>

 *13. Operating conditions,* <br>
    Process- tt <br>
    voltage- 80 <br>
    Temperature- 25C <br>
    
 --> Below script we will source to perform,<br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/25.%20script%20for%20tt_025C_1v80.png"> <br>
  
 --> Output,<br> 
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8a6f2bd28db2880ef5c6d46cbab4754c9a07bbad/DAY-14_FINAL/26.%20wns%20and%20tns%20for%20tt_025C_1v81.png"> <br><br>



 **- Can see the below graphs, WNS and TNS for Setup of all the above cases,** <br>
  <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/29f0d0c74be4c346a66c8df2d81c03cf03d05346/DAY-14_FINAL/WNS%20for%20setup_n.PNG"> <br>
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/70b7883551885ee98fcf81b91c574a02a138a2c1/DAY-14_FINAL/for%20setup%20WNS.PNG"> <br>
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/de2a1c249f35bf9db6c568bc94e0aa6560a29cb5/DAY-14_FINAL/TNS%20for%20setup.PNG"> <br><br>

**- Can see the below graphs, WNS and TNS for Hold of all the above cases,** <br>
 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/29f0d0c74be4c346a66c8df2d81c03cf03d05346/DAY-14_FINAL/WNS%20for%20Hold_n.PNG"> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/70b7883551885ee98fcf81b91c574a02a138a2c1/DAY-14_FINAL/for%20hold%20wns.PNG"> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/de2a1c249f35bf9db6c568bc94e0aa6560a29cb5/DAY-14_FINAL/TNS%20for%20hold.PNG"> <br><br>

**--> Observations,** <br>

 - In faster cells, hold violations are common due to quick data processing. Faster cells allow less time for data to stabilize before capture. Here also we can see in operating conditions wherever we used ff process, there we can see the hold violations and further that becomes more dangerous as voltage and temperature increases.<br>
 
- In slower cells often face setup issues. Slower cells require more setup time because they process data slowly, potentially leading to setup violations if not met. Here also we can see in operating conditions wherever we used ss process, there we can see the setup violations and further that becomes more dangerous as voltage and temperature decreases.<br><br>
</details>



## DAY-15 Inception of EDA and PDK
<details>
	<summary> Introduction </summary>
	An integrated circuit (IC), often referred to as simply an IC, is a comprehensive assembly of electronic circuits situated on a single, compact flat component—commonly recognized as a "chip." This chip primarily consists of semiconductor material, predominantly silicon. The customary arrangement involves mounting the integrated circuit onto a printed circuit board (PCB), thereby giving rise to a fully operational electronic system.<br>
      <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/DAY-15%20I1.PNG"> <br>

View of, how complete system looks,<br>
      
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/I2.PNG"> <br>
      
*-->Core*  <br>
A "core" in the context of integrated circuit (IC) design denotes a fundamental functional block or module. Cores are meticulously crafted to execute precise tasks or functions, and their integration with other cores and components allows for the creation of intricate ICs with diverse functionalities to serve various purposes.<br>
*-->Die*  <br>
A "die" stands as a distinctive component within the context of silicon wafer intricacies, encapsulating an individual integrated circuit (IC) or chip. The silicon wafer undergoes meticulous division into multiple smaller sections, and within each of these sections resides a replicated version of the identical integrated circuit design. These segmented portions, aptly named "dies," represent miniature entities. It's noteworthy that each die, functioning as an independent entity, can operate autonomously once surgically separated from the wafer, embodying the essence of an individualized and self-sufficient chip.<br>
*-->Pads*  <br>
Pads serve as the tangible external connections or terminals on the SoC. These crucial points act as the interface between the SoC and the external environment, encompassing input and output pins for linking with other electronic components, power supply pins, ground pins, and more. Positioned along the periphery of the die, pads facilitate soldering or wire connections to the SoC, playing a pivotal role in establishing and expanding the SoC's connectivity.<br>
     
*- Varieties of Pads* <br>

- Input Pads: <br>
These serve as conduits for external signals entering the IC. For instance, they might receive data inputs from sensors or user interfaces, facilitating the integration of external information.<br>

- Output Pads: <br>
Designed for transmitting signals generated within the IC to external devices or other segments of a circuit. An example includes the use of output pads to send data to a display or transmit information to another IC.<br>
- Power Pads: <br>
Essential for providing power to the IC, these pads are typically linked to the power supply voltage (VDD) and ground (GND), ensuring the energy requirements of the IC are met.<br>

- Ground Pads: <br>
Connected to the ground reference voltage (GND), ground pads play a critical role in maintaining proper functionality and reducing noise within the circuit.<br>

- No-Connect Pads: <br>
Some pads intentionally remain unconnected and are designated as "no-connect" to prevent unintended connections, ensuring the integrity and stability of the circuit.<br>

 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/I3.PNG"> <br>
 Contained within a QFN-48 package, denoting Quad Flat No Leads with 48 pins, this specific component boasts a dimension of 7mm by 7mm. Each of the 48 pins serves as a vital connection point, establishing interfaces with various components or packages integrated onto the design board. The central focal point within this package is typically occupied by a microchip. The pins situated on the periphery, commonly termed "outbounds," play a pivotal role in orchestrating the seamless exchange of data between the external world and the encapsulated chip, thus contributing significantly to the functionality of the entire package.
</details>


<details>
	<summary> RTL to GDS</summary>
	 <img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/RTL%20to%20GDS.PNG"> <br>
	
 **->Synthesis:-**
 synthesis is a critical step that involves the transformation of a high-level hardware description of a digital circuit, often articulated in a hardware description language (HDL) like VHDL or Verilog. This transformation leads to the creation of a netlist, a representation encompassing both the logical and physical components essential for shaping the actual integrated circuit.<br>

During this intricate process, standard cells emerge as fundamental building blocks. These cells boast a consistent layout, and each one is depicted in various perspectives, including electrical, HDL, and SPICE models. Notably, standard cells offer both abstract and detailed layout views. These versatile components play a pivotal role in the synthesis journey, contributing significantly to the construction of the final layout of the integrated circuit. Their regularity and adaptability make them indispensable in achieving optimal functionality and efficiency in the overall design. <br><br>

**->Floorplan:-**
Floor planning, a pivotal early-stage process in VLSI design, entails defining the physical layout and strategic placement of functional blocks, modules, and components within an integrated circuit (IC). This meticulous planning is crucial for optimizing various factors such as chip area, signal routing, power distribution, and thermal management.<br>

*- Chip Floorplan:*<br>

The term "Chip Floorplan" specifically refers to the meticulously designed layout for an integrated circuit (IC) or semiconductor chip. This layout, presented as a diagram, intricately details the physical arrangement and placement of diverse components, functional blocks, and critical elements within the silicon area of the chip.<br><br>

*- Macro Floorplan:*<br>

In semiconductor and integrated circuit (IC) design, a "Macro Floorplan" stands as a distinct type of floorplan. This is particularly utilized in the context of macros, which are predefined and pre-characterized functional blocks or modules within an IC, each performing a specific function. Macros can encompass anything from processor cores to memory blocks, representing complex building blocks strategically positioned within the IC.<br><br>

*- Power Planning :*<br>

Power planning in VLSI design is a critical facet of semiconductor chip design, focusing on the management and distribution of electrical power within the IC. Effective power planning is indispensable for achieving reliable and efficient operation while minimizing power consumption. This aspect plays a crucial role in the overall success of the VLSI design by ensuring optimal power delivery and consumption throughout the integrated circuit.<br><br>

**->Placement:-**

Placement emerges as a pivotal step in the physical design process of crafting integrated circuits (ICs). This intricate phase revolves around strategically determining the optimal locations for each logical cell, commonly known as standard cells, within the silicon area of the chip. The effectiveness of this placement profoundly influences critical factors such as performance, power consumption, and chip area utilization.<br>

*- Objectives of Placement:*

The primary goal of the placement process is to orchestrate standard cells in a configuration that achieves multiple objectives. These include minimizing the total wirelength, which refers to the aggregate length of wires connecting the cells. Additionally, effective placement aims to optimize chip area utilization and adhere to various design constraints, encompassing crucial aspects such as timing, power, and manufacturability.<br>

In summary, placement is a meticulous and strategic endeavor in the IC design journey, aiming to strike a delicate balance that enhances performance, reduces power consumption, optimizes chip area utilization, and meets stringent design constraints to ensure the overall success and efficiency of the integrated circuit.<br><br>


**-> Clock Tree Synthesis (CTS):-** 

CTS, an acronym for "Clock Tree Synthesis," holds a pivotal role in the intricate process of physically designing integrated circuits (ICs). It specifically focuses on the generation and optimization of the clock distribution network within the chip.<br>

*- Primary Objective of CTS:* <br>
The primary goal of CTS is to ensure the efficient and reliable distribution of clock signals to all flip-flops and sequential elements within the IC. This involves minimizing clock skew, the variation in arrival times of clock signals at different points, and meeting the stringent timing constraints crucial for the synchronized operation of the chip.<br>

*- Significance in VLSI Design:*<br>
Clock Tree Synthesis is deemed a critical step in VLSI design due to its profound impact on the overall performance, power consumption, and reliability of integrated circuits. A well-designed clock distribution network enhances the chip's efficiency and mitigates issues related to timing discrepancies.<br>

*- Automation and Optimization:*<br>
To tackle the complexities of modern and high-performance ICs, advanced algorithms and tools are employed to automate and optimize the CTS process. These tools play a key role in achieving precision and efficiency in the distribution of clock signals, contributing to the success of the overall VLSI design.<br>

In essence, Clock Tree Synthesis stands as a fundamental and meticulous phase in VLSI design, ensuring that the heartbeat of the chip—the clock signals—is orchestrated with precision, impacting its performance, power efficiency, and reliability.<br><br>


**-> Routing:-**
Routing, within the context of Very Large Scale Integration (VLSI) design, stands as a foundational step in the intricate process of physically crafting integrated circuits (ICs). This critical phase involves the strategic generation of physical connections, employing metal traces or wires, that interlink the diverse components and logic elements situated on the chip.

*- Efficient Signal and Power Routing:* <br>
The core objective of routing is to establish efficient pathways for the transmission of data signals, control signals, and power throughout the IC. This meticulous interconnection process ensures that the intricate web of signals and power distribution adheres to design constraints, such as timing, power consumption, and manufacturability.<br>

*- Impact on IC Performance:* <br>
Routing's significance reverberates in its critical role in determining the overall performance of the IC. The efficiency of data transmission, the accuracy of control signal propagation, and the reliability of power distribution are all contingent on the effectiveness of the routing strategy implemented.<br>

*- Key Determinants:* <br>
Routing, being a linchpin of the VLSI design process, significantly influences the power consumption, performance metrics, and overall functionality of the IC. The intricacies of the routing decisions made during this phase ripple through the entirety of the IC's design and functionality.<br>

In conclusion, routing in VLSI design is not merely the physical connection of components; it is a strategic and pivotal phase that intricately weaves the pathways for signals and power, shaping the backbone of an efficiently functioning integrated circuit.<br><br>


**-> Signoff:-**

Sign Off marks the conclusive stage in the design process just before the design is dispatched for fabrication or manufacturing. This pivotal phase involves an exhaustive set of checks, analyses, and validations to guarantee that the integrated circuit (IC) design aligns with all requisite criteria, constraints, and specifications before proceeding to the foundry for manufacturing. <br>

*- Comprehensive Validation Process:* <br>
At Sign Off, the design undergoes a meticulous validation process encompassing checks for functionality, performance, and adherence to design constraints. This all-encompassing examination ensures that every facet of the IC design is thoroughly reviewed and approved before transitioning to the manufacturing phase. <br>

*- Critical Nature of Sign Off:* <br>
The Sign Off stage assumes paramount importance as any undetected design errors or issues at this juncture can potentially lead to costly and time-consuming problems. These issues might manifest during subsequent phases of the manufacturing process or even after the ICs are in operation, underscoring the critical nature of a rigorous and comprehensive Sign Off. <br>

*- Preventing Future Complications:* <br>
By addressing potential design discrepancies and ensuring alignment with specifications, Sign Off serves as a preventive measure. It aims to circumvent complications that could arise in the manufacturing process or during the operational life of the ICs, safeguarding against disruptions and optimizing the overall efficiency and reliability of the integrated circuits. <br>

In conclusion, Sign Off is not just a procedural formality; it is the last line of defense against design anomalies, offering assurance that the integrated circuit is ready for the next stages of manufacturing and operational deployment. <br><br>


**-> Pysical verification:-**

Physical Verification stands as a crucial phase in the design process of integrated circuits (ICs), involving a meticulous series of checks and analyses. Its primary objective is to confirm that the physical layout of the IC aligns with specified design rules, constraints, and manufacturing prerequisites. This scrutiny is essential for ensuring the manufacturability, functionality, and reliability of the IC design before it advances to the fabrication stage. <br>

*-->Design Rule Checking (DRC):* <br>

*- Geometry Checks:* <br>
DRC meticulously validates that the layout strictly adheres to the design rules set by the foundry. This encompasses scrutinizing minimum feature sizes, spacing requirements, and the width and spacing of metal layers, along with other geometric constraints. <br>
*- Layer-Specific Rules:* <br>
Different layers within the IC come with specific design rules. DRC conducts comprehensive checks to ensure compliance across all layers, including metal, polysilicon, diffusion, and more. <br><br>


*-->Electrical Rule Checking (ERC):* <br>
*- Electrical Connectivity:* <br>
ERC ensures the absence of electrical shorts or opens in the layout, verifying that the actual connections align with the intended connectivity outlined in the schematic.<br>
*- Antenna Checking:* <br>
ERC extends its scrutiny to charge buildup issues, known as antenna effects, which may arise during the manufacturing processes of deposition and etching. <br><br>


*- Layout Versus Schematic (LVS) Verification:* <br>
*- Netlist Consistency:* <br>
LVS performs a meticulous comparison between the layout netlist and the schematic netlist, ensuring their equivalence. Any disparities are flagged for resolution.<br>
*- Parasitic Extraction:* <br>
Parasitic elements like capacitance and resistance are extracted from the layout and cross-referenced with the schematic to verify electrical equivalence.<br>
In summary, Physical Verification acts as the gatekeeper, validating the precision and compliance of the IC design with stringent rules and requirements. By addressing geometric, electrical, and schematic considerations, this phase plays a pivotal role in fortifying the IC's journey from design to fabrication.

</details>


<details> 
	<summary>LAB</summary>
	
**OpenLane :-**
OpenLane stands out as a trailblazing and open-source toolchain, empowering the creation of custom Application-Specific Integrated Circuits (ASICs). Widely recognized in the semiconductor realm, it's celebrated for making chip design accessible to all. OpenLane boasts a comprehensive suite of EDA (Electronic Design Automation) tools and scripts, smoothing the journey from RTL (Register Transfer Level) to GDSII (Graphic Design System II) in ASIC design. It's not just a tool—it's a movement, championing accessibility, collaboration, and personalized circuit creation. This tool gives developers, from hobbyists to seasoned pros, the keys to design and produce custom chips tailored to their unique specifications. OpenLane's transparent, community-driven ethos is a breath of fresh air, propelling ASIC design forward and breaking down the traditionally high barriers to entry in this field.<br>

--> Commands:- <br>

```ruby
/flow.tcl -interactive
package require openlane 0.9
prep -design picorv32a
run_synthesis
```
<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/1."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/2."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/3."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/4."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/5."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/6."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/7."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/8."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/9."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/9.b"> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/10."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/11."> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/12.png"> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/e9b787e91e6822ef6b2309a60409e738b1915e83/DAY-15/12."> <br>
-> before we run synthesis we can see runs is created here after setting up the design,<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8f17441d40f6e37b18b22a7ba532803dcabcb5a1/DAY-15/13%20before%20we%20run%20synthesis%20we%20can%20see%20runs%20is%20created%20here%20after%20setting%20up%20the%20design.png"> <br>
-> we can see in runs just now one file is created wrt to current time,<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8f17441d40f6e37b18b22a7ba532803dcabcb5a1/DAY-15/14%20we%20can%20see%20in%20runs%20just%20now%20one%20file%20is%20created%20wrt%20to%20current%20time.png"> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8f17441d40f6e37b18b22a7ba532803dcabcb5a1/DAY-15/15.png"> <br>
-> by commanding less merged.lef we can see all the content which is about metal layer,vias,etc,<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8f17441d40f6e37b18b22a7ba532803dcabcb5a1/DAY-15/16.%20by%20commandinf%20less%20merged.lef%20we%20can%20see%20all%20the%20content%20which%20is%20about%20metal%20layer%2Cvias%2Cetc.png"> <br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8f17441d40f6e37b18b22a7ba532803dcabcb5a1/DAY-15/16.png"> <br>
-->  since we havn't done synthesis yet so we can see every othere info is empty,<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8f17441d40f6e37b18b22a7ba532803dcabcb5a1/DAY-15/18.%20since%20we%20havn't%20done%20synthesis%20yet%20so%20we%20can%20every%20othere%20info%20is%20empty.png"> <br>
 --> we haven't done synthesis yet so we can see all the other result and stage reports and synthesis reports are empty,<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8f17441d40f6e37b18b22a7ba532803dcabcb5a1/DAY-15/19.%20we%20haven't%20done%20synthesis%20yet%20so%20we%20can%20all%20the%20other%20reports%20and%20synthesis%20reports%20are%20empty.png"> <br>
--> config.tcl,<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/8f17441d40f6e37b18b22a7ba532803dcabcb5a1/DAY-15/20.%20config.tcl%20.png"> <br>
--> Giving the commands to run synthesis,<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/32609b61099912cfe7897f3f52793314fc779b53/DAY-15/22.%20giving%20the%20command%20to%20run%20synthesis.png"> <br>
--> Can see, synthesis is done,<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/32609b61099912cfe7897f3f52793314fc779b53/DAY-15/23.%20synthesis%20done.png"> <br>
--> From the synthesis report, we can calculate the flop ratio by the use of no. of DFF and total no. of cells,<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/32609b61099912cfe7897f3f52793314fc779b53/DAY-15/24.%20from%20synthesis%20report%20calculate%20flop%20ratio%20by%20the%20use%20of%20no.%20of%20DFF%20and%20total%20no.%20of%20cells.png"> <br>
--> Earlier it was empty but now after synthesis, we can see the netlist is generated,<br>
<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/32609b61099912cfe7897f3f52793314fc779b53/DAY-15/25.%20earlier%20it%20was%20empty%20but%20now%20after%20synthesis%20we%20can%20see%20the%20netlist%20is%20generated.png"> <br><br>

- The number of d flip flops = 1613 <br> 
- Total Number of cells = 14876 <br> 
- *D flip flop ratio* = 1613/14876 => **0.108429** or In percentage **10.8429%** <br> 


</details> 


## DAY-16 Understand the importance of good floorplan vs bad floorplan and Introduction to library cells
<details> 
<summary> Utilization factor and Aspect ratio </summary>
	  Utilization Factor and Aspect Ratio are important parameters in VLSI (Very Large Scale Integration) chip design that play a crucial role in determining the efficiency and performance of integrated circuits. <br>
	 --> Let's delve into each of these concepts in detail: <br>
	
**Utilization Factor:-** <br>

*-> Definition:* The utilization factor, often denoted as UF is a metric that measures the effective usage of a given area on a silicon wafer for placing digital circuit components such as gates, flip-flops, and other functional blocks. It is expressed as the ratio of the total area occupied by the circuit components to the total available area on the chip.

*-> Formula:* <br>
**Utilization Factor (UF) = (Total Area Occupied by Components) / (Total Available Area on Chip)**  <br>

*-> Importance:* <br>

Efficient Space Utilization: A high utilization factor indicates efficient use of silicon real estate, which is essential for optimizing chip size and manufacturing cost. <br>
Minimizing Cost: Smaller chip sizes result in lower manufacturing costs, which is critical in the high-volume production of integrated circuits. <br>
Avoiding Overcrowding: While maximizing utilization is desirable, it's important not to overcrowd the chip, as this can lead to increased heat generation and signal interference. <br> <br>

*->Design Considerations:* <br>

Logic Synthesis: During the logic synthesis stage of chip design, tools aim to minimize the area occupied by gates and other logic elements while meeting the required functionality. <br>
Floorplanning: Careful floorplanning is essential to efficiently place components on the chip's layout, ensuring a balanced and effective utilization of space. <br>
Optimization Algorithms: Utilization factor can be improved using optimization algorithms that seek to minimize chip area while meeting performance and power constraints. <br><br>


**Aspect Ratio:** <br>

*->Definition:* The aspect ratio of a chip refers to the ratio of its width to its height. In VLSI chip design, the aspect ratio plays a significant role in determining the chip's layout and fabrication process. <br>

**Formula: Aspect Ratio = (Width of the Chip) / (Height of the Chip)** <br>

*->Importance:* <br>

Fabrication Compatibility: The aspect ratio influences the ease of manufacturing and the yield of the chips. Fabrication processes may have limitations on the maximum or minimum aspect ratio they can support. <br>
Routing and Signal Propagation: The aspect ratio affects the routing of interconnects between components on the chip. A well-chosen aspect ratio can minimize signal propagation delays and improve overall  performance. <br>
Heat Dissipation: The aspect ratio can also impact the thermal characteristics of the chip. A chip with a long, narrow shape may have difficulties dissipating heat efficiently. <br><br>


*->Design Considerations:* <br>

Process Technology: Designers must consider the capabilities and constraints of the specific semiconductor fabrication process being used. Different processes may have different aspect ratio limitations.<br>
Signal Timing: The aspect ratio should be chosen to minimize signal delays, especially for high-speed designs. A balanced aspect ratio can help ensure that signals traverse the chip with minimal skew.<br>
Thermal Management: For chips with high power density, an aspect ratio that facilitates effective heat dissipation through packaging and cooling solutions is crucial.<br>
In summary, the utilization factor and aspect ratio are critical factors in VLSI chip design. Achieving an optimal balance between efficient space utilization and manufacturing constraints is essential to produce cost-effective, high-performance integrated circuits. Designers must carefully consider these factors during the various stages of chip design, from logic synthesis to layout and fabrication.<br>
</details>

<details>
	<summary> Concept of Preplaced cells </summary>
	Preplaced cells are a fundamental concept in VLSI (Very Large Scale Integration) system design, particularly in the context of digital integrated circuits. These cells play a crucial role in defining the layout and organization of the chip.<br>
	
*--> Below is a detailed explanation of preplaced cells in VLSI system design:* <br>

*Definition:* <br>

Preplaced cells, often referred to as predefined cells or macrocells, are fixed-layout blocks or functional units that are placed at specific locations on the silicon wafer before the automatic placement and routing stages of the chip design process. These cells are typically designed to perform specific functions and are placed manually by the chip designer at strategic positions within the chip layout.<br>

*Key Characteristics and Information:* <br>

*Purpose:* <br>

Functional Units: Preplaced cells represent functional units or blocks of logic that provide specific features or functionality within the chip. They can include components such as memory blocks, analog modules, standard cells, or other predefined building blocks. <br>

Area Optimization: The placement of preplaced cells allows designers to optimize the use of valuable silicon area for critical functions, ensuring that these functions are located optimally for performance, power efficiency, and signal integrity. <br>

*Manual Placement:*  <br>

Manual Intervention: Unlike standard cells, which are placed automatically by EDA (Electronic Design Automation) tools during the place and route stage, preplaced cells are manually positioned by the chip designer. This manual placement is typically based on design constraints and the specific requirements of the chip. <br>

Fixed Locations: Once placed, preplaced cells remain fixed at their designated locations during the subsequent phases of chip design and manufacturing. This is essential for maintaining the integrity of critical functions. <br>

*Usage Scenarios:* <br>

Analog and Custom Blocks: Preplaced cells are commonly used for analog or custom-designed blocks that require precise placement and are not amenable to automated placement and routing. Examples include analog-to-digital converters (ADCs), digital-to-analog converters (DACs), and custom-designed memory blocks. <br>

Clock and Power Distribution: In many cases, clock generation and distribution networks are preplaced to ensure that clock signals reach all parts of the chip efficiently and with minimal skew. Similarly, power distribution networks are often carefully designed and preplaced to ensure proper power delivery. <br>

*Design Trade-offs:* <br>

Design Flexibility vs. Efficiency: While preplaced cells offer precise control over placement, they can limit the flexibility of design changes later in the process. Therefore, their use should strike a balance between design efficiency and adaptability <br>

Performance Optimization: Preplaced cells can be strategically positioned to optimize critical signal paths, reduce signal delays, and enhance overall chip performance. This is particularly important for high-speed or high-frequency designs. <br>

*Verification and Timing Closure:* <br>

Timing Constraints: The placement of preplaced cells affects timing constraints, and designers must ensure that the design meets required performance specifications and timing closure goals. <br>

Signal Integrity: The positioning of preplaced cells can also impact signal integrity and should be carefully considered to minimize signal skew, crosstalk, and other potential issues. <br>

In summary, preplaced cells are a vital component of VLSI system design, allowing designers to manually place critical functional units and optimize the chip layout for performance, power efficiency, and signal integrity. While they provide precise control over placement, careful consideration must be given to their usage and positioning to meet design requirements and constraints effectively.
</details>



<details> 
<summary>Decoupling capacitor</summary>

Decoupling capacitors are essential components in VLSI (Very Large Scale Integration) system design, playing a critical role in ensuring the stable and reliable operation of integrated circuits. They are primarily used to manage power supply noise and voltage fluctuations, which can have a significant impact on the performance and functionality of digital chips.<br>

*--> Below is detailed information about decoupling capacitors in VLSI system design:* <br>

*Definition:* <br>

Decoupling capacitors, also known as bypass capacitors or simply decaps, are passive electronic components that are placed strategically on an integrated circuit (IC) to mitigate voltage fluctuations and noise on the power supply lines. They provide a local reservoir of charge, which can be quickly drawn upon to compensate for sudden changes in current demand.<br><br>

*Key Characteristics and Information:* <br>

*Purpose:* <br>

Noise Reduction: Decoupling capacitors primarily serve to reduce power supply noise caused by digital switching activity, which can introduce unwanted voltage spikes and noise onto the power rails. <br>

Stabilization: They stabilize the power supply voltage, ensuring that it remains within an acceptable range during transient events, such as clock edges or data transitions. <br>

Preventing Glitches: Decoupling capacitors helps prevent glitches and logic errors that can occur when power supply voltages momentarily drop below-specified thresholds. <br><br>

*Location and Placement:* <br>

Close Proximity: Decoupling capacitors are placed as close as possible to the power and ground pins of individual components, such as flip-flops, gates, or memory cells. This proximity reduces the impedance of the power distribution network and enhances its effectiveness. <br>

Different Capacitor Sizes: Depending on the specific requirements of the component, different capacitor sizes may be used throughout the chip. Smaller capacitors (e.g., 100nF) address high-frequency noise, while larger capacitors (e.g., 1uF or more) handle lower-frequency fluctuations. <br><br>

*Types of Decoupling Capacitors:* <br>

Ceramic Capacitors: These are commonly used due to their low cost, high capacitance values, and good high-frequency characteristics. They come in various dielectric materials like X7R, X5R, and others. <br>

Tantalum Capacitors: Tantalum capacitors offer high capacitance values in a compact form factor. They are suitable for applications where space is limited. <br>

Electrolytic Capacitors: These capacitors are used when very high capacitance values are required but are less common in VLSI due to their larger size and slower response time compared to ceramic and tantalum capacitors. <br><br>

*Design Considerations:* <br>

Decoupling Network: Multiple decoupling capacitors are often used in a network to provide better filtering across a range of frequencies. This can include a combination of small and large capacitors to address both high-frequency and low-frequency noise. <br>

Simulation and Analysis: Tools like SPICE (Simulation Program with Integrated Circuit Emphasis) are used to analyze and simulate the effectiveness of decoupling capacitor placement and values to meet design goals. <br>

Layout and Routing: Proper placement and routing of power distribution lines are essential to ensure that power is delivered efficiently to the decoupling capacitors and distributed evenly throughout the chip.
<br>

*Impact on Performance:* <br>

Timing and Signal Integrity: Well-designed decoupling networks help improve signal integrity by reducing power supply noise, minimizing signal jitter, and preventing glitches that can affect timing. <br>

Power Consumption: Effective decoupling can also lead to lower power consumption, as it reduces the need for circuits to operate at higher voltages or consume additional power to overcome noise-induced errors.
<br><br>
In conclusion, decoupling capacitors are a critical part of VLSI system design, used to manage power supply noise and voltage fluctuations, enhance the stability of integrated circuits, and improve their overall performance and reliability. Proper placement, selection, and network design of decoupling capacitors are essential for achieving optimal results in VLSI designs. <br>
</details>


<details>
	<summary>Power planning </summary>
	Power planning, the use of decoupling capacitors, ground bounce, voltage droop, and voltage mesh are all important aspects of VLSI (Very Large Scale Integration) system design that play a crucial role in managing power distribution and ensuring reliable operation of integrated circuits.<br>
        Let's explore each of these concepts in detail: <br>
	
**--> Power Planning:**

Definition: Power planning, also known as power distribution network (PDN) design, involves the layout and distribution of power supply lines (VDD) and ground lines (VSS or GND) throughout the chip. The goal is to ensure efficient and low-impedance delivery of power to all functional blocks.

*- Importance:*

Proper power planning is essential to avoid voltage drops, noise, and signal integrity issues.
It helps maintain stable power supply voltages, which are crucial for reliable circuit operation.
Effective power planning also contributes to minimizing power dissipation.

**- Use of Decoupling Capacitors:**

Definition: Decoupling capacitors, as explained in a previous response, are placed strategically on the chip to mitigate voltage fluctuations and noise on the power supply lines.

Importance: Decoupling capacitors provide a local charge reservoir, reducing power supply noise and stabilizing voltage levels.
They are crucial for maintaining signal integrity, preventing glitches, and ensuring reliable circuit operation, especially in high-speed designs.

**- Ground Bounce:**

Definition: Ground bounce refers to the temporary increase in the ground voltage potential at the ground (VSS or GND) pins of digital components during a switching event. It occurs due to the inductance and resistance in the ground network. <br>

 Causes and Consequences: <br>
Rapid switching of digital signals can cause ground bounce.<br>
Ground bounce can lead to incorrect logic levels, increased power consumption, and even functional errors in the design if not managed properly.<br>

 Mitigation: <br>
Proper power planning and decoupling capacitor placement help mitigate ground bounce. <br>
Ground lines should be designed with low resistance and inductance to minimize voltage fluctuations. <br>



**- Voltage Droop:**  <br><br>

Definition: Voltage droop, also known as IR drop, refers to a temporary reduction in the power supply voltage (VDD) at a specific location on the chip during a high-current demand event.<br>

Causes and Consequences: <br>
High-current draws, such as during logic transitions or memory read operations, can cause voltage droop. <br>
Voltage droop can lead to logic errors, timing violations, and reliability issues. <br>

Mitigation: <br>
Power planning plays a significant role in reducing voltage droop by ensuring low-impedance power distribution. <br>
Decoupling capacitors help provide charge during high-current demands, reducing voltage droop. <br>


**- Voltage Mesh:**  <br><br>

Definition: A voltage mesh is a network of power distribution lines (VDD) and ground lines (VSS) designed to provide a uniform voltage supply and minimize IR drop across the chip. <br>

Importance: <br>
Voltage mesh design is critical for maintaining consistent power supply voltages, especially in large and complex chips.<br>
It ensures that power is evenly distributed, reducing voltage droop and ground bounce.<br>

Design Considerations:<br>
Multiple power rails may be used to create voltage islands within the chip, each with its voltage mesh.<br>
Advanced voltage regulation techniques, such as on-chip voltage regulators, can be employed to further improve voltage stability. <br>

In summary, power planning, decoupling capacitors, ground bounce, voltage droop, and voltage mesh are all integral parts of VLSI system design aimed at ensuring reliable and stable power distribution within integrated circuits. Proper consideration and implementation of these techniques are essential for achieving optimal chip performance, signal integrity, and functionality. <br>
</details>







<details>
	<summary>LAB- OpenLANE for floorplan</summary>
	--> The Images given below give a clear picture of how the floorplan is done in Openlane and how the directories look before and after the run, <br>
        ->README.md file which will say what all parameters need to be set for each stage,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/26.%20README.md%20file%20which%20will%20say%20what%20all%20parameter%20are%20need%20to%20be%20set%20for%20each%20stage.png"> <br>
        -> parameters which are needed to be set for floorplan,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/27.%20parameter%20which%20are%20needed%20to%20be%20set%20for%20floorplan.png"> <br>
        ->command to see default values are set for floorplan,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/28.%20command%20to%20see%20default%20values%20are%20set%20for%20floorplan%20.png"> <br>
        -> What all default values are set for floorplan,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/28.%20what%20all%20default%20values%20are%20set%20for%20floorplan%20.png"> <br>
	->command to see that config.tcl file values which are set for floorplan,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/30.%20command%20to%20see%20that%20config.tcl%20file%20values%20which%20are%20set%20for%20floorplan%20.png"> <br>
        ->config.tcl file values which are set for floorplan,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/31.%20config.tcl%20file%20values%20which%20are%20set%20for%20floorplan%20.png"> <br>
        -> Now we can see after running the floorplan there is reports are getting generated,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/32.%20now%20we%20can%20see%20after%20running%20floorplan%20there%20is%20reports%20are%20getting%20generated.png"> <br>
        ->can see in this what all parameter it has taken,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/35.%20can%20see%20in%20this%20what%20all%20parameter%20it%20has%20taken.png"> <br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/35.%20can%20see%20in%20this%20what%20all%20parameter%20it%20has%20taken.png"> <br>
        ->DEF file after running floorplan,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/36.%20DEF%20file%20after%20running%20floorplan.png"> <br>
        ->To see the actual layout after the floorplan,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/37.%20To%20see%20the%20actual%20layout%20after%20floorplan.png"> <br>
	->Can see the layout after floorplan,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/38.%20Can%20see%20the%20layout%20after%20floorplan.png"> <br>
        ->"what" command,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/what.png"> <br>
        ->Reviwing layout after floorplan,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/39.%20Reviwing%20layout%20after%20floorplan.png"> <br>
        ->reviewing layout after floorplan--> Tap cells ,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/41.%20reviewing%20layout%20after%20floorplan...%20Tap%20cells%20.png"> <br>
	-> reviewing layout after floorplan... preplaced cells in the left bottommost core,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/42.%20reviewing%20layout%20after%20floorplan...%20preplaced%20cells%20in%20left%20bottom%20most%20core.png"> <br>
</details>








<details>
	<summary> Netlist binding and Placement </summary>
	Library netlist binding and initial place design are important stages in the physical design flow of VLSI (Very Large Scale Integration) chip design. These stages are critical for achieving efficient chip layouts and ensuring that the final design meets performance and area requirements. <br>
	-> Here's detailed information about both concepts: <br>
	
**-> Library Netlist Binding:** <br><br>

*Definition:* <br>

Library Netlist: A library netlist is a representation of the logic functions and standard cells available in the chip design library. It includes information about the functionality, timing characteristics, and power consumption of each standard cell. <br>

Binding: Library netlist binding is the process of associating specific standard cells from the design library with the logic gates and components specified in the RTL (Register-Transfer Level) description of the digital design. <br>

*Importance:*

Functional Mapping: Library netlist binding maps the high-level functional description of a design to the actual standard cell instances that will be used in the physical implementation. <br>

Performance Optimization: By selecting appropriate cells from the library, designers can optimize for various factors, such as area, speed, and power consumption, to meet the design's performance goals. <br>

Timing Analysis: Binding determines the logical and physical connectivity of cells, which is essential for accurate timing analysis and optimization. <br>

*Design Considerations:*

Cell Selection: Designers must choose the most suitable standard cells from the library based on the design's requirements, considering factors like speed, area, and power. <br>

Cell Connectivity: Binding involves specifying how cells are connected in the netlist, including input and output pins, signal connections, and power and ground connections. <br>

Technology Constraints: Design libraries may have constraints and guidelines that must be followed during netlist binding, such as minimum and maximum fanout, drive strength, and more. <br>

*Tools:*

Netlist binding is typically performed using Electronic Design Automation (EDA) tools that provide the ability to select, connect, and configure standard cells from the design library.<br><br>


**-> Initial Place Design:** <br>

*Definition:*

Initial Placement: Initial place design is the process of positioning the standard cell instances on the chip's layout canvas before further optimization and routing. It involves defining the approximate locations of each cell based on a variety of factors, including logic connectivity, power distribution, and timing requirements. <br>

*Importance:*<br>

Layout Efficiency: Proper initial placement can significantly impact the chip's layout efficiency, ensuring that components are positioned optimally to reduce wire length and area usage. <br>

Timing and Signal Integrity: The initial placement can have a substantial effect on signal timing, signal integrity, and power distribution, making it crucial for achieving design goals. <br>

Reduced Design Iterations: A good initial placement can reduce the need for extensive subsequent iterations and adjustments during the physical design flow. <br>

*Design Considerations:* <br>

Hierarchical Approach: Initial placement is typically performed hierarchically, starting from the chip level and working down to individual blocks or sub-modules within the design. <br>

Legal Placement: The placement must adhere to legal constraints, which may include avoiding overlap between cells, maintaining specified clearances, and respecting the overall chip floor plan. <br>

Timing-Driven Placement: Timing-driven placement considers the critical paths and timing constraints of the design, placing critical cells first to meet performance requirements. <br>

*Tools:* <br>

Initial placement is typically carried out using EDA tools specifically designed for physical design, which take into account various constraints and objectives. <br><br>


In summary, library netlist binding and initial place design are crucial stages in the physical design flow of VLSI chip design. Netlist binding associates functional descriptions with physical standard cells, while initial placement positions these cells on the chip's layout canvas, setting the stage for subsequent optimization and routing. These stages are vital for achieving efficient and high-performance chip layouts.
</details>







<details>
	<summary> LAB- OpenLANE for Placementc</summary>
	->Result after run_placement,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/43.%20Result%20after%20run_placement.png"> <br>
        ->To see the layout post placement,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/44.%20To%20see%20the%20layout%20post%20placement.png"> <br>
	->Layout post placement,<br>
	<img width="800"  alt="netlist" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/52ec2c3df782605e02dae4eb8238ed5edd322889/DAY-16/45.layout%20post%20placement.png"> <br>
</details>






<details>
	<summary> Optimize placement using estimated wire length and capacitance</summary>

Optimizing placement using estimated wire length and capacitance is a critical step in the physical design flow of VLSI (Very Large Scale Integration) chip design. This process involves arranging standard cells on the chip layout in a way that minimizes the total wire length and the overall parasitic capacitance. <br>
-> Here's a detailed explanation of this optimization technique: <br>
**Wire Length Optimization:** <br>

*Definition*: Wire length optimization focuses on minimizing the total length of interconnect wires used to connect standard cells in the layout. Shorter wire lengths lead to reduced signal propagation delays, lower power consumption, and improved signal integrity. <br> <br>

*Importance*: <br>
    - Shorter interconnects reduce resistance and thus reduce RC (Resistance-Capacitance) delay, which is crucial for high-speed designs. <br>
    - Smaller wire lengths result in lower power consumption, as energy is dissipated as heat in the wires.<br>
    - Reducing wire lengths helps minimize area usage on the chip, potentially resulting in smaller and more cost-effective designs.<br><br>

*Techniques for Wire Length Optimization*: <br>
    - Clustering: Grouping related cells together can minimize wire lengths by reducing the distance signals need to travel. <br> 
    - Global Routing Algorithms: These algorithms determine the high-level routing of signals and attempt to minimize wire lengths. <br>
    - Timing-Driven Placement: Placement tools can be guided by timing constraints to minimize wire lengths for critical paths. <br><br>
    
**Capacitance Optimization:** <br>

*Definition*: Capacitance optimization aims to reduce the parasitic capacitance associated with interconnect wires and cell-to-cell connections. Parasitic capacitance can slow down signal transitions and increase power consumption. <br><br>

*Importance*: <br>
    - High parasitic capacitance can lead to longer signal delays, especially when combined with wire resistance (RC delay). <br>
    - Reducing capacitance can help improve the overall power efficiency of the chip. <br><br>

*Techniques for Capacitance Optimization*: <br>
     Wire Sizing: Increasing the width of interconnect wires can reduce their parasitic capacitance but may increase wire resistance. <br>
     Spacing and Layer Assignment: Optimizing the spacing between wires and the assignment of signal lines to different metal layers can reduce capacitance. <br>
     Shielding: Metal layers or shield layers can be added to reduce the coupling between nearby wires, mitigating capacitive coupling effects. <br><br>
     
**Integrated Optimization:** <br>

*Trade-offs*: Wire length and capacitance optimization often involve trade-offs. For example, reducing wire length may require using wider wires, which can increase capacitance. <br>
*Tools and Algorithms*: EDA (Electronic Design Automation) tools use various algorithms and optimization techniques to simultaneously consider both wire length and capacitance when performing placement. <br>



**Timing-Driven Placement:** <br>

Timing Constraints: In many cases, placement is guided by timing constraints. This means that cells are placed to meet required setup and hold times while also minimizing wire lengths and capacitance. <br>

**Iterative Process:** <br>

- Optimization using wire length and capacitance is often an iterative process. Placement tools may perform several iterations to improve placement quality based on feedback from routing and other stages of the design flow.<br><br>

- In summary, optimizing placement using estimated wire length and capacitance is essential for achieving high-performance and power-efficient VLSI chip designs. By carefully arranging standard cells, minimizing wire lengths, and reducing parasitic capacitance, designers can meet timing requirements, reduce power consumption, and enhance the overall efficiency of the integrated circuit. This optimization process is a critical part of the physical design flow in modern chip design.
<br>

- Repeaters and buffers play a significant role in maintaining signal integrity in VLSI (Very Large Scale Integration) system design. They are essential components that are strategically placed within the chip's layout to ensure that signals propagate correctly and reliably through long interconnects.<br>
**->Here's a detailed explanation of repeaters, buffers, signal integrity, and their placement in VLSI system design:** <br>
 
**Repeater and Buffer Definitions:** <br>

Repeater: A repeater is a digital logic element placed along a signal path to restore and amplify a signal, allowing it to travel over longer distances without distortion or loss of integrity. Repeaters are typically used for global or long-distance signals.<br>

Buffer: A buffer is a similar component to a repeater but is generally used to isolate and drive signals on different clock domains or within a local area. Buffers are often employed to deal with clock skew and to ensure that signals maintain their integrity when crossing clock domains.<br>

**Importance of Repeaters and Buffers:** <br>

Signal Integrity: As VLSI designs become more complex, signals need to traverse longer distances on the chip. Without repeaters or buffers, these signals can suffer from distortion, signal degradation, and timing violations, leading to functional errors.<br>

Mitigating Effects of RC Delay: Signals traveling through long interconnects experience RC (Resistance-Capacitance) delay due to the resistance of wires and the capacitance of the metal layers. Repeaters and buffers help mitigate the effects of RC delay by restoring signal levels and reducing the impact of capacitance.<br>

Clock Domain Crossing: Buffers are essential for handling signals that need to cross clock domains, ensuring that they maintain their integrity and are synchronized properly.<br><br>

**Placement of Repeaters and Buffers:** <br>

Strategic Placement: The placement of repeaters and buffers is critical and should be strategically planned based on the specific signal path requirements and the chip's floor plan.<br>

Global Signals: Repeaters are often used for global signals, such as clock distribution networks and data buses that span large areas of the chip. They are typically placed at regular intervals to boost signal strength and ensure synchronization.<br>

Local Buffers: Buffers are used for local signals that need to cross clock domains or travel short distances but may still require signal-level restoration.<br>

Timing Considerations: Placement should take into account timing constraints and signal arrival times to ensure that repeaters and buffers do not introduce additional delays.<br>

Power Considerations: While repeaters and buffers can improve signal integrity, they consume power. Careful consideration is needed to balance power consumption and signal quality.<br><br>

**Automated Placement Tools:** <br>

EDA (Electronic Design Automation) tools offer automated capabilities for placing repeaters and buffers. These tools consider the design's timing constraints, signal strengths, and other factors to optimize the placement.<br><br>

**Design Iterations:** <br>
 
The placement of repeaters and buffers often involves iterations, as the initial placement may need adjustments to meet timing and signal integrity requirements.<br>

In summary, repeaters and buffers are critical components in VLSI system design that help ensure signal integrity, particularly for long interconnects and when crossing clock domains. Proper placement and configuration of these components are essential for reliable and high-performance chip designs. They are key elements in addressing the challenges associated with signal propagation in modern, high-density integrated circuits.<br><br>
</details>



<details>
	<summary>Final Placement </summary>
	Final placement optimization and abutment are important stages in the physical design flow of VLSI (Very Large Scale Integration) chip design. These stages focus on refining the placement of standard cells to meet various design goals and constraints.<br>
	
*Here's detailed information about final placement optimization and abutment:* <br>
**Final Placement Optimization:** <br><br>

*Definition:* <br> Final placement optimization, often referred to simply as placement, is the process of determining the precise positions of standard cells on the chip layout. It comes after the initial placement stage and is a critical step in achieving design objectives.<br> <br>

*Objectives:* <br>
 
Minimize Wire Length: One of the primary goals is to minimize the total wire length of interconnections, as shorter wires reduce signal delays and power consumption. <br>
Address Timing Constraints: Final placement ensures that critical paths meet setup and hold time requirements.<br>
Optimize Area: Efficient use of chip area is essential, as it affects chip size, cost, and manufacturability.<br>
Manage Power: Proper placement can help distribute power efficiently and minimize voltage droop.<br>
Enhance Signal Integrity: Careful placement can reduce the risk of crosstalk and other signal integrity issues.<br><br>

*Optimization Techniques:*<br>
Placement algorithms are used to iteratively move cells to improve the overall placement quality while satisfying constraints.<br>
Methods include simulated annealing, genetic algorithms, and analytical placers.<br>
EDA (Electronic Design Automation) tools provide various options for placement optimization, often allowing designers to prioritize different objectives.<br><br>

*Timing-Driven Placement:*<br>

Timing constraints play a significant role in final placement optimization. Critical paths are identified, and cells are placed to minimize their delay.<br>
Slack is often used as a measure to determine if timing constraints are met.<br><br>

*Tools:*<br>

Commercial EDA tools provide advanced placement engines that use various algorithms and techniques to optimize placement while considering multiple objectives.<br><br>


**Abutment:** <br><br>

Definition:<br> Abutment, in the context of VLSI design, refers to the practice of aligning the edges of adjacent standard cells to minimize the space between them. It is particularly relevant for cells that have vertical or horizontal symmetry and can reduce the overall chip area.<br>
<br>
Importance:<br>

Abutment helps optimize chip area usage, as it minimizes unused space between cells.<br>
It simplifies the routing of interconnections by reducing the length of wires needed to connect adjacent cells.<br><br>

Types of Abutment:<br>
Vertical Abutment: Involves aligning the top and bottom edges of cells in adjacent rows.<br>
Horizontal Abutment: Involves aligning the left and right edges of cells in adjacent columns.<br>
Corner Abutment: Aligning the corners of adjacent cells can be used in certain cases.<br><br>

Design Considerations:<br>
The abutment is most effective when cells have compatible heights or widths.<br>
It may not always be possible or desirable, particularly for irregularly shaped cells or when it conflicts with other design goals.<br><br>

Abutment Tools:<br>
EDA tools often provide options for automatically abutting cells during the placement phase.<br><br>
In summary, final placement optimization and abutment are crucial steps in the physical design flow of VLSI chip design. These stages focus on refining the positions of standard cells to meet design objectives related to wire length, timing, area, power, and signal integrity. The abutment, in particular, can help optimize chip area usage by aligning the edges of adjacent cells, reducing unused space and simplifying interconnection routing. Both processes are instrumental in achieving high-performance and efficient chip layouts.
</details>




<details>
	<summary> Library Characterisation</summary>
	Library characterization is a critical step in the design of integrated circuits, and it involves characterizing the library of standard cells provided by a semiconductor foundry. <br>
	
 *--> Here's a brief explanation of the need for library characterization:*
 
**-Customization for Specific Process Technology:** Library characterization is necessary because standard cells need to be customized for a specific semiconductor manufacturing process. This process technology can vary from one foundry to another and even from one node to another within the same foundry. Characterization ensures that standard cells are tailored to work optimally within the parameters of the chosen process. <br>

**-Timing and Performance:** Different standard cells have unique timing characteristics and performance capabilities. Library characterization provides detailed information about the delay, power consumption, and other performance metrics of each cell under various operating conditions. This data is crucial for accurate timing analysis and optimization during the chip design process.<br>

**-Variability and Process Corner Analysis:** Semiconductor manufacturing processes exhibit variability, leading to variations in device characteristics and performance. Library characterization involves characterizing cells across various process corners (e.g., slow, typical, fast) to account for this variability. Designers use these models to ensure that the chip operates reliably under different conditions.
<br>

**-Power Analysis:** Accurate characterization includes modeling power consumption for different modes of operation (active, standby, sleep). This information helps designers estimate and manage power consumption during the chip's operation. <br>

**-Signal Integrity and Noise Analysis:** Library characterization also involves modeling the behavior of standard cells with respect to signal integrity and noise, allowing designers to assess and address issues related to crosstalk, signal quality, and noise margin.<br>

**-Advanced Design Techniques:** Library characterization supports advanced design techniques such as static timing analysis (STA), dynamic voltage and frequency scaling (DVFS), and low-power design methodologies. These techniques rely on accurate library data to optimize chip performance and power efficiency. <br>

**-Design Confidence:** Characterization data provides designers with the confidence that their designs will function correctly under real-world conditions. It allows for more accurate simulations, reducing the risk of design errors and costly design iterations. <br>

**-Compliance and Quality Assurance:** Many semiconductor foundries require library characterization to ensure that chip designs adhere to their process specifications and quality standards. It helps guarantee that chips manufactured in their processes will meet their performance and power consumption targets. <br>

In summary, library characterization is a necessary step in the VLSI design process. It provides designers with accurate models and data for standard cells, allowing them to design integrated circuits that meet performance, power, and reliability requirements while taking into account the intricacies of the specific semiconductor manufacturing process being used.<br><br>

</details>



<details>
	<summary>Congestion aware analysis </summary>
	
Congestion-aware placement is a critical aspect of VLSI (Very Large Scale Integration) chip design that focuses on optimizing the placement of standard cells while considering and mitigating congestion-related issues on the chip layout. Congestion refers to areas of the chip layout that experience high routing congestion, making it challenging to efficiently route wires and maintain signal integrity. <br> <br>

**--> Here's a detailed explanation of congestion-aware placement:** <br>
**- The Need for Congestion-Aware Placement:** <br>

As chip designs become more complex, routing congestion becomes a significant challenge. High congestion can lead to suboptimal layouts, increased wire length, longer delays, and reduced signal integrity.
Congestion can occur due to various factors, including high fanout nets, dense logic regions, and limited routing resources in specific areas of the chip. <br><br>

**- Key Objectives of Congestion-Aware Placement:** <br>

*Minimize Congestion:* The primary objective is to minimize congestion in the layout, ensuring that routing resources are efficiently utilized, and congestion hotspots are reduced or eliminated. <br>
*Optimize Timing:* Congestion-aware placement should maintain or improve timing characteristics by reducing wire delays and avoiding congested regions that might lead to timing violations.<br>
*Enhance Signal Integrity:* Proper placement can help reduce the risk of crosstalk and other signal integrity issues that can arise in congested areas.<br>
*Ensure Manufacturability:* Congestion-aware placement can also consider manufacturability factors, such as ensuring that there is enough space for manufacturing processes like lithography and etching.<br><br>

**- Techniques for Congestion-Aware Placement:** <br>

*Analytical Placers:* Advanced placement algorithms take into account congestion estimates and utilize mathematical models to optimize cell placement while avoiding congested regions. <br>
*Hierarchical Approaches:* Hierarchical placement techniques start with high-level block placement, which can be manually or automatically generated to minimize congestion. Then, finer-grained placement occurs 
 within each block, considering local congestion issues. <br>
*Global and Detailed Placement:* Global placement optimizes the placement of larger blocks, while detailed placement refines the position of individual cells to optimize for congestion and timing.<br>
*Congestion Estimation:* Estimating congestion during placement often involves computing congestion maps that identify regions of high congestion. This information guides placement optimization.<br>
*Iterative Refinement: Placement is an iterative process where cells are moved and repositioned based on congestion feedback. Iterations continue until placement objectives are met.<br>

**- Post-Placement Optimization:** <br>

After congestion-aware placement, additional optimization steps may be performed, such as global and detailed routing, to further improve routing and congestion issues. Congestion-aware routing algorithms can take advantage of placement information to make routing decisions that minimize congestion. <br><br>

**- EDA Tools:** <br>

 Commercial EDA (Electronic Design Automation) tools offer advanced placement engines that incorporate congestion-aware techniques and algorithms. These tools provide visualization of congestion maps and metrics to assist designers in identifying and addressing congestion issues. <br><br>

In summary, congestion-aware placement is a crucial step in VLSI chip design, aimed at optimizing cell placement while mitigating congestion-related problems. By considering routing resources, timing, signal integrity, and manufacturability, this technique helps ensure that chip designs meet performance goals and can be manufactured efficiently. Effective congestion-aware placement requires a combination of advanced algorithms, iterative refinement, and collaboration between designers and EDA tools.<br>
 
</details>



<details> 
        <summary> Cell Design and characterization flows </summary>
The cell design and characterization flow is a crucial process in VLSI chip design that involves creating, validating, and characterizing standard cells (logic gates) based on specific input parameters 
and requirements. 
	
**--> Below is an overview of the cell design and characterization flow, highlighting the inputs, design steps, and outputs:** <br>

**1. Inputs:** <br>
**PDKs (Process Design Kits):** <br>
- DRC (Design Rule Check): Specifies the design rules that must be followed for successful chip fabrication.<br>
- LVS (Layout vs. Schematic): Ensures the layout matches the intended circuit schematic.<br>
- SPICE Models: Provides accurate transistor-level electrical characteristics of the process technology.<br>
- Library: Contains pre-designed standard cells that may serve as templates.<br>
- User-Defined Specs: Specific requirements, such as speed, power, or area targets.<br>
- Cell Width and Height: Dimensions of the standard cell.<br>
- Metal Layers: Information on available metal layers and routing resources.<br>
- Pin Location: Defines the location of input and output pins.<br>
- Drawn Gate Length: The physical gate length specified by the technology node.<br><br>

**2. Design Steps:** <br>

**Circuit Design:** <br>
- Create the logical function of the standard cell using digital logic gates (NAND, NOR, AND, OR, etc.). <br>
- Define the internal structure, transistor sizes, and interconnections.<br>
- Ensure the cell meets user-defined specs (speed, power, area).<br>
Simulate the cell's behavior using SPICE or other circuit simulation tools.<br><br>

**Layout Design:** <br>
- Translate the logical circuit into a physical layout, adhering to the design rules from the PDK's DRC. <br>
- Place transistors, metal layers, and other components while optimizing for area and performance. <br>
- Ensure that the layout is compatible with the technology node's metal layers and routing resources. <br>
- Verify layout correctness using LVS tools. <br><br>

**Characterization:** <br>
- Extract SPICE models from the layout to represent the cell's electrical behavior. <br>
- Perform extensive simulation to characterize the cell under various conditions (timing, voltage, temperature).<br>
- Collect data on cell performance, including timing, power consumption, and noise margins.<br>
- Validate the cell's functionality and adherence to user-defined specs.<br><br>

**3. Outputs:** <br>

**CDL (Cell Description Language):** <br>
A text-based format that describes the cell's logical behavior, pin locations, and connectivity. <br>

**GDS (Graphic Data System):** <br>
A binary format representing the cell's physical layout, suitable for fabrication and chip assembly. <br>

**LEF (Library Exchange Format):** <br>
Contains information about the cell's physical characteristics, such as dimensions, pin locations, and metal layers, to aid in chip assembly and routing. <br>

**Extracted Spice Model:** <br>
A transistor-level SPICE model extracted from the layout, capturing the cell's electrical behavior.<br>

**Timing, Noise, Power Data:** <br>
Characterization results, including timing information (setup, hold times), noise margins, and power consumption data. <br>

**Libraries:** <br>
The standard cell library containing all characterized cells, is ready for use in chip design. <br>

**Function of PMOS & NMOS Network Paths:** <br>
Information about the logical and electrical behavior of the PMOS and NMOS transistor networks within the cell. <br>

In summary, the cell design and characterization flow involves transforming logical circuit descriptions into physically realizable layouts while adhering to design rules and meeting specific user-defined requirements. The outputs of this process are essential components in the larger chip design flow, enabling the efficient integration of standard cells into complex integrated circuits.<br><br>

Euler's path and stick diagrams are concepts used in the field of VLSI (Very Large Scale Integration) design, specifically in the layout and physical design of digital integrated circuits. <br>
*-> Let's explore both concepts:* <br>

**--> Euler's Path:** <br>

**Definition:** <br>
An Euler's path is a path in a graph that visits every edge (connection) exactly once and returns to the starting node. If such a path exists, the graph is called Eulerian. <br>

**Application in VLSI Design:** <br>
In VLSI design, circuits are often represented as graphs where nodes represent logic gates and edges represent the interconnections between gates. Euler's path concepts are applied to solve problems related to routing and connectivity in chip layouts. <br>

**Usage:** <br>
Euler's path algorithms help determine whether it is possible to route interconnections on a chip layout without conflicts, overlaps, or open-ended connections. If a chip layout can be represented as an Eulerian graph, it is easier to find a solution to routing problems. <br>


**--> Stick Diagram:** <br>

**- Definition:** <br>
A stick diagram is a graphical representation used in the initial stages of VLSI layout design. It represents the approximate layout of transistors and interconnections using simple shapes like rectangles, lines, and dots. <br>

**- Purpose:** <br>
Stick diagrams provide an abstract and high-level representation of a layout to quickly visualize the arrangement of transistors and connections without going into detailed geometries. They are particularly useful in the early stages of layout design when exploring various layout possibilities and ensuring that components fit within the chip area. <br>

**- Components:** <br>
In stick diagrams, rectangles or sticks typically represent transistors (NMOS or PMOS), lines represent metal interconnects, and dots indicate contacts or vias. <br>


**Benefits:** <br>
Stick diagrams facilitate rapid design exploration, allowing designers to assess the feasibility of a layout concept without diving into the complexities of detailed geometries. They aid in early-stage design decisions regarding area usage, placement of transistors, and routing strategies. <br>

**Limitations:** <br>

Stick diagrams are highly abstract and lack the level of detail needed for precise manufacturing and fabrication. Detailed layouts with exact dimensions and design rules are required for the final chip design.
<br>

**Evolution:**  <br>
Stick diagrams are often used as a starting point for more detailed representations, such as layout schematics and actual geometric layouts, as the design progresses. <br>

In summary, Euler's path concepts are applied in VLSI design to solve routing and connectivity problems, ensuring that interconnections in chip layouts are feasible. Stick diagrams, on the other hand, provide a high-level and abstract representation of layouts to aid in early-stage design exploration and decision-making, allowing designers to quickly visualize and assess layout possibilities. Both concepts are valuable tools in the field of VLSI design.<br><<br>

The characterization flow for timing, noise, and power in VLSI (Very Large Scale Integration) design is a crucial process that involves modeling and analyzing the electrical behavior of integrated circuits. --*-> Here's a brief overview of the typical characterization flow for these key parameters:* <br>

**1. Timing Characterization Flow:** <br>

**- Input:** <br>
Completed circuit layout. <br>
Library of standard cells with their electrical characteristics (e.g., delay models). <br>
Timing constraints (e.g., clock frequency, setup, and hold times). <br><br>

**- Steps:** <br>

*-Static Timing Analysis (STA):*

Perform a static timing analysis to calculate the worst-case and best-case delays through the combinational logic paths.<br>
Check if the design meets setup and hold time requirements.<br>
Identify critical paths and slack times.<br><br>

*- Transition Time Analysis:* <br>
Analyze the rise and fall times of signals at different points in the design. <br>
Ensure that signal transitions meet timing constraints.<br><br>

**Output:** <br>
- Timing reports containing delay information, critical paths, and slack times.<br>
- Data for ensuring that the design meets specified performance goals.<br><br>

**2. Noise Characterization Flow:** <br>

**- Input:** <br>
Completed circuit layout. <br>
Library of standard cells with their electrical characteristics. <br>
Noise constraints and specifications. <br>

**- Steps:** <br>
*Noise Analysis:* <br>
Analyze the impact of noise sources, such as crosstalk and power supply noise, on signal integrity. <br>
Estimate noise margins and evaluate the susceptibility of the design to noise-induced errors. <br>

*Crosstalk Analysis:* <br>
Identify nets and signal lines that are susceptible to crosstalk. <br>
Assess the impact of crosstalk on signal quality and timing. <br>

**- Output:** <br>
Reports on noise sources, noise margins, and crosstalk effects. <br>
Data for ensuring that the design maintains signal integrity and meets noise-related constraints. <br>

**3. Power Characterization Flow:** <br>

**- Input:** <br>
Completed circuit layout. <br>
Library of standard cells with power consumption models. <br>
Power constraints and specifications.<br><br>

**- Steps:** <br>

*Power Analysis:* <br>
Analyze dynamic power consumption due to switching activity in the design.<br>
Evaluate static (leakage) power consumption when the circuit is idle.<br>
Estimate total power consumption under various operating conditions.<br>

*- Low-Power Design Techniques:* <br>

Implement low-power design strategies such as clock gating, power gating, and voltage scaling.<br>
Evaluate the impact of these techniques on power consumption.<br><br>

**- Output:**
Reports on dynamic and static power consumption, including peak power and average power. <br>
Data for ensuring that the design meets power-related constraints and goals.<br><br>

In summary, the typical characterization flow for timing, noise, and power in VLSI design involves analyzing the electrical behavior of integrated circuits to ensure that they meet performance, noise, and power specifications. These characterizations are essential for validating and optimizing the design for reliable and efficient operation.<br>
</details>


## Day-17 Standard Cell Characterizations ##

<details>
 <summary>IO placer revised </summary>
 You can adjust the alignment of the Input/Output (I/O) pins by modifying the value of the FP_IO_MODE parameter. By default, this parameter is set to 1, but you can change it using the following command:

 ```ruby
set ::env(FP_IO_MODE) 2
```
After changing the mode following image is obtained.<br>
<img width="600" alt="fp_pin_uneven2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/fp_pin_uneven2.png"><br>

Below image is the zoomed version of above image.<br>
<img width="600" alt="fp_pin_uneven_zoom" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/fp_pin_uneven_zoom.png"><br>

Here you can observe that pins are place in uneven order.
</details>

<details>
 <summary>Spice Simulation lab for CMOS Inverter</summary>
	
 1. The initial step involves generating a SPICE Deck file that encompasses essential details, such as the netlist's connectivity information, specified input sources, and designated points for observing outputs. In the creation of this SPICE Deck, the process entails defining the interconnections among components, specifying component values, as well as recognizing and labeling nodes accordingly.
	
 2. A CMOS inverter is a digital logic gate that takes an input signal and produces an output signal that is the logical complement (opposite) of the input. In other words, when the input is high (1), the output is low (0), and when the input is low (0), the output is high (1).
  
 3. A CMOS inverter is constructed using complementary pairs of both NMOS (n-channel metal-oxide-semiconductor) and PMOS (p-channel metal-oxide-semiconductor) transistors. When one transistor is on (conducting), the other is off (non-conducting), allowing for low-power consumption and high noise immunity.
 
 4. A node is identified when a component is positioned between two nodes.

- The SPICE deck for CMOS inverter is as follows.

```ruby
M1 out in vdd vdd pmos W=0.375u L=0.25u
M2 out in 0 0 nmos W=0.375u W=0.25u
cload out 0 10f
Vdd vdd 0 2.5
Vin in 0 2.5
** Simulation Commands**
.op
.dc Vin 0 2.5 0.05
** .include tsmc_025um_model.mod **
.LIB "tsmc_025um_model.mod" CMOS_MODELS
.end
```

1. Component M1 represents a PMOS transistor with its drain connected to the OUT node, its gate linked to the IN node, and its substrate and source connected to VDD. M1 also features a specified width-to-length (W/L) ratio.
2. Component M2 represents an NMOS transistor with its drain linked to the OUT node, its gate connected to the IN node, and its substrate and source tied to the ground (0V). M2 also includes a defined W/L ratio.
3. The load capacitance, with a value of 10fF, is connected between the OUT node and ground. Likewise, the supply voltages, set at 2.5V, are connected between the ground and their respective nodes.
4. The Simulation command signifies the incremental variation of the gate voltage, ranging from 0V to 2.5V, in steps of 0.05V. This procedure is executed to observe and record the output characteristics concerning changes in the input voltage. The model file should be structured as follows, providing a comprehensive description of both NMOS and PMOS transistors, including their respective dimensions (length and width).

The layout of the CMOS inverter is as follows:<br>
<img width="600" alt="layout_inv" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_inv.png"><br>

Below image shows that poly is connected to PMOS and NMOS.<br>
<img width="600" alt="layout_inv" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_tckon(n%2Cp).png"><br>

Following commands are runned in tckon Main window.
```ruby
extract all
ext2spice cthresh 0 rthresh 0
ext2spice
```
The spice netlist generated as shown below.<br>
<img width="600" alt="spice_gen" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/spice_gen.png"><br>
</details>

<details>
 <summary>16 Mask CMOS Fabricaion</summary>

The manufacturing process involves several key steps:

1.Substrate Preparation: Commences with a silicon wafer as the initial material, which undergoes rigorous cleaning and pre-processing to prepare it for further stages.

2.Gate Oxide Formation (Mask 1): A thin layer of silicon dioxide (SiO2) is either grown or deposited onto the silicon wafer. This layer functions as the gate dielectric.

3.Polysilicon Gate Formation (Mask 2): Polysilicon is deposited and precisely patterned to create gate electrodes for both NMOS and PMOS transistors.

4.N-Well and P-Well Formation (Mask 3): The creation of regions for NMOS and PMOS transistors involves the use of n-type and p-type ion implantation processes.

5.Source and Drain Formation (Masks 4 and 5): Ion implantation, followed by annealing processes, is employed to define the source and drain regions of the transistors.

6.Gate Spacer and Silicidation (Masks 6 and 7): Insulating spacers are introduced around the gate structures, and metal silicide is formed on the source and drain regions to reduce contact resistance.

7.Interlayer Dielectric (ILD) Deposition (Mask 8): A layer of insulating material, typically silicon dioxide, is deposited and planarized to create a level surface for metal interconnections.

8.Contact and Via Formation (Masks 9 and 10): Etching processes create contact holes through the ILD, facilitating connections between metal interconnects and the underlying transistor nodes.

9.Metal Layer 1 (Mask 11): The formation of metal lines and interconnects allows for connections between different parts of the circuit.

10.Intermetal Dielectric (IMD) Deposition (Mask 12): Another insulating layer is deposited to provide separation between metal layers and isolation.

11.Metal Layer 2 (Mask 13): Additional layers of metal interconnects may be added as required.

13.Passivation Layer (Mask 14): A protective layer is deposited to shield the underlying layers and offer electrical insulation.

14.Pad Opening (Mask 15): Openings are created in the passivation layer to enable wire bonding or solder bump connections.

15.Testing and Packaging (Mask 16): Chips undergo rigorous testing for functionality and performance, followed by packaging to prepare them for their final use.

This comprehensive process forms the foundation of semiconductor device manufacturing, allowing for the creation of integrated circuits with intricate electronic functionalities.

***CMOS Inverter layout in Magic***

- When we select nmos and pmos box in Magic and run *what* command in tckon window we obtain below image.<br>
<img width="600" alt="layout_tckon(n%2Cp)" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_tckon(n%2Cp).png"><br>

- The connection of Y to both the drain terminals of the PMOS and NMOS transistors is depicted as illustrated in the figure.<br>
<img width="600" alt="layout_Y_con" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_Y_con.png"><br>
- The connections of the PMOS source and NMOS source are established as follows:<br>
<img width="600" alt="layout_NMOS_source" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_NMOS_source.png"><br>
<img width="600" alt="layout_PMOS_source" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_PMOS_source.png"><br>

- When we delete some layers we get drc errors same is illustrated in below image.<br>
<img width="600" alt="layout_Drc" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_Drc.png"><br>

- Below image is obtained after removing Drc Errors.<br>
<img width="600" alt="layout_inv" src="https://github.com/Sidv005/Samsung-PD-Training/blob/befa507f9dfa9062514315167655ed907184f0bf/SamsungPD_training/day3_openlane/layout_inv.png"><br>
</details>

<details>
 <summary>Labs on DRC</summary>
	
- Initially, it is necessary to duplicate the 'open_pdks.git' repository from RTimothyEdwards. Now all the magic files is with us. We will look for mtal3.mag. So metal3.mag file now with us.

- *cif see VIA2* command is runned in tckon window to obtain metal 3 contacts.
- When we see the layout of metal3.mag in Magic it is the same as shown below.<br>
<img width="600" alt="layout_metal3" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3d749d7d212dcf9f2c67be43a5160b9c3384e187/SamsungPD_training/day3_openlane/layout_metal3.png"><br>

- Now width and height of the box is shown in below image which determine distance between the metal contact and metal layer boundary. <br>
<img width="600" alt="layout_metal3_tckon" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3d749d7d212dcf9f2c67be43a5160b9c3384e187/SamsungPD_training/day3_openlane/layout_metal3_tckon.png"><br>

- Now poly.mag is loaded in Magic Following image shows the tckon window.<br>
<img width="600" alt="layout_poly_tckon" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3d749d7d212dcf9f2c67be43a5160b9c3384e187/SamsungPD_training/day3_openlane/layout_poly_tckon.png"><br>

- Below image of tckon window shows the width box in poly.<br>
<img width="600" alt="layout_poly_tckon_box" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3d749d7d212dcf9f2c67be43a5160b9c3384e187/SamsungPD_training/day3_openlane/layout_poly_tckon_box.png"><br>

- Now sky130A.tech file is edited by adding ***allpolynonres*** in poly.9. After editting we load the tech file and check drc using *drc check* in tckon window. This is shown in below image.<br> 
<img width="600" alt="tech_edit1_layout" src="https://github.com/Sidv005/Samsung-PD-Training/blob/3d749d7d212dcf9f2c67be43a5160b9c3384e187/SamsungPD_training/day3_openlane/tech_edit1_layout.png"><br>
- Here we can obsevre that no drc error is occuring. Hence we succesfully fixed poly.9 error. 
</details>











## Day-18 Pre timing Analysis and Importance of Good Clock Tree ##

<details>
 <summary>Steps to convert Grid into track info</summary>
	
 - Library Exchange Format (LEF) is a standard format used in the field of Very Large Scale Integration (VLSI) design. It is primarily used to describe the physical properties and characteristics of standard cells, macros, and other elements in a semiconductor library. 
- LEF files provide crucial information that is essential for the physical design and manufacturing processes of integrated circuits. LEF files are typically used in conjunction with Design Exchange Format (DEF), which describes the logical design of the circuit.
- LEF files describe the characteristics of individual cells or components within a semiconductor library.
- Here we are converting .mag files of inverter to .lef .

- The track info detail is as follows:<br>
<img width="600" alt="tracks_info" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/1.%20track%20info.png"><br>
- Now the grid is set as shown in the below figure.<br>
<img width="600" alt="tracks_info" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/2.%20Command%20G.png"><br>



1. Rule 1 : Input and output port should lie on the intersection of horizontal and vertical track

2. Rule 2 : The width of a standard cell should be odd multiple of the horizontal track pitch<br>
<img width="600" alt="grid_check" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/3.%20rule%201%20odd%20multiple.png"><br>

- Here we can observe that the width equals to 3 times the horizontal track pitch.
</details>

<details>
 <summary>Steps to convert magic layout to lef</summary>

- Save the layout with your name For e.g. sky130_siddhant

Then use the ***lef_write*** command this creates a .lef file

The following image shows the inclusion of the sky130_nihar.lef file in src.<br>
<img width="600" alt="src_content" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/4.%20can%20see%20mag%20file%20of%20my%20name%20is%20created.png"><br>

The contents of the .lef file are shown in the below image.<br>
<img width="600" alt="siddhant.lef" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/5.%20nihar_inv.lef%20.png"><br>

</details>

<details>
 <summary>Introduction to timing libs and steps to include lef cell</summary>

```ruby
cd ~/Desktop/work/tools/openlane_working_dir/openlane/vsdstdcelldesign
cp sky130_nihar_inv.lef ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/src
cd ~/Desktop/work/tools/openlane_working_dir/openlane/vsdstdcelldesign/libs
cp sky130_fd_sc_hd__* ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/src
cd ~/Desktop/work/tools/openlane_working_dir/openlane/designs/picorv32a/
vim config.tcl
```
The openLane start command for new cell:<br>
<img width="600" alt="config" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/6.%20openlane%20start%20command%20for%20new%20cell.png"><br>
run_synthesis command:<br>
<img width="600" alt="config" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/8.%20run_synthesis.png"><br>
The following image demonstrates how the custom cell is merged into the design during synthesis.<br>
<img width="600" alt="siddhant.lef_added" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/7.%20in%20synthesis%20we%20can%20it%20has%20taken%20my%20cell.png"><br>

- We can observe that the cell of our name is getting used.
</details>



<details>
 <summary>Introduction to Delay Table</summary>

- Clock gating is a power-saving technique in digital circuit design. It involves using control logic to disable the clock signal to specific circuit blocks when they are not in use. This reduces dynamic power consumption, and heat generation, and can extend battery life in low-power devices. An example of clock gating can be seen in the below image.<br>
<img width="600" alt="pic1_gating" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/pic1_gating.PNG"><br>

- For each level of buffering, we should have an identical buffer being used, and each node should be driving the same node.

- Keep in mind that the load at the output will vary, and since the load of one buffer is varying, the input transition of the following buffer will also vary.<br>
<img width="600" alt="pic2_gating" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/pic2_gating.PNG"><br>

The example of the delay table is as follows:<br>
<img width="600" alt="pic3" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/pic3.PNG"><br>

- Each type of cell will have its own individual delay table, as the internal pmos and nmos width/length ratio gets varied, the resistance changes, the RC constant gets varied as well, meaning the delay of each cell gets varied.
- The values of delay which are not available in the table are extrapolated based on the given data.
- If the Starting delay is 40 ps with C load as 50 pF the value will be between x9 and x10. As shown in the figure<br>

<img width="600" alt="pic4_gating" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/pic4_gating.PNG"><br>
The observations of the delay table are as shown in the figure<br>
<img width="600" alt="pic5" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/pic5.PNG"><br>
</details>

<details>
 <summary>Steps to configure synthesis settings to fix slack and include vsdinv</summary>
	
The various configurations of Synth are as follows

1. SYNTH_STRATEGY: control the area and timing
2. SYNTH_SIZING: control in cell sizing instead of buffering
3. SYNTH_BUFFERING: control if we want to buffer high fanout net
4. SYNTH_DRIVING_CELL: ensure more drive strength cells to drive input

In openlane
```ruby
echo $::env(SYNTH_STRATEGY)
set ::env(SYNTH_STRATEGY) "DELAY 0"
echo $::env(SYNTH_STRATEGY)
echo $::env(SYNTH_BUFFERING)
echo $::env(SYNTH_SIZING)
set ::env(SYNTH_SIZING) 1
echo $::env(SYNTH_SIZING)
echo $::env(SYNTH_DRIVING_CELL)
```
- With SYNTH_STRATEGY of Delay 0, the tool will focus more on optimizing/minimizing the delay, the index can be 0 to 3 where 3 is the most optimized for timing (sacrificing more area).
- SYNTH_SIZING of 1 will enable cell sizing where the cell will be upsized or downsized as needed to meet timing.<br>
<img width="600" alt="SET_STRATEGY1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/02ddba812831bd12ca3271a69608cf8c5ec1085f/SamsungPD_training/day4_final/SET_STRATEGY1.png"><br>

After modifying the configuration when we give run_synthesis<br>
<img width="600" alt="slack%3D-10(reduced)" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/10.%20slack%200%20after%20changing%20constraints%20.png"><br>
run_floorplan error command:<br>
<img width="600" alt="run_floorplan" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/11.%20floorplan%20error.png"><br>

When we give run_floorplan we get an error of macro placement so we need to comment the lines from flooplan.tcl.<br>
<img width="600" alt="run_floorplan" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/12.%20commenting%20from%20floorplan.tcl%20to%20solve%20error.png"><br>
Then when we run_floorplan it works<br>
<img width="600" alt="run_placement" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/13.%20run_floorplan.png"><br>
Then we need to give run_placement<br>
<img width="600" alt="run_placement" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/14.%20run_placement.png"><br>
Layout of my cell: <br>
<img width="600" alt="place_layout" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/15.%20layout%20of%20my%20cell.png"><br>
Can see my cell in layout:<br>
<img width="600" alt="place_layout" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/16.%20can%20see%20my%20cell%20in%20layout.png"><br>
</details>

<details>
 <summary>Setup Time analysis and flop setup time</summary>
	
*Setup Time (Ts) < Clock Period (T) - Combinational Delay (o)*

In this condition, Ts represents the minimum required time for the data to be stable before the clock edge arrives. The clock period T is the time between consecutive clock edges, and "o" is the combinational delay, which is the time taken by the logic between the data input and the flip-flop's clock input to process the data.

- This inequality ensures that there is sufficient time for the data to settle before the clock edge, preventing metastability or incorrect data capture in the flip-flop or latch.<br>
<img width="600" alt="pic_setup" src="https://github.com/Sidv005/Samsung-PD-Training/blob/48dc18c3c1d6a4345ce30928ae694884a256e207/SamsungPD_training/day4_final/pic_setup.PNG"><br>
<img width="600" alt="pic_setup2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/48dc18c3c1d6a4345ce30928ae694884a256e207/SamsungPD_training/day4_final/pic_setup2.PNG"><br>

**Clock Jitter and Uncertainity**
- Clock jitter, found in electronics and digital systems, denotes the deviation from the expected, regular timing of a clock signal.
- This irregularity can stem from multiple factors and is of significant concern in situations demanding precise timing, including high-speed digital communication, signal processing, and high-performance computing.

Consider the below example<br>
<img width="600" alt="jitter1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/48dc18c3c1d6a4345ce30928ae694884a256e207/SamsungPD_training/day4_final/jitter1.PNG"><br>

- In this context, we anticipate the clock signal to arrive precisely at the clock pin at either 0 seconds or at Ts. However, in practical situations, achieving exact timing can be challenging due to inherent variations in clock source generation. As a result, we need to adjust our understanding of combinational delay to accommodate the inherent uncertainty introduced by clock jitter.
- This means that the combinational delay becomes more critical and should consider the impact of clock jitter on timing requirements.<br>

<img width="600" alt="jitter2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/48dc18c3c1d6a4345ce30928ae694884a256e207/SamsungPD_training/day4_final/jitter2.PNG"><br>
</details>

<details>
 <summary>Steps to configure OpenSTA</summary>
- Firstly we have to write a pre_sta.conf file<br>
<img width="600" alt="pre_sta_conf" src="https://github.com/Sidv005/Samsung-PD-Training/blob/65a532a682167581f10bdfb2c7c311cb7c2f8446/SamsungPD_training/day4_final/pre_sta_conf.tcl.PNG"><br>
can see the slack met after pre_sta.conf<br>
<img width="600" alt="pre_sta_conf" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/17.%20can%20see%20the%20slack%20met%20after%20in%20pre_sta.conf%20.png"><br>	
- Then we need to run sta pre_sta.conf<br>
<img width="600" alt="pre_sta_conf" src="https://github.com/Sidv005/Samsung-PD-Training/blob/65a532a682167581f10bdfb2c7c311cb7c2f8446/SamsungPD_training/day4_final/pre_sta.png"><br>
- New verilog (.v):<br>
<img width="600" alt="pre_sta_conf" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/17.%20new%20verilog.v%20.png"><br>	
</details>

<details>
 <summary>Clock Tree Synthesis TritconCTS and signal integrity</summary>
	
- Now we need to use the below commands in openlane<br>
```ruby
run_cts
```

- run_cts:<br>
<img width="600" alt="(run_cts)" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/19.%20run_cts.png"><br>


*Verifying the CTS design*

- Use the below commands in openlane
```ruby
echo $::env(LIB_TYPICAL)
echo $::env(CURRENT_DEF)
echo $::env(CTS_MAX_CAP)
echo $::env(CTS_CLK_BUFFER_LIST)
echo $::env(CTS_ROOT_BUFFER)
```

<img width="600" alt="(verify_cts)" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/20.%20cts_verification.png"><br>

</details>

<details>
 <summary>Timing Analysis with real clocks</summary>

Executing these commands in OpenLANE:
```ruby
openroad                                                                                                       
read_lef designs/picorv32a/runs/13-01_14-09/tmp/merged.lef
read_def designs/picorv32a/runs/13-01_14-09/results/cts/picorv32a.cts.def
write_db pico_cts.db
read_db pico_cts.db
read_verilog designs/picorv32a/runs/crct2/results/synthesis/picorv32a.synthesis_cts.v
read_liberty -max $::env(OPENLANE_ROOT)/designs/picorv32a/src/sky130_fd_sc_hd__slow.lib
read_liberty -min $::env(OPENLANE_ROOT)/designs/picorv32a/src/sky130_fd_sc_hd__fast.lib
set_propagated_clock [all_clocks]
read_sdc designs/picorv32a/src/my_base.sdc
report_checks -path_delay min_max -format full_clock_expanded -digits 4
```
These are the outputs of the above commands shown in below figure.<br>
<img width="600" alt="(openroad_commands)2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/65a532a682167581f10bdfb2c7c311cb7c2f8446/SamsungPD_training/day4_final/(openroad_commands)2.png"><br>

From the below image we can observe that min slack is met.<br> 
<img width="600" alt="min_slack" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/22.%20min_violated.png"><br>
Max is violating<br>
<img width="600" alt="max_slack" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/21.%20max_violated.png"><br>

***Steps to execute STA with right timing library***

In order to meet the max slack we follow the below commands:-
```ruby
exit        (Exit openroad)
openroad
read_db pico_cts.db
read_verilog /openLANE_flow/designs/picorv32a/runs/13-01_14-09/results/synthesis/picorv32a.synthesis_cts.v
read_liberty $::env(LIB_SYNTH_COMPLETE)
link_design picorv32a
read_sdc designs/picorv32a/src/my_base.sdc
set_propagated_clock [all_clocks]
report_checks -path_delay min_max -fields {slew trans net cap input pin} -format full_clock_expanded
echo $::env(CTS_CLK_BUFFER_LIST)
```
Following the verification of checks in the report, we observe that both the minimum and maximum requirements have been satisfied.<br>
<img width="600" alt="slack_met1" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/24.%20met_hold_kargaye.png"><br>
<img width="600" alt="slack_met2" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/23.%20met_kargaye.png"><br>

*Steps to observe impact of bigger CTS buffers on setup and hold timing*

Initially, we need to execute these commands in OpenLANE. In this process, we are converting the current DEF (Design Exchange Format) file to a placement-specific DEF file.
```ruby
exit 
echo $::env(CTS_CLK_BUFFER_LIST)
set ::env(CTS_CLK_BUFFER_LIST) [lreplace $::env(CTS_CLK_BUFFER_LIST) 0 0]
echo $::env(CURRENT_DEF)
set ::env(CURRENT_DEF) /openLANE_flow/designs/picorv32a/runs/13-01_14-09/results/placement/picorv32a.placement.def
run_cts
```
The output of the above commands is shown below.<br>
<img width="600" alt="commands1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/d3a9c83fc1937f943217921722ab4623f4ef7e89/SamsungPD_training/day4_final/commands1.PNG"><br>

In OpenLANE, these commands must be executed to assess the effect of large buffers. In this case, we are solely focused on timing analysis by loading the DEF, LEF, and cts.v files.<br>
```ruby
open road
read_lef /openLANE_flow/designs/picorv32a/runs/13-01_14-09/tmp/merged.lef
read_def /openLANE_flow/designs/picorv32a/runs/13-01_14-09/results/cts/picorv32a.cts.def
write_db pico_cts1.db
read_db pico_cts1.db
read_verilog /openLANE_flow/designs/picorv32a/runs/13-01_14-09/results/synthesis/picorv32a.synthesis_cts.v
read_liberty $::env(LIB_SYNTH_COMPLETE)
link_design picorv32a
read_sdc designs/picorv32a/src/my_base.sdc
set_propagated_clock [all_clocks]
report_checks -path_delay min_max -fields {slew trans net cap input pin} -format full_clock_expanded
```

run_cts:<br>
<img width="600" alt="commands1" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/25.%20run_cts.png"><br>
We can see slack has met now:<br><br>
<img width="600" alt="commands1" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-18/26.%20slack%20met.png"><br>
</details>





## Day-19 Final Step RTL to GDSII ##
<details>
 <summary>Introduction to maze Routing use Lee's Algorithm</summary>

***Routing***

Routing in the context of VLSI (Very Large Scale Integration) pertains to the intricate task of establishing connections among different elements within an integrated circuit, including transistors, logic gates, and various electronic components. This is achieved by creating an intricate network of interconnected wires or metal layers. The quality and efficiency of routing are of paramount importance as they directly impact the performance and functionality of VLSI chips. VLSI routing primarily consists of two main categories: global routing and detailed routing.

***Maze Routing Lee's Algorithm***

The Lee algorithm, which is sometimes referred to as the Lee-Moore algorithm, is a widely employed pathfinding or maze routing technique within the realm of computer science, notably in the domains of VLSI design and printed circuit board (PCB) design. Its primary function is to determine the most efficient route between two points on a grid or maze while accounting for obstacles or obstructed areas. This algorithm operates on a breadth-first search (BFS) principle and is frequently utilized during the intricate routing phases in VLSI design.

<img width="800" alt="pic1" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7d341dd1400516ddbd940e228b96f016f0c1eda5/day19/pic1.PNG"><br>

The procedural steps in Lee Algorithm is as follows. 

*Initialization :*

To prepare for the pathfinding process, begin by establishing a grid or maze where each cell has two potential states: it can either be unoccupied (open) or obstructed. Designate one of these cells as the starting point, denoting it as the source cell, and choose another cell as the destination point, which will serve as the target cell. Next, create a queue data structure to keep track of the cells that need to be examined during the exploration.

*Breadth-First Search :*

Commence by taking the source cell and placing it into the queue.
Assign a step count of 0 to the source cell.
Initiate a loop that will continue as long as there are cells in the queue.
For each cell within the queue:

- Examine the adjacent cells in all four directions (up, down, left, and right). Ensure that these neighboring cells are unobstructed and haven't been visited yet.
- If a neighboring cell is unvisited, mark it as visited, enqueue it, and set its step count as the current cell's step count incremented by one.
- Continue this process until the destination cell is reached or until there are no more cells to explore.

*Backtracking :*

Upon reaching the destination cell, the algorithm can backtrack its steps from the destination back to the source. This is achieved by inspecting neighboring cells and selecting the one with a shorter distance value at each stage, effectively retracing the shortest path from the destination to the source.

*Path Construction:*

- Following the backtracking process, the algorithm reconstructs the path from the source to the destination, ultimately determining the shortest route.

- The Lee algorithm holds particular significance in the context of detailed routing for VLSI design. This is because it excels in identifying the shortest path, all while considering the grid's layout and potential obstacles. It offers an efficient means to navigate around hindrances, steer clear of congestion, and establish connections between different elements on an integrated circuit.

<img width="600" alt="pic2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7d341dd1400516ddbd940e228b96f016f0c1eda5/day19/pic2.PNG"><br>

<img width="800" alt="pic3" src="https://github.com/Sidv005/Samsung-PD-Training/blob/7d341dd1400516ddbd940e228b96f016f0c1eda5/day19/pic3.PNG"><br>

The Lee algorithm boasts a notable advantage in that it assures the discovery of the shortest path. Nevertheless, it should be noted that its memory requirements can be substantial, and it may become computationally demanding when dealing with sizable grids or mazes. To mitigate these constraints, a variety of adaptations and enhancements have been developed. These include the bidirectional Lee algorithm, the A* algorithm, and hierarchical iterations tailored for PCB routing, all of which aim to optimize and refine the original Lee algorithm.
</details>

<details>
 <summary>Design Rule Checks</summary>

- Design Rule Checks (DRC) play a pivotal role in the integrated circuit (IC) design and manufacturing workflow, particularly in the realm of Very Large Scale Integration (VLSI) design.

- DRC encompasses a series of directives and assessments employed to verify that the IC's layout complies with both manufacturing and design standards. These standards are indispensable in ensuring the successful manufacturing of the IC and its subsequent performance in alignment with the intended specifications.

Some of the Design Rule checks are illustrated in the below figure.<br>
<img width="600" alt="pic4" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8628a922c6bd7c820ab305342bfe1355a0010711/day19/pic4.PNG"><br>
- A signal short, classified as a DRC violation, occurs when two wires that shouldn't be connected inadvertently make contact on the same layer. Such an occurrence can potentially result in functional failures, necessitating prompt attention.

- To resolve this issue, a straightforward solution involves relocating one of the wires to a separate metal layer. It's essential to bear in mind that this adjustment must adhere to any new DRC rules that have been introduced.
  
<img width="600" alt="pic5" src="https://github.com/Sidv005/Samsung-PD-Training/blob/8628a922c6bd7c820ab305342bfe1355a0010711/day19/pic5.PNG"><br>

- Conducting parasitic extraction involves the retrieval of resistance and capacitance values associated with the wires, which will subsequently be applied in downstream procedures.
  </details>

  <details>
 <summary>Labs</summary>

To run OpenLANE following commands are executed.
```ruby
cd work/tools/openlane_working_dir/openlane
make mount
pwd
ls -ltr
./flow.tcl -interactive
package requires openlane 0.9
prep -design picorv32a -tag 13-01_14-09
```
In OpenLANE
```ruby
echo $::env(CURRENT_DEF)    (Ensure current_def is on the CTS stage)
gen_pdn                     (To generate power distribution network)
```

The below images illustrate the occurrence of errors when the above commands are run.<br>
<img width="600" alt="route_pic7" src="https://github.com/Sidv005/Samsung-PD-Training/blob/799df10e787d03f566a7e068394ae1f66348237e/day19/route_pic7.PNG"><br>
<img width="600" alt="route_pic8" src="https://github.com/Sidv005/Samsung-PD-Training/blob/799df10e787d03f566a7e068394ae1f66348237e/day19/route_pic8.PNG"><br>

***Fundamentals of global and detail routing and configure TritonRoute***

```ruby
echo $::env(CURRENT_DEF)            (Ensure the def file of pdn has been created)
echo $::env(ROUTING_STRATEGY)
set ::env(CURRENT_DEF) <path_of_cts.def>
run_routing
```

Executing the "run_routing" command yields the following result:<br>
<img width="600" alt="route_pic9" src="https://github.com/Sidv005/Samsung-PD-Training/blob/799df10e787d03f566a7e068394ae1f66348237e/day19/route_pic9.PNG"><br>

The below screenshot shows the results folder.<br>
<img width="600" alt="route_pic10" src="https://github.com/Sidv005/Samsung-PD-Training/blob/799df10e787d03f566a7e068394ae1f66348237e/day19/route_pic10.PNG"><br>

</details>









## Day-20 Floorplanning and power planning labs ##
<details>
 <summary>Theory</summary>
	The physical design flow in VLSI (Very Large Scale Integration) is a series of steps that transform a high-level hardware description of a digital circuit into a physical layout that can be fabricated as an integrated circuit (IC) on a semiconductor wafer. This flow involves several stages and a range of tools and methodologies. Here is an overview of the typical steps in the physical design flow:

1. Design Specification: This is the initial step where you gather requirements and specifications for the digital circuit. It includes understanding the functionality, power consumption, performance, area constraints, and other design goals.

2. RTL Design: Register Transfer Level (RTL) design involves creating a high-level representation of the digital circuit in a hardware description language (HDL) like VHDL or Verilog. The RTL description typically consists of flip-flops, registers, and the interconnections between them.

3. Logic Synthesis: This step involves converting the RTL description into a gate-level representation. Logic synthesis tools map the RTL to a library of standard cells, optimizing for area, power, and speed while meeting the design constraints.

4. Floor Planning: In this phase, you decide on the placement of different functional blocks and macros on the chip. It involves defining the size and location of each block to optimize for area, power, and signal routing.

5. Power Planning: Power distribution networks are designed to ensure that all parts of the chip receive a stable and adequate power supply. This includes the design of power grids and voltage regulation circuits.

6. Placement: The placement stage determines the physical locations of each standard cell on the chip. Tools aim to minimize wirelength, optimize for timing, and meet other design constraints.

7. Clock Tree Synthesis (CTS): CTS is the process of designing a clock distribution network to ensure that clock signals reach all the flip-flops and latches with minimal skew and low power consumption.

8. Routing: The routing step involves creating the physical wires (metal layers) that connect the gates, ensuring that all connections meet design requirements and constraints. Global and detailed routing are usually performed.

9. Design for Manufacturing (DFM): DFM considerations address manufacturability issues like lithography, etching, and other process-related aspects to ensure the chip can be manufactured with high yield.

10. Design Verification: Extensive verification is carried out at each stage of the physical design flow to ensure that the final layout adheres to the original design specifications and that it is free from logical and physical errors.

11. Physical Verification: This involves checking the design against manufacturing rules, including design rule checking (DRC) and layout vs. schematic (LVS) checks.

12. Extraction: Parasitic capacitances and resistances are extracted from the layout and included in the simulation models to accurately predict circuit behavior.

13. Sign-off: This is the final review and approval stage before tape-out, where the design is deemed ready for fabrication.

14. Tape-out: Once the design is thoroughly reviewed, validated, and optimized, it is sent for semiconductor fabrication. A set of files representing the design layout is created and submitted to the foundry.

15. Post-Tapeout Tasks: After fabrication, there may be additional tasks such as package design, testing, and assembly before the final IC is ready for use.

The physical design flow in VLSI is a complex and iterative process that requires careful planning and the use of various EDA (Electronic Design Automation) tools. Success in physical design depends on meeting the design goals and constraints while optimizing for power, area, and performance.
</details>

<details>
 <summary>Labs</summary>
	
```ruby
git clone https://github.com/manili/VSDBabySoC.git
git clone https://github.com/Devipriya1921/VSDBabySoC_ICC2.git
git clone https://github.com/bharath19-gs/synopsys_ICC2flow_130nm.git
git clone https://github.com/kunalg123/icc2_workshop_collaterals.git
git clone https://github.com/google/skywater-pdk-libs-sky130_fd_sc_hd.git
git clone https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git
```

 ```ruby
gvim vsdbabysoc.tcl &
gvim avsdpll.lib &
```

*vsdbabysoc.tcl*
- Modifying the contents to my path, remove -lib in read_lib commands, and replace MYCLK to clk since the clock used in the design is {clk}
- All of the commands have been inserted in gvim and the tool will run it once at a time.<br>
<img width="800" alt="1.vsdbabysoc.tcl" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/1_vadbabysoc_tcl.png"><br>
<img width="800" alt="1.vsdbabysoc.tcl" src=""><br>



 *avsdpll.lib*
 
- Remove the unwanted pins<br>
<img width="800" alt="3.avsdpll.lib" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/3_avsdpll_lib.png"><br>

```ruby
dc_shell
source vsdbabysoc.tcl
```

-sourcing that tcl file:<br>
<img width="800" alt="3.avsdpll.lib" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/4_source.png"><br>
***Reports***

Report timing image is shown below.<br>
<img width="800" alt="pic3_timing" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/8_report_timing.png"><br>

Report area image is shown below.<br>
<img width="800" alt="pic4_area" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/6_report_area.png"><br>

Report power image is shown below.<br>
<img width="800" alt="pic5_power" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/7_report_power.png"><br>

Report constraints:<br>
<img width="800" alt="pic5_power" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/9_report_constraint.png"><br>


***Output schematic***<br>
<img width="800" alt="sche_pic1" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/10_report_gui.png"><br>
<img width="800" alt="sche_pic1" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/11_report_gui.png"><br>
<img width="800" alt="sche_pic1" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/12_report_gui.png"><br>
<img width="800" alt="sche_pic1" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/13_report_gui.png"><br>
<img width="800" alt="sche_pic1" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/14_report_gui.png"><br>
<img width="800" alt="sche_pic1" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/15_report_gui.png"><br>
*RVMYTH core*<br>
<img width="800" alt="sche_pic2" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/sche_pic2.png"><br>

***Performing physical design***

```ruby
gvim top.tcl
gvim icc2_common_setup.tcl
gvim icc2_dp_setup.tcl
gvim init_design.read_parasitic_tech_example.tcl
gvim init_design.mcmm_example.auto_expanded.tcl
gvim pns_example.tcl
```
*Modifying files*

1. top.tcl<br>
<img width="800" alt="3.top.tcl" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/16_top_TCL.png"><br>
<img width="800" alt="3.top.tcl" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/17_top_TCL.png"><br>
<img width="800" alt="3.top.tcl" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/18_top_TCL.png"><br>

2. icc2_common_setup.tcl<br>
<img width="800" alt="4.icc2_common.tcl" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/19_icc2_commom.png"><br>
<img width="800" alt="4.icc2_common.tcl" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/20_icc2_commom.png"><br>

3. icc2_dp_setup.tcl<br>
<img width="800" alt="5.icc2_dp.tcl" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/21_icc2_dp_setup.png"><br>

4. init_design.read_parasitic_tech_example.tcl<br>
<img width="800" alt="6.init_example.tcl" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/22_example_tcl.png"><br>
 
5. init_design.mcmm_example.auto_expanded.tcl<br>
<img width="800" alt="7.init_expanded.tcl" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/23_expanded_tcl.png"><br>

6. pns_example.tcl<br>
<img width="800" alt="8.pns_ex.tcl" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/24_pns_example.png"><br>

**Observing for utilization**

***Output Layout***

```ruby
source top.tcl
```

<img width="800" alt="pic7_floorplan_plac" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/25.%20run%20completed.png"><br>

gui run completed
<img width="800" alt="pic8_chip" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/26.%20gui_run%20completed.png"><br>

Below screenshot displays the timing report showing slack = -5.31. <br>
<img width="800" alt="pic9_40%25_before_propagated" src="https://github.com/Sidv005/Samsung-PD-Training/blob/5867dee56a51d6d04d937d6db09f9af1480ebff6/day20/pic9_40%25_before_propagated.png"><br>


-pll_dac :<br>
<img width="800" alt="pic13_40-50%25violators" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/77ca6e75034f22aa71437cadaf8257b75e31fcb2/DAY-20/27.%20pll_dac.png"><br>


</details>









## Day-21 Placement and CTS labs ##
<details>
 <summary>Theory</summary>

1. Placement in IC design refers to the vital process of determining the physical locations of electronic components within an integrated circuit (IC). This step is of paramount importance in the overall IC design process, as it significantly impacts the final performance, power consumption, and manufacturability of the chip. The primary objective of placement is to allocate a physical position for each logic gate, flip-flop, or other components on the chip, with the goal of minimizing wirelength, reducing congestion, and optimizing factors like signal delay and power consumption.

2. Routing in VLSI design involves the task of interconnecting various components, such as logic gates and flip-flops, placed on an integrated circuit (IC) with the necessary wires or interconnects. The primary goal of routing is to establish an efficient and reliable network of connections between these components on the chip. This network must meet timing constraints, minimize wirelength, and alleviate congestion issues.

3. Clock Tree Synthesis (CTS) is a critical phase in the design of digital integrated circuits, particularly those featuring synchronous logic, such as microprocessors and application-specific integrated circuits (ASICs). The primary purpose of CTS is to create a well-organized and optimized distribution network for clock signals, ensuring that all sequential elements, such as flip-flops, receive clock signals with minimal skew, low latency, and low power consumption.
</details>

<details>
 <summary>Labs</summary>
	
**Observing for 40% of utilization**


Script in top.tcl

1. create_placement is used to create placement for the design. floorplan option is selected to make the design planning styled as placement.
2. Pin Placement is done by sourcing pns.tcl to sync with the current technology file regarding power grid creation.<br>
<img width="800" alt="pic1_create_placement" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/1_clock_leaves.png"><br>

<img width="800" alt="pic2_create_placement" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/2_clock_tree.png"><br>
<img width="800" alt="pic2_create_placement" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/2_clock_treepng"><br>
*Reports that were generated from the run*

```ruby
gvim check_design.pre_pin_placement
```
As shown in below figure there are 3 warnings in total for pre-placement while checking the design.
<img width="800" alt="pic3_pre_placement_warnings" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/4check_desinpng"><br>

```ruby
gvim report_port_placement.rpt
```
Below image shows the report_port_placement.<br>
<img width="800" alt="pic4_report_port_placement.rpt" src="<img width="800" alt="pic3_pre_placement_warnings" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/5check_design.png"><br>"><br>


```ruby
gvim vsdbabysoc.post_estimated_timing.rpt
```
Below image shows the report of vsdbabysoc.post_estimated_timing <br>
<img width="800" alt="pic7_post_estimated_timing.rpt" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/9estimated_timing.rpt.png"><br>



```ruby
gvim vsdbabysoc.post_estimated_timing.qor
```
Below image shows the qor report of vsdbabysoc.post_estimated_timing_qor<br>
<img width="800" alt="pic8_post_estimated_timing.qor" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/6%20timing.qor.png"><br>
<img width="800" alt="pic9_post_estimated_timing.qor2" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/7%20timing.qor1.png"><br>

From above image we can observe that Post estimated timing qor shows there is no violating path reported with 61 nets having violations, 58 max trans violations, and 61 max cap violations.

```ruby
gvim vsdbabysoc.post_estimated_timing.qor.sum
```

Below image shows the summary on qor report of vsdbabysoc.post_estimated_timing_sum <br>
<img width="800" alt="pic10_post_estimated_timing.qor.sum" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/8iming.qor.sum.png"><br>

Placement Analysis:-<br>
<img width="800" alt="pic11_pll_schematic" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/10%20placement.png"><br>

top.tcl <br>
<img width="800" alt="pic12_chip_schematic" src="https://github.com/gohilnihar07/Samsungpdtraining/blob/69030f1d2a865563907b0a8e9f0cdce67bb7de91/day-21/11%20top.tcl.png"><br>
 </details>






