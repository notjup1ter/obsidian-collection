---
class: "[[University/Classes/Discrete Mathematics 2 (CS 3120)|Discrete Mathematics 2 (CS 3120)]]"
date: 2026-02-18
---
# Resources
---
[[System/Attachments/02-RegularLanguages.pdf|02-RegularLanguages]]



To begin, start with [[Finite State Machine|Finite State Machines]]
- Model of computation with the following features:
	- very small amount of memory
	- must be able to understand machine's input and output
	- See if we can find at least one function the machine cannot compute

![[System/Attachments/Deterministic Finite Automata.png]]
Features of a [[Deterministic Finite Automata]]
- accepts input as strings
	- when one character of input is read, machine is transferred to a new state
	- can loop back into the same state
- has a **start state**, and can have one or more **accepting states**
- machine has a varied number of states, but can only be in one at a time, which is the only variable / memory DFA's have

*Technical Terminology*
*  A 5-tuple $(Q,\Sigma, \delta , q_{0}, F)$
	* $Q$ - finite set called the **states**
	* $\Sigma$ - finite set called the alphabet
	* $\delta$  -  $Q \times \Sigma \rightarrow Q$ - the **transition function**
	* $q_{0} \in Q$ - **start state**
	* $F \subseteq Q$ - set of **accept states**

[[2-DFA]]
- DFA, but can be in two states at once
- Has 2 start states, and machine accepts if either state is an acceptance state
- If there is a 2-DFA that accepts a string for a given finite alphabet, then a DFA does too!


[[Non-Determinism]] and [[Non-Determinisitic Finite Automata]]
* Feature of computational models that allows for the machine to exist in multiple states at once
	* Sounds the same as a DFA, BUT two distinctions
		* an extension of a 2-DFA (n-DFA technically)
		* 2-DFA is forced to exist in two states at once, while NFA's do NOT
		* Also, its transition function is the powerset of the states, $\mathcal{P}(Q)$. 
![[System/Attachments/Screenshot 2026-02-20 at 10.09.10 AM.png]]

[[University/Notes/Regular Languages|Regular Languages]] 
* What is it: a language that is recognizable by a [[Deterministic Finite Automata]]
* Properties:
	* [[Closure]]: When a regular operation is performed on a regular language, the resulting language is **still regular**
		* Shown by constructing some form of computationally equivalent machine to the original DFA that processes a regular langauge
			* Can be a 2-dfa, nfa, as these are both computationally equivalent to a DFA!