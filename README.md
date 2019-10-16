# Mapping_Example
Mapping example in Solidity

Note: Now, if you use var keyword like var person = p[a]; , you will get below SyntaxError:

SyntaxError: Use of the "var" keyword is disallowed. Use explicit declaration `struct bank.Person storage pointer person = ...´ instead.

If you use Person person = p[a]; , then you will get TypeError :

TypeError: Data location must be "storage" or "memory" for variable, but none was given. Person person = p[a];

So better Option is to use storage keyword along with Struct name like below:

Person storage person = p[a];
