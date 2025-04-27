# systems-programming-assignment-1-solved
**TO GET THIS SOLUTION VISIT:** [Systems Programming Assignment #1 Solved](https://www.ankitcodinghub.com/product/systems-programming-assignment-1-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;122379&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Systems Programming  Assignment #1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
The coalition race

1 Before You Start

● It is mandatory to submit all the assignments in pairs. If you can’t find a partner, use the designated forum.

● Read the assignment together with your partner and make sure you understand the tasks.

Before writing any code, make sure you read the whole assignment.

● Skeleton files will be provided on the assignment page, you must use these classes as a basis for your project and implement (at least) all the functions that are declared in them.

2 Assignment Goals

The objective of this assignment is to design an object-oriented system and gain implementation experience in C++ while using classes, standard data structures, and unique C++ properties such as the “Rule of 5”. You will learn how to handle memory in C++ and avoid memory leaks. The resulting program must be as efficient as possible.

3 Assignment Definition

In a faraway democracy, SPLand, there is a political crisis, they can’t form a government in years. The reason is complex promises about whether to cooperate with other parties.

We need you to help the politicians find a coalition!

After 5 elections, the SPLand president decided to change the method of forming a coalition by letting multiple “agents” from different parties try their best to create a 61 coalition as fast as possible.

In this assignment, you will write a C++ program that simulates the “Coalition Race” and report the first coalition formed (or failure).

The simulator should be based on a graph that contains:

● Parties as vertices

● Collaborations as edges (2 parties that agree to cooperate)

● “Similarity score” as edge weight, for every 2 connected parties

Here is an example for a graph at the beginning of the simulation. The colors represent the state of the parties (will be explained later).

The program will receive a config file (JSON) as input, which includes the parties’ details (id, name, number of mandates, join policy), the graph, and the list of agents (id, party id, selection policy). “Join policy” and “Selection policy” will be explained later.

Each agent belongs to a party. In every step, the agent offers an adjacent party to join. When a party has decided to join a coalition, it should clone the agent who made the offer to the newly joined party (so the joined party can now help the coalition).

To clarify:

● Coalition is a set of connected parties (in SPLand, connectivity is enough).

● In each party, there is a single agent if the party belongs to a coalition (state Joined).

● The total number of agents in the simulation equals the number of parties in the graph belonging to some coalition (state Joined).

Example

Suppose an agent from party#0 offered party#1 to join its coalition.

If party#1 accepts the offer, it adds itself to the coalition and adds a clone of the agent to the vector of agents (as well as updating the id and party id).

3.1 Classes

To solve this assignment, you will use the OOP approach. We will provide you skeleton files with some classes. Some of the declared methods will be implemented for you, and some are left for you to implement. You are free to add more classes, members, and methods to the existing classes but you must not change the given signatures.

Parser – This is a class with static methods only, that is responsible for parsing from JSON to object of class Simulation and the other way around. We supply the full implementation of the class, you should not change it, but you might want to look at it.

Simulation – This class is responsible for managing the simulation resources and making simulation steps (described in The program flow). This object is created by Parser using the initial values from the JSON configuration file. The Simulation object contains

● Graph

● Vector of Agents

Note that an edge exists if and only if the weight is greater than 0.

Party – A vertex in the graph. Each party has an id, name, number of mandates, join policy and party state. The states are:

1. Waiting – the party is not a part of any coalition yet, and also didn’t get offers yet.

2. CollectingOffers – after receiving the first offer, the party changes its state and starts collecting offers from Agents for joining coalitions.

The party has a “cooldown” – a timer of exactly 3 iterations, until moving to the next state by joining some coalition. Note, if a party got the first offer at the end of iteration 𝑖, it will join some coalition at the beginning of iteration 𝑖 + 3.

Note – the iteration is counted even if the party did not get an offer in that iteration.

3. Joined – after 3 iterations, the party uses JoinPolicy::join(…) method for deciding which offer to accept. After joining a coalition, the party’s state won’t change anymore and it cannot join any other coalitions.

Agent – This class has agentId, partyId (each agent associated with a single party), and selection policy. In each step, an agent is trying to select a neighboring party (in the graph) using SelectionPolicy::select(…) and offers the party to join its coalition.

SelectionPolicy – an abstract class that represents a strategy algorithm for selecting the next party to offer. It has the abstract method SelectionPolicy::select(…) that will be implemented in the derived classes:

● MandatesSelectionPolicy – Selects the neighboring party with the most mandates.

● EdgeWeightSelectionPolicy – Selects the neighboring party with the highest edge weight.

If the maximum mandates/edge weight is not unique, take the first party (with the lower id).

Example:

In this example, the agent (associated with party#0) will select party#1 when using EdgeWeightSelectionPolicy, or party#2 when using MandatesSelectionPolicy. Note that a party can receive offers in both Waiting and CollectingOffers states (as mentioned already, if a party is Waiting, it will change its state to CollectingOffers and trigger the cooldown timer).

JoinPolicy – an abstract class that represents a strategy algorithm for choosing which offer to accept and which coalition to join. It has JoinPolicy::join(…) abstract method that will be implemented in the derived classes:

● MandatesJoinPolicy – Selects the coalition with the largest number of mandates. Note that this refers to the number of mandates in the iteration when the offer is accepted. If the number of mandates is not unique, join the coalition that offered first.

● LastOfferJoinPolicy – Selects the coalition that made the last offer.

Example:

Suppose agent#1 offered party#1 to join its coalition in iteration 0, and agent#2 offered party#1 to join its coalition in iteration 1.

In iteration 3, party#1 needs to choose which coalition to join. In this iteration, the coalition of agent#1 has 45 mandates and the coalition of agent#2 has 40 mandates.

If party#1 is using MandatesJoinPolicy (configured in JSON file), it will join agent#1 coalition, and if the party is using LastOfferJoinPolicy, it will join agent#2 coalition.

You can (but don’t have to) add more classes if you find it helpful.

3.2 The program flow

We recommend following the main.cpp implementation we supplied while reading this section.

The program receives the config file’s path as the first command line argument. Once the program starts, it parses the config file and creates a “Simulation” object.

The format of the file is JSON, which is a very common format for object representation.

The main function checks every iteration if the termination conditions are satisfied (described in Termination conditions). Until they are satisfied, the main function calls the Simulation::step() method and saves the state of the simulation as JSON. At the end of the simulation, the results list will be written to an output file (this is how we can grade your solution).

All the file-handling methods are implemented for you in the supplied code.

The flow of Simulation::step() is applying Party::step(Simulation&amp; s) for each party (from graph) and then applying Agent::step(Simulation&amp; s) for each agent (keep the original order).

The flow of Party::step(Simulation&amp; s) is to check if the status is CollectingOffers and update the timer if so. Once the timer of 3 iterations is done – join some coalition (using the

JoinPolicy). When joining, the party’s state should be changed to Joined and the agent must be cloned.

The flow of Agent::step(Simulation&amp; s) is to select a party using SelectionPolicy::select(…) and then offer the party to join the coalition (in which the agent is a member).

The selection of the party is from the set of parties that satisfy the conditions:

1. The party is a neighbor of the party to which the agent belongs.

2. The party is in Waiting or in CollectingOffers state.

3. The party did not already receive an offer from any agent from the coalition to which the agent belongs. That is, if an agent from a coalition offers a party to join, other agents from the same coalition should not select the party (this might be a waste of an offer).

When there are no parties to select from, the agent is idle.

3.3 Configuration file format

The configuration file is given in a JSON format, and it contains a dictionary (hash map) with the following entries:

● parties – list of objects with name, mandates, join_policy.

● graph – a 2D list that represents the adjacency matrix.

● agents – list of objects with party_id, selection_policy.

The agentId and the partyId members are based on the index of the object in the list. When you clone an agent, make sure to change those fields in the cloned object.

Parsing of JSON is easy in C++ using Niels Lohman’s JSON for Modern C++ – an open-source project. If you want, you can learn how to use this package, and see examples here.

3.4 Termination Conditions

The program terminates when one of the coalitions reaches at least 61 mandates or when all the parties have already joined a coalition (all parties are in state Joined).

3.5 Output

The program creates a “.out” file in JSON format (which is a bit different from the input JSON). The parser is doing this part for you, but you will have to implement the methods marked with “TODO” in the skeleton files.

3.6 Full Example

Now we will follow a full simulation example based on the “01.json” config file we supplied to you. Take a look at it.

– At the beginning of the simulation, it initialized with 4 parties, 2 agents, and 2 coalitions ({party#0}, {party#3}).

– At Iteration#0:

– No parties in CollectingOffers state – pass.

– Agent#0 selects from the set {party#2} using EdgeSelectionPolicy and offers party#2.

– Agent#1 selects from the set {party#1, party#2} using EdgeSelectionPolicy and offers party#2.

– At Iteration#1:

– Party#2 in CollectingOffers state but the timer is not done – pass.

– Agent#0 has no parties to select from – pass.

– Agent#1 selects from the set {party#1} using EdgeSelectionPolicy and offers party#1.

– At Iteration#2:

– Party#1 and Party#2 in CollectingOffers state but both timers are not done – pass.

– Agents have no parties to select from – pass.

– At Iteration#3:

– Party#1 in CollectingOffers state but timer not done – pass.

– Party#2 in CollectingOffers state and timer is done – joining using LastOfferJoinPolicy to coalition#1 and clone agent#1.

– Agents have no parties to select from – pass – At Iteration#4:

– Party#1 in CollectingOffers state and timer is done – joining using MandatesJoinPolicy to coalition#1 and clone agent#1.

– Agents have no parties to select from – pass.

3.7 General instructions

● All classes with dynamic resources (and only them) must implement the rule of five.

● You are NOT ALLOWED to modify any of the supplied functions’ signatures (the declaration). We will use these functions to test your code, attempting to change their declaration might cause a compilation error and a significant reduction in your grade.

You are allowed to add additional header and cpp files as you see fit.

● You must not add any global variables to the program.

● Besides correctness, we will test your code quality and memory management principles. That means, for example, proper use of objects, pointers, references, and stack/heap allocation, as well as performance, clean and modular code.

● Make sure to read updates and clarifications on the assignment page.

● Ask questions regarding the assignment in the forum only.

4 Provided files

The following files will be provided for you on moodle:

● Headers: Agent.h, Graph.h, JoinPolicy.h, json.hpp (used for parsing the JSON config file), Parser.h, Party.h, SelectionPolicy.h, Simulation.h

● Sources: Agent.cpp, Graph.cpp, main.cpp, Parser.cpp, Party.cpp, Simulation.cpp

● Basic makefile – you should extend it

● visualization.py (will be explained in section 5)

● Tests: 3 JSON files and their expected outputs (will be explained in section 6)

5 Visualization

To help you debug your simulation, we wrote for you a python script that can generate graph visualizations from the output file.

To run it, first install some packages by running:

sudo apt update

sudo apt-get install python3-dev python3-setuptools

sudo apt-get install libtiff5-dev libjpeg8-dev libopenjp2-7-dev zlib1g-dev libfreetype6-dev liblcms2-dev libwebp-dev tcl8.6-dev tk8.6-dev python3-tk libhar buzz-dev libfribidi-dev libxcb1-dev

sudo apt-get install python3-pip pip3 install networkx pip3 install matplotlib

and then:

python3 visualization.py &lt;path to output ile&gt;

6 Tests

We provided you 3 JSON files for different scenarios of the program, and their expected output. You can compare the expected output with your actual output using the Linux diff command:

diff -s &lt;expected output ile&gt; &lt;your output ile&gt;

This is the important part – you should have the exact same output as expected.

We encourage you to write additional tests yourselves to further examine the behavior of your program.

7 Submission

● Your submission should be in a single zip file called ”student1ID_student2ID.zip”. The files in the zip should be set in the following structure:

▪ src/

▪ include/

▪ bin/

▪ makefile

src/ directory includes all .cpp files that are used in the assignment. include/ directory includes the header (*.h or *.hpp) files used in the assignment.

bin/ directory should be empty, no submitting of binary files. It will be used to place the compiled file when checking your work.

● The makefile should compile the cpp files into the bin/ folder and create an executable named ”cRace” and place it also in the bin/ folder.

● Your submission will be built (compile+link) by running the following commands: “make”.

● Your submission will be tested by running your program with different scenarios.

● Your submission must compile without warnings or errors on the department computers.

● We will test your program using Valgrind in order to ensure no memory leaks have occurred. We will use the following valgrind command:

The expected valgrind output is:valgrind –leak-check=full –show-reachable=yes [program-name] [program parameters] All heap blocks were freed — no leaks are possible

● Compiler commands must include the following flags:ERROR SUMMARY: 0 errors from 0 contexts (suppressed: 0 from 0)

● After you submit your zip to Moodle, re-download the file that you have just submitted,-g -Wall -Weffc++ -std=c++11 -Iinclude

GOOD LUCK AND ENJOY!
