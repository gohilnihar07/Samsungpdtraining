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
	When we try to synthesize it, it shows<br>
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
	<summary> Combinational logic optimization techniques and It's examples </summary>
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
It's important to note that optimization can involve trade-offs between different design parameters like area, power, timing, etc. So designers need to consider their specific requirements and constraints to strike the right balance<br>
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

       4. opt_chcek4<br>
	  --> Verilog code for design opt_check4,<br>
	     <img width="600" alt="netlist" src=""><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src=""><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src=""><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src=""><br><br>

       5. multiple_module_opt<br>
	  --> Verilog code for design multiple_module_opt,<br>
	     <img width="600" alt="netlist" src=""><br>
          --> Circuit diagram and expecting optimize result,<br>
	     <img width="600" alt="netlist" src=""><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src=""><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src=""><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src=""><br><br>

       6. multiple_module_opt2<br>
	  --> Verilog code for design multiple_module_opt2,<br>
	     <img width="600" alt="netlist" src=""><br>
          --> Circuit diagram and expecting optimize result,<br>
	     <img width="600" alt="netlist" src=""><br>
	  --> statistics,<br>
	     <img width="600" alt="netlist" src=""><br>
	  --> Graphical representation after mapping,<br>
	     <img width="600" alt="netlist" src=""><br>
	  --> Generated netlist,<br>
	     <img width="600" alt="netlist" src=""><br><br>
</details>
