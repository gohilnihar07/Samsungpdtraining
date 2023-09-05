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

<details>
	<summary> Basics of DFT </summary>
</details>
--> Testability:-<br>
In VLSI terms,<br>
it means "if a design is well-controllable and well-observable it is said to easily testable."
<br><br>

What is DFT?<br>
It is a technique which facilitates a design to become testable after prooduction.Adding an extra design for an existing design to make sure it can be tested after being fabricated. "or" in other words Testability features are designed into the chip during its design phase to enable efficient testing. These features help in detecting manufacturing defects, design errors, and other issues that might affect the chip's performance or reliability.<br>
A few saples of designs included for making the whole chip tetstable. For example,
<br><br>
--> For macros, we including MBIST logic,<br>
  Design for Testability (DFT) techniques play a crucial role in ensuring that complex macros (large functional blocks) within a chip can be effectively tested for faults. These macros can include memory blocks, processors, and other specialized components. DFT for macros often involves the incorporation of Memory Built-In Self-Test (MBIST) logic.<br>
  Memory Built-In Self-Test (MBIST) is a DFT technique specifically designed for testing memory arrays within integrated circuits. It involves adding dedicated circuitry to the memory block that enables the memory to be tested using built-in self-test patterns. This eliminates the need for external test equipment and simplifies the testing process.<br><br>

--> For flops, we will use SCAN chains,<br>
 The SCAN chain (also known as Scan Path) technique is a fundamental Design for Testability (DFT) methodology used to improve the testability of digital circuits, particularly sequential elements like flip-flops. It allows for efficient testing of the internal logic states of flip-flops by serially shifting in test patterns and shifting out responses, thereby simplifying the process of observing and controlling the states of these elements during testing.<br>

Here's how the SCAN chain technique works for flip-flops in DFT:<br><br>

   - Basic Concept:<br>
        In a traditional digital circuit, the primary inputs and outputs are connected to the external pins, and the internal states of flip-flops are not directly accessible.<br>
        In the SCAN chain technique, additional circuitry is introduced to create a chain of flip-flops that can be connected in a serial manner.<br><br>

   - Scan-In and Scan-Out (SI and SO) Ports:<br>
        Each flip-flop is augmented with two additional ports: Scan-In (SI) and Scan-Out (SO).<br>
        During normal operation, the SI and SO ports are disconnected, and the flip-flops behave like regular sequential elements.<br>
        During testing, the SI and SO ports are connected to the adjacent flip-flops, forming a serial shift register.<br><br>

   - Test Mode:<br>
        The circuit enters the test mode by configuring control signals to activate the SCAN chain. This isolates the flip-flops from the normal logic and enables the shift-register behavior.<br>
        The initial values of the flip-flops are loaded into the chain through the SI port.<br><br>

   - Shifting Test Patterns:<br>
        Test patterns, which represent the desired inputs for the circuit, are loaded into the SCAN chain through the SI port. These patterns are serially shifted from flip-flop to flip-flop.<br><br>

   - Observing Responses:<br>
        As the test patterns propagate through the SCAN chain, the responses (expected outputs) are observed at the SO port.<br>
        These responses are then compared to the expected results to identify any faults or defects.<br><br>

    - Benefits:<br>
        The SCAN chain technique provides full controllability and observability of internal flip-flop states, enabling comprehensive testing of sequential logic.<br>
        It simplifies the process of applying test patterns and capturing responses, reducing the need for complex external test equipment.<br>
        Faults related to flip-flops, such as stuck-at faults or transition faults, can be efficiently detected and diagnosed.<br><br>

   - Trade-offs:<br>
        Introducing the SCAN chain requires additional circuitry, which can lead to increased chip area and potential performance overhead.<br>
        The test mode might not perfectly emulate the actual operating conditions, so certain faults might still remain undetected.<br><br>

The SCAN chain technique is a widely used DFT methodology and is supported by many industry-standard tools and methodologies. It greatly enhances the testability of digital circuits containing numerous sequential elements, like flip-flops, ensuring that the manufactured chips are of high quality and reliability.<br><br><br>


--> For combinational circuit, we will generate test patterns,<br>
for combinational circuits, we generate and apply test patterns to verify the correctness of their functionality. Combinational circuits are digital circuits where the outputs depend solely on the current inputs, with no memory or feedback elements. Testing combinational circuits involves creating input patterns that exercise various input combinations to detect faults or errors in the circuit's logic.<br>

Here's how the process of generating test patterns for testing combinational circuits typically works:<br><br>

    - Fault Models: First, you need to define the types of faults you want to detect in the combinational circuit. Common fault models include stuck-at faults (where a signal is stuck at either logic high or logic low), transition faults (where a signal fails to transition within a specific time), and bridging faults (where two signal lines are shorted together).<br><br>

    - Test Generation Algorithms: Various algorithms exist to automatically generate test patterns to detect different fault models. These algorithms analyze the circuit's logic and structure to generate input patterns that activate specific fault conditions.<br><br>

    - Controllability and Observability: The ability to control inputs and observe outputs is critical for effective testing. Ensure that the circuit's inputs and outputs are accessible for applying test patterns and capturing responses.<br><br>

    - Test Coverage: Test coverage is a measure of how well the generated test patterns exercise the circuit's logic and detect potential faults. High test coverage indicates that a wide range of potential issues has been addressed.<br><br>

    - Automatic Test Pattern Generation (ATPG): ATPG tools are used to automatically generate test patterns that activate specific fault conditions. These tools use algorithms like Boolean Difference or Path Sensitization to generate effective test vectors.<br><br>

    - Applying Test Patterns: The generated test patterns are applied to the inputs of the combinational circuit. The circuit processes these patterns, and its outputs are observed.<br>
<br>
    - Fault Detection and Diagnosis: By comparing the observed outputs with expected outputs, you can identify discrepancies that might indicate the presence of faults. Analyzing the discrepancies helps you narrow down the location and type of fault.
<br><br>
    Iterative Process: The process might involve multiple iterations of test pattern generation, application, and analysis to improve coverage and fault detection.<br><br><br>



--> Why do we do DFT?<br><br>
  -The primary reasons for implementing DFT in IC design include:<br>

- Fault Detection: The main purpose of DFT is to detect manufacturing defects, design errors, and faults that may arise due to various factors. By embedding DFT features, designers can identify faults early in the manufacturing process, minimizing the likelihood of faulty chips reaching the market.<br>

- Reliability Enhancement: DFT techniques contribute to the overall reliability of ICs by identifying and addressing potential defects before the chips are deployed in real-world applications. This reduces the risk of field failures and costly recalls.<br>

- Cost Reduction: Detecting and rectifying issues during the manufacturing phase is significantly less expensive than addressing problems after the chips have been manufactured and integrated into devices. DFT helps in reducing post-manufacturing costs related to testing, debugging, and rework.<br>

- Time Savings: Traditional testing methods that rely on external testers can be time-consuming. DFT techniques such as Built-In Self-Test (BIST) and scan chains enable on-chip testing, leading to faster testing cycles and quicker time-to-market for products.<br>
So, basically it makes the testing easy at the post-production process.<br><br>

  We have 3 main levels of testing after a chip being fabricated,namely:<br>
  1.Chip-level,when the chips are manufactured,<br>
  Chip-level testing involves testing the individual integrated circuits (chips) that make up a system. It focuses on ensuring the functionality and quality of each chip before it's integrated into a larger assembly.itcemploys various Design for Testability (DFT) techniques, such as scan chains, Built-In Self-Test (BIST), and boundary scan (JTAG), to verify the chip's correctness.The main goal is to identify manufacturing defects, design errors, or faulty components within an individual chip.<br><br>

  2.Board-level,when the chips are integrated on the board,<br>
  Board-level testing involves testing the entire printed circuit board (PCB) that holds and connects multiple chips and components. It ensures that the board operates as intended, accounting for signal integrity, power delivery, and interconnections.The main goal is to verify the interactions between chips and components on the PCB, ensure signal quality, and validate power distribution.<br><br>

  3.System-level,when several boards are assembled together,<br>
  System-level testing involves testing the complete electronic system, which can comprise multiple PCBs, chips, software, and possibly mechanical components. It verifies the system's overall functionality and performance.The main goal is to ensure that the entire system functions as intended, meets performance specifications, and is ready for deployment in its intended application.<br><br><br>


  --> When or where DFT comes into the picture in ASIC design flow?<br>
     So, the answer lies in the below basic ASIC design flow diagram,<br>
     <img width="600" alt="netlist" src=""> <br>
    - DFT considerations start at the RTL design stage. Designers should account for scan chain insertion, test point placement, and any additional DFT logic required.<br>
    - Before synthesis, tools or methodologies may be used to perform DFT analysis. This includes identifying scan chains, memory BIST structures, and other DFT elements. then RTL modifications are made to incorporate DFT structures such as scan chains, boundary scan (JTAG) logic, and memory BIST controllers.<br>
    - Post synthesis the DFT logic is synthesized along with the design's functional logic. Care is taken to ensure that DFT elements are correctly inserted, and that the DFT logic and functional logic interact as intended.<br><br><br>

    --> pro's and con's of DFT,<br><br>
    Design for Testability (DFT) techniques offer several advantages and have certain drawbacks as well. Here's an overview of the pros and cons of DFT:<br>

  --> Pros (Advantages) of DFT:<br>
  - Improved Testability: DFT enhances the testability of complex digital designs, allowing efficient testing of circuits that might otherwise be challenging to test comprehensively.<br>
  - Reduced Time-to-Market: By incorporating DFT techniques, testing can be performed more quickly and efficiently, contributing to shorter development cycles and faster time-to-market.<br>
  - Lower Testing Costs: On-chip testing (e.g., scan chains, BIST) reduces the need for expensive external test equipment, resulting in cost savings during manufacturing.<br>
- Higher Test Coverage: DFT techniques can achieve higher test coverage, meaning a larger portion of potential faults is detected and addressed.<br>
- Debugging and Diagnosis: DFT features provide insights into the location and nature of faults, aiding debugging and diagnosis efforts.<br><br>

--> Con's of DFT: <br>
- Increased Design Complexity: Incorporating DFT elements can increase the overall design complexity, potentially leading to longer design times.<br>
- Area Overhead: DFT logic occupies additional chip area, which can impact the overall chip size, power consumption, and cost.<br>
- Timing Impact: Some DFT techniques, especially those involving scan chains, can impact the circuit's timing characteristics, potentially leading to performance degradation.<br>
- Manufacturing Challenges: The insertion of DFT logic can introduce manufacturing challenges, such as ensuring proper manufacturability and testing of DFT structures.<br>
- Test Pattern Generation: Generating effective test patterns can be complex, and achieving high test coverage may require significant computational resources and time.<br><br>

Careful consideration and balance between the advantages and disadvantages of DFT are crucial to achieving optimal results in the design and testing of integrated circuits.<br><br><br>



        
     
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
	  
	  ```ruby
	   csh
           dc_shell
	  ```
   
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









  




	

