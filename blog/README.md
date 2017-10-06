# Programming the Mojo v3 FPGA Development Board

**Alexander DeForge Winter-2017**

The files provided are modified from code provided by the Embedded Micro Mojo IDE. Embedded Micro created the Mojo v3 development board.
<br><br>The Embedded Micro Mojo IDE can be found <a href="https://embeddedmicro.com/tutorials/mojo-software-and-updates/mojo-ide">here</a>.

## Modified Blinker Tutorial
In order to replicate the modified blinker tutorial, create a "new project" in the Mojo IDE and select "Blinker Demo" from the "From Example" dropdown.
<br><br>In addition to the provided modified files, an external astable multivibrator circuit must be constructed and interfaced with the Mojo v3 FPGA development board at PIN1. 
<br><br>This configuration provides functionality for blinking the Mojo v3 built-in LED's at the same rate as the astable multivibrator.
<br><br>The applicable files for this tutorial are: modified_blinker.luc, modifiedblinker_mojo_top.luc, and pinIn.ucf(a "Constraints" file).

## Modified CPU Tutorial
In order to replicate the cpu scheduler tutorial, create a "new project" in the Mojo IDE and select "Basic CPU" from the "From Example" dropdown.
<br><br>In addition to the provided modified files, an external astable multivibrator circuit must be constructed and interfaced with the Mojo v3 FPGA development board at PIN1.
<br><br>This configuration provides the foundation for executing two instruction ROM's in simulated logical concurrency. The logical concurrency is governed by a basic round robin scheduler; the time slice for this scheduler is governed by the signal from the astable multivibrator. The provided instRom's provide a proof of concept, but do not take full advantage of the architecture.
<br><br>The applicable files for this tutorial are: modified_cpu.luc, modified_instRom.luc, modifiedcpu_mojo_top.luc, and sliceclock.ucf(a "Constraints" file).

## Alternate Setups
Any alternate circuit which outputs no more than 3.3V may be used with the Mojo v3 FPGA development board.
<br><br>Behavior of the FPGA system, with the code provided, is undefined for alternate circuits.
