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