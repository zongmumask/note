# Concepts

* formal language: set of strings
* string: a sequence of symbols from an alphabet
* alphabet: a finite set of symbols
* finite automata: can be used to recognize certain languages
* deterministic finite automata: DFAs, have exactly one transition out of each state for each symbol in the alphabet
* two DFAs equivalent if they recognize the same laguage
* ![image](https://upload-images.jianshu.io/upload_images/1322498-00e670c8ffb681a0.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/922/format/webp)
* in a NFA a string is accepted if there exits at least one path from the start state to accept state
* ![image](https://upload-images.jianshu.io/upload_images/1322498-acbbb6c89d81733d.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1200/format/webp)
* ![image](https://upload-images.jianshu.io/upload_images/1322498-69cddbd68318fc99.jpg?imageMogr2/auto-orient/strip|imageView2/2/w/1200/format/webp)
* DFA and NFA's graph deepth is the number of symbols in the processing string
* regular language is a language that can recognize by a DFA

# NFA to DFA conversion

* NFA to DFA conversion: thinking of a combination of the states in the NFA as a single state in DFA that you are constructing
* the subset construction: the state in DFA we are constructing is a subset of states in NFA
* the number of subsets is 2 power N(the number of states count)
* epsilon closure(q0): the epsilon closure of q0 is q0 itself plus all the states that can be reached from q0 via epsilon transitions
* ![image](https://upload-images.jianshu.io/upload_images/1322498-1af20109068553b0.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* ![image](https://upload-images.jianshu.io/upload_images/1322498-8f2f82d95ec68e0f.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
* the start state in the target DFA is the epsilon-closure of the start state in the original NFA
* a state(set of NFA states) in the DFA ia an accept state if at least one of the states that constitute the state corresponds to an accept state in the original NFA
* conversion make trap state explicit

# Regular operations and Regular expression
![image](https://upload-images.jianshu.io/upload_images/1322498-e45482e0f815153c.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)