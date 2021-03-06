CoreSociety
===========

Core Society is a digital organism simulator based on a grid of programmable Cores.
Not unlike a cellular automata a core can affect the state of its 4 direct neighbours. 

Each core has 256 words of memory and an intruction pointer pointing at a specific memory adress. When the core gains execution focus that word is interpreted as an instruction. The instruction set is similar to that of ordinary CPUs and allows the core to act like a tiny computer. It includes the ability to reserve and release energy which is used up by executing instructions and also determines which core is the next in line to execute: the core with the currently highest unbound energy!

There are no free instructions and one core will always have execution focus. So even a grid only consisting of uninitialized cores will leak energy.

The simulator ships with a handful of missions. The task is usually to beat a certain score threshold by defining the initial memory layout of a subset of the grid's cores. As soon as the simulation starts there's no way to interact with the outcome so you have to come up with a smart strategy, an efficient implementation and that usually means doing lot's of iterations.

All but the most basic missions will require your program to write to the memory of adjacent cores to change their program and thus make them work towards your goal. Usually the grid is initialized with "enemy" cores who will try to prevent you from achieving a high score by spending all their energy to decrease the score. So the first part of the sim is usually spend on getting board control, then you can spend the remaining total energy budget on getting the score up.

***Getting started***

Download the repository and just start the prebuild executable (CoreSociety.exe) or build it yourself.

Click on the top left icon to open a scenario. A click on the 'Play' Icon starts the simulation.

You can click on a listing in the 'Deck' to open a second window that allows you to modify the listing which defines a core's memory contents. That way you can change the initial state of the simulation to attain a favorable outcome.

To learn more about the instruction set and how to program a core have a look at the Documenation.pdf.

Last but not least there are reference solutions supplied if you are stuck with a mission.

Have fun!

