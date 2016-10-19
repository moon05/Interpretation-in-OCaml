Authors: Gabriel Morales & Abdullah Al Mamun
Course: CSC 254 - Programming Language Design & Implementation
Assignment: Interpretation

Files Included:
	- interpreter.ml
	- README.txt

How to Run:
	$ ocaml str.cma interpreter.ml

Description:
	AST_ize functions
		- These were similar to the action routines used in the last project to create
		  an explicit syntax tree
		- The statment list created invloved removing all the unnecessary parse tree
		  nodes and nonterminals to extract the actual rules of the grammar in their
		  appropriate forms
		- Most of these functions actually create ast nodes to add to the ast_sl
		  structure to be returned. The ast_ize_sl function manages the generated nodes
		  by storing them all into one list
	
	Interpret functions
		- These were the functions that took the AST_ize as input and then interpreted
		  the program.
		- Most of the functions output a tuple of status code, a memory list, an input
		  list and an output list.
		- Only interpret_expr returns a value and memory list tuple. This function is
		  in pretty much every other function to evaluate expressions.
	
	Completing Basic Requirements
		- We have taken care of catching the dynamic errors:
			~ unexpected end of input
			~ non-numeric input
			~ use of an uninitialized variable
			~ divide by zero
	
	Extra-Credit
		- We have attempted suggested extra-credit no. 3
		- This generates warning messages at the execution for any values that were
		  assigned into a variable and then never used (These do not necessarily
		  appear at the end of the output)



