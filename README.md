# Mathematics Accelerator

![Visualisation of a fractal by Wolfgang Beyer with the program Ultra Fractal 3. - Own work, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=321973](doc/fractal.jpg)

[Detailed Requirements and Technical Information](maths-accelerator/README.md)

The aim of this project is to create an educational tool that can visualise a mathematical function.
Evaluation of the function will be computationally intensive, which means that a custom-logic FPGA accelerator is a good choice for achieving the necessary responsiveness for human interaction.
The advantage of FPGA accelerator is that the logic is specific to the algorithm, which makes it more efficient than a CPU implementation.
However, maximising the potential of the FPGA requires parallelisation of the algorithm and choosing the best number representations and word lengths.
A starter project is provided that demonstrates the interface between a simple video generator and a processor system running Linux on the Zynq platform.

#### Core technical challenges

- Develop an accelerator for the Pynq system-on-chip FPGA platform, written in Verilog or SystemVerilog, that can generate a video output visualising the chosen function
- Identify opportunities for parallelism to increase calculation throughput
- Use numerical analysis to determine the optimum number representations and bit-widths to achieve a suitable accuracy
- Use human-computer interaction to allow a user to manipulate and understand the visualisation
- Quantify the impact of design implementation decisions in terms of algorthmic throughput
