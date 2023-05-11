The Monty language
Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). It relies on a unique stack, with specific instructions to manipulate it. The goal of this project is to create an interpreter for Monty ByteCodes files.

Monty byte code files

Files containing Monty byte codes usually have the .m extension. Most of the industry uses this standard but it is not required by the specification of the language. There is not more than one instruction per line. There can be any number of spaces before or after the opcode and its argument:The monty program.

Usage: monty file

where file is the path to the file containing Monty byte code

Opcodes that you can use with monty:

push	pushes an element to the stack.
	Usage: push <int>
	where <int> is an integer.

pall	prints all the values on the stack, starting from the top of the stack.

pint	prints the value at the top of the stack, followed by a new line.

pop	removes the top element of the stack.

swap 	swaps the top two elements of the stack.

add     adds the top two elements of the stack.

nop 	doesn’t do anything.

sub 	subtracts the top element of the stack from the second top element of the stack.

div 	divides the second top element of the stack by the top element of the stack.

mul 	multiplies the second top element of the stack with the top element of the stack.

mod 	computes the rest of the division of the second top element of the stack by the top element of the stack.

'#'	when the first non-space character of a line is #, treat this line as a comment.

pchar 	prints the char at the top of the stack, followed by a new line.

pstr 	prints the string starting at the top of the stack, followed by a new line.

rotl 	rotates the stack to the top.

stack 	sets the format of the data to a stack (LIFO). This is the default behavior of the program.

queue 	sets the format of the data to a queue (FIFO).

Brainf*ck files are stored inside the bf sub directory.

bf 1001-add.bf 	Add two digits given by the user.

bf 02-mul.bf 	Multiply two digits given by the user.

bf 1003-mul.bf	Read the two digits from stdin, multiply them, and print the result, followed by a new line


