# MINI-PROJECT
# DESIGN AND IMPLEMENTATION OF REAL TIME TRAFFIC CONTROL SYSTEM USING VERILOG
# TEAM MEMBERS
B. Poojitha
B. Sandhya
B. Rakesh
N. Prashanth Reddy

# OBJECTIVE OF THE PROJECT

The main objective was to design a traffic light controller system to manage the traffic movement of four roads at the same time, and achieve maximum utilization for the four roads. Optimal traffic light control is a multi-agent decision problem, our design learns the expected waiting times of cars for red, yellow and green lights at each intersection. In the rush hours, when people going to work or coming back to home the traffic lights of all roads are controlled with fixed time. Optimize the traffic signal timing of a network of intersection by evaluating the real time traffic demand in the area. To reduce delays, shorter queues and decreased travel times. Coordinating signal timing minimizes stating and stopping of vehicles in the traffic to avoid the traffic jam.

# INTRODUCTION

Now a days Traffic congestion is a severe problem in many modern cities around the world. Traffic congestion has been causing many critical problems and challenges in the major and most populated cities. To travel to different places within the city is becoming more difficult for the travelers in traffic. Due to these congestion problems, people lose time, miss opportunities, and get frustrated. Traffic congestion directly impacts the companies. Due to traffic congestions there is a loss in productivity from workers, trade opportunities are lost, delivery gets delayed, and thereby the costs goes on increasing. To solve these congestion problems, we have to build new facilities & infrastructure but at the same time make it smart. Therefore many countries are working to manage their existing transportation systems to improve mobility, safety and traffic flows in order to reduce the demand of vehicle use. Therefore, many researches about traffic light system have been done in order to overcome some complicated traffic phenomenon but existent research had been limited about present traffic system in well-travelled traffic scenarios. The Aim of the project is to develop a Traffic Control System using Verilog in xilinx software as to reduce cost of the requirements rather than using sensors, PLD technology which are of high cost. we have to implement the Street light controller using the Verilog code and the later is simulated using Xilinx software and simulation is done with the ISE Simulator. Through using Verilog language to the traffic light controller design, the traffic light control circuit uses digital signal automatic control to realize two groups of lights which are red, yellow and green. Those lights command vehicles and pedestrians passing safely at the crossroad, which bases on the data of traffic state transition.

# VLSI DESIGN FLOW

1)	DESIGN ENTRY :
Design entry is the first step in the design of any VLSI circuit using EDA tools. In this step the intended dHardware description languages :
Design is entered on the personal computer. Figure below shows the various ways of design entry. The various ways in design entry are as follows,
•	Schematic entry
•	Design entry using Hardware Description Languages(HDL)
•	Using Finite State Machines (FSM)
•	EDIF entry
•	Ways of design entry

3)	FUNCTIONAL/GATE LEVEL SIMULATION :
The functional gate level simulations are carried out to test the designs entered in the design entry tools. The designs are tested by applying the test inputs are outputs are checked as per the specifications. The important role of this simulations is to find the errors in the design before the design is implemented in the target device (CPLD/FPGA). These simulations are mainly carried out initial stages of the system design.

3)	COMPILERS AND SYNTHESIS TOOLS :
A typical CAD software package contains several components. Analyze is the first step in the synthesis flow. In this stage, the HDL code is checked for syntax errors. The Logic optimization is the process that decreases the area or increases the speed of a design. Normally the system designer develops the HDL code and the synthesis tool identifies the syntax errors. The synthesis process creates the net list. Net list is the description of the circuit developed by the HDL code. Net list is basically contains the connectors, instances and the connected signals.

4)	ASSIGNING CONSTRAINT:
Design constraint is a subset of the values of a type. The set of possible values for an object of a given type that can be subjected to a condition is called a constraint. The file containing the information A program that converts all input results into a single merged file. About the pins, there direction and locked pin of the selected hardware device is called as User Constraints File (UCF). Before implementing the design on the actual device this file is required which selects the particular functional block (for CPLD) and configurable logic block (for FPGA) on which design to be loaded.

5)	IMPLEMENTATION :
In this step the design is implemented on the device. A library containing the design unit in which a given component is declared is called as Target cell library. The target library is used to determine the visible entity declaration under certain circumstances for a default binding indication. The different steps in implementation are as follows,
●	Mapping or Fitting:
Mapping is the step in which the logic elements are mapped to the logic functions on a FPGA device. Fitting is the step to put the design logic into macro cell locations of the CPLD.

6)	TIMING SIMULATION:
This simulation step is carried out after the synthesis, placing and routing of the design. The important role of this step is to check the dynamic timing details of the HDL code. A timing analysis or a point-to- point delay analysis of a design network is called as Static Timing Analysis.

7)	PROGRAMMING:
The final step of the design process is the downloading of the design on the device. In this step a bit stream file is created, a bit stream is a stream of data that contains location information for logic on a device, that is, the placement of Configurable Logic Blocks. This bit stream file is downloaded on the device using programming. Programming is the process of configuring the programmable interconnect in the FPGA or CPLD.

# MOORE'S MACHINE CYCLE

Moore machine is a finite-state machine whose current output values are determined only by its current state. This is in contrast to a Mealy machine, whose output values are determined both by its current state and by the values of its inputs. Like other finite state machines, in Moore machines, the input typically influences the next state. Thus the input may indirectly influence subsequent outputs, but not the current or immediate output.
Road structure shows four traffic lane represented by north side lane, east side lane, south side lane and west side lane. Every lane has their own separate traffic light system which is having regular as usual red, yellow and green lights. The north side lane has north green, north red, and north yellow light. The above figure shows the Moore machine cycle. Here first the cycle starts at time T=0 and it travels from S0 and green light will be accessed for north lights. After 7s then the cycle move from S0 to S1 and the green light and red light will be accessed. Now from S1 yellow and red color will be accessed for north lights. After 3s, the cycle move from S1 to S2. Again from S2, green light will be accessed for south lights. After 7s, the cycle moves from S2 to S3 and the green and red lights will be accessed. From S3, yellow and red colors are accessed for south lights for 3s. After 3s, cycle moves to S4. From S4, green color and red color are accessed for east lights for 7s. After 7s, cycle moves to S5. From S5, yellow and red colors are accessed for east lights for 3s and after that cycle moves to S6. From S6, green and red colors are accessed for west lights for 7s and after that cycle moves to S7. From S7, yellow and red colors are accessed for west lights for 3s and after that cycle moves to S0.

# ADVANTAGES

1.	Helps in reducing the frequency of an accident of some special nature i.e; Right angle accidents.
2.	They intercept heavy traffic to allow traffic to cross the road intersection safely.
3.	They direct traffic on different routes without excessive congestion.
4.	It reduces the cost by doing this project in VHDL rather than using embedded systems.
5.	Power consumption is less



