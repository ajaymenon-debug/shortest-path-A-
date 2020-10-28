
Calling the program:

The program has two command line arguments as follows: python a*algorithm.py INPUT/inputi.txt OUTPUT/outputi.txt Flag

eg for calling the program: python a*algorithm.py INPUT/input1.txt OUTPUT/output1.txt 3

Flag where the folders INPUT and OUTPUT should reside in the same folder as your program.

• inputi.txt – the name of the input file, where i is the number of the input file;
• outputi.txt – the name of the output file, where i is the number of the output file;
• Flag – indicates how many node expansions require a diagnostic output (if it is 0, no diagnostic output is required) 

Input:

• The first line will contain one number that specifies the number of rows and columns in the map.
• Subsequent lines will contain the map, one line per row. The following values will be accepted for each tile:
The following illustrates a procedure call and sample input for applying A/A* to a 3x3 map and printing diagnostic output for 5 iterations:
python planpath.py INPUT/input1.txt OUTPUT/output1.txt 5 where input1.txt is

SXR 
RRR 
XXG 


Output format:
• The sequence of moves are formatted as a list of actions separated by dashes followed by a blank space and the cost of the path according to the algorithm. If no path was found, the output should state NO-PATH.
• The actions (in UPPER CASE) are: R (Right), RD (Diagonal Right-Down), D (Down), LD (Diagonal Left-Down), L (Left), LU (Diagonal Left-Up), U (Up), RU (Diagonal Right-Up).
• For example, a path that goes Start, Right, Right-Down, Down, Down, Left- Down and Goal, with a total cost of 8, is represented as follows: S-R-RD-D-D- LD-G 8