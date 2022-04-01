# Robo Game

This Assignment is to design and implement a parser and interpreter for a simple
programming language to control simple robots. The robot language has commands
directing the robot to perform various basic actions and test various sensors. It
also includes control structures (loops and conditionals) and operators for
calculating and comparing. A grammer for the full language is given below:

PROG  ::= STMT*
STMT  ::= ACT ";" | LOOP | IF | WHILE | ASSGN ";" 
LOOP  ::= "loop" BLOCK
IF    ::= "if" "(" COND ")" BLOCK [ "elif"  "(" COND ")"  BLOCK ]* [ "else" BLOCK ]
WHILE ::= "while" "(" COND ")" BLOCK
ASSGN ::= VAR "=" EXP
BLOCK ::= "{" STMT+ "}"
ACT   ::= "move" [ "(" EXP ")" ] | "turnL" | "turnR" | "turnAround" | 
          "shieldOn" | "shieldOff" | "takeFuel" | "wait" [ "(" EXP ")" ]
EXP   ::= NUM | SEN | VAR | OP "(" EXP "," EXP ")"  
SEN   ::= "fuelLeft" | "oppLR" | "oppFB" | "numBarrels" |
          "barrelLR" [ "(" EXP ")" ] | "barrelFB" [ "(" EXP ")" ] | "wallDist"
OP   ::= "add" | "sub" | "mul" | "div"
COND  ::= RELOP "(" EXP "," EXP ")"  | and ( COND, COND ) | or ( COND, COND )  | 
not ( COND )  
RELOP ::= "lt" | "gt" | "eq"
VAR   ::= "\\$[A-Za-z][A-Za-z0-9]*"       
NUM   ::= "-?[0-9]+"
