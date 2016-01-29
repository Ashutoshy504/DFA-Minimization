# DFA-Minimization

### Summary
This program that takes a deterministic finite state machine and produces an equivalent one with a minimal number of states.

For more information on deterministics FSMs, see https://en.wikipedia.org/wiki/Deterministic_finite_automaton

### Constraints

This program can only convert FSMs which have a vocabulary size of less than or equal to 26, and the vocabulary symbols must
be translated to the letters a-z. Also, this program can only convert FSMs which have a state size of less or equal to 63, and these 
state numbers must be transated to 0-63.


### Input/Output
The program reads description of a deterministic finite state machine from standard input and produce an equivalent deterministic
finite state machine on standard output.  The states in the input are represented by integers
0, 1,..., 63 and the symbols by characters a, b, ..., z. 
* The first line of the input is the initial state.
* The second line contains the final states, separated by blanks. 
* Each subsequent line is a transition asa triple with a source state, a symbol, and a target state, separated by blanks.  
The output is analogous. Remember that the state numbers of the reduced FSM have no relevance to the state numbers of the original FSM.

 Sample input:<br />
 0<br />
 2 5<br />
 0 a 1<br />
 1 b 2<br />
 0 b 3<br />
 3 a 4<br />
 4 b 5<br />
 
 Sample output:<br />
 3<br />
 0<br />
 1 b 0<br />
 2 a 1<br />
 3 a 1<br />
 3 b 2<br />
 
### Make and run
 
This program can be compiled using gcc and does not require any third party libraries.
 
