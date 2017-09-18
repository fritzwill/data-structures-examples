Will Fritz
3/27/2017

From the users perspective, the program is meant to rank people based on the card they have. The cards come from a standard 52 card deck. The users are supposed to enter in how many cardholders there will be. Then on the following lines THose cardholders are listed in the format: Name Rank Suit. After repeating this as many times as they want, the user then terminates the input by placing a '-1' on their final line.

From the programmers perspective, a struct is used to represent each cardHolder. The struct has three values: string name, int rank, int suit. THe main program starts by reading in the first line, which is the number of cardHolders to be inputted. A list of type cardHolders is then initiated to store the output. THe program then enters a for loop for the number of names so that many lines are read using getline. Each individual word in the line is accessed by making an istringstream object. A cardHOlder 'filler' object is initiated and then filled according by uitlizing a switch statement. This filler cardHolder is then placed into the output list. This entire process is placed in a while loop that runs until '-1' is read in from the user's input. THis allows for multiple sets of cardHolders to be ranked. After the -1 is read, output list is sorted by calling sort(&compareRank); This called the sort function on the output according t the rule set by the created function 'compareRank'. This function implements the rules of ranking by accessing the components of the inputted cardHolder objects. After the lsit is sorted, each name is printed according to the lab description of 'name, name, name'. This is done by implementing a custom print function.

I tested the program by inputting both custom inputs and the inputs provided by the lab. The code produced the intended values every time. I then used the 'make test' provided by the lab. The program correctly compiled, passed the output test, passed the memory test, and passed the time test.