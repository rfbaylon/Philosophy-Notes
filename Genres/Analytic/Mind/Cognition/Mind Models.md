Presupposes a lot from information in [[Do Machines Think]]

# Classicism
See [[Newell&Simon]]
*Physical Symbol Systems == PSS*
A physical symbol system has the necessary and sufficient conditions for general intelligent action.

Any system that incorporates physical symbols and acts upon such such a system.
	*If* I get the symbolic input "bear," *then* I act upon such an input and run. 

#### Heuristic Search Hypothesis
**Keep in mind, this view implies machines have desires!!**
Well structured task domains the agent has an explicit understanding of 
- initial state
	- ax+b=cx+b
- goal state
	- x=?
- operators
	- subtracting, dividing, etc
- restrictions
	- Mathematical axioms

A machine will search all possible trees in order to return a single answer by searching for it through many *many* possible legal answers.

## Classicism
See [[Newell&Simon]]
#Update 

### Argument from Heuristics
At some point though, as in chess, there are just way too many potential moves (10^120) in order to brute force a search through all legal possibilities. Thus, machines will use heuristics to reduce the amount of searches. This is the basis for AI. If humans have heuristics, according to [[Newell&Simon]], then it proves that humans are Physical Symbol Systems, proving machines can rise to the level of human intelligence, as we can both be PSS's

## A2 Classicism

### The Chinese Room Experiment
See [[Searle]]
[[Searle]] argues that Physical Symbol Systems (PSSs) cannot think as they are mere syntactic beings. PSSs only know how variables in a syntax interrelate, but can never understand what the variables actually mean. 
He makes this argument though the Chinese Room analogy
If you were in a room, being fed Chinese symbols on sheets of paper through a slot in the door and you had an instruction sheet telling you to press a certain set of buttons on a keyboard when a certain set character showed up, that wouldn't mean you knew Chinese. Even if a native Chinese speaker could semantically understand the inputs going into the room and could understand the outputs coming from the typing, that wouldn't mean that the person in the room operating with the symbols understands Chinese. 
In a similar way, just because meaningful statements are inputted to a computer and externally meaningful statements come out, that doesn't mean that the computer understands the context or meaning of what it is doing. Again, it only operates syntactically. 
Symbol input -> Searle (Rule Book) -> Symbol Output
Typed input -> CPU (Memory) -> Displayed Output

# Connectionism

![[Pasted image 20221224205341.jpg]]

![[Pasted image 20221225160756.png]]
([[Rummelhardt]], 1989)

Connectionists see it as a mistake to see the brain as a large central processeing system where cognition happens in racking a central system for matching parts. While Classicists see the brain as a computer like physical symbol system, connectionists see that cognityion happens within the connections of small nodes interrelating. Each neural path coordinates a small part of cognition that cross eachother to do more complex cognition. 

### Major Tenets
There are seven major components of any connectionist system: set of processing units; 
• a set of processing units;
• a state of activation defined over the processing units; 
• an output function for each unit that maps its state of activation into an output; 
• a pattern of connectivity among units; 
• an activation rule for combining the inputs impinging on a unit with its current state to produce a new level of activation for the unit;
• a learning rule whereby patterns of connectivity are modified by experience; and 
• an environment within which the system must operate.
([[Rummelhardt]], 1989)


## Connectionism
See [[Churchland]], [[Rummelhardt]]
#Update 

### Connectionist Learning is Flexible
See [[Rummelhardt]]
Whereas a classical PSS will fail when a variable is slightly changed, a connectionist model is incredibly flexible and can adapt quite easily as it's knowledge on the old variable is decentralized. Because of this, it can continue to cognize the familiar parts while creating new connections to adapt to the changes. PSS systems will crash when there is any slight variation. Because of this, Connectionist models also seem to be the most promising way forward for AI research as with neural networks can actually *learn*.
(Pg 223, [[Rummelhardt]], 1989)


### Connectionism Better Represents Memory
See [[Rummelhardt]]
Rather than a PSS system which always has equal access to all information, a connectionist system builds intensity as the same neural path is crossed frequently. As this happens, those paths are easier to cognize as they are more intense, and the non used paths retire to create more useful pathways. This seems to align much more wiht how humans use memory than a PSS system.
(Pg 222, [[Rummelhardt]], 1989)

### Connectionism Answers the Scaling Problem

### Connectionism Answers the Generalization Problem
See [[Rummelhardt]]
Given a set of observations, what is the appropriate principle that applies to all cases? Note that the network at any point in time can be viewed as a specification of an inductive hypothesis. 
Our proposal is that we follow a version of [[Ockham’s Razor]], and select the network that is consistent with the simplest, most robust observations made. 

## A2 Connectionism

### Connectionism Lacks Structure
See [[Fodor]], [[Pylyshyn]]
"What's deeply wrong with connectionist architecture is this. Because it acknowledges neither syntactic nor semantic structure in mental representations,
it perforce treats them not as a generated set but as a list. But lists, qua lists, have no structure; any collection of items is a possible list. And, correspondingly, on connectionist principles, any collection of (causally connected) representational states is a possible mind."
(Pg 334, [[Fodor]] & [[Pylyshyn]], 1998)