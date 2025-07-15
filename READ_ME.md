
DJIA Data Organization

Author: Eleanor Stenberg
Last Updated: 2025-06-10

-- What it does -------

In this C program, the Dow Jones Industrial Average records from 1970 to 2022 were taken and organized in 3 different data structures- array dictionaries, linked lists, and hash tables. 


----- Dictionaries -----
-- Array Based 
Utilizes parallel arrays and linear searching for Key-Value pairs of Date-Value.
Big O Store time | O(1)
Big O Fetch Time | O(n)
--
-- Linked List 
Utilizes head insertion linked lists. Node: Date, Value, Pointer.
Big O Store time | O(1)
Big O Fetch Time | O(n)
--
-- Hash Table 
Utilizes open addressing and double hashing.
Big O Store time | O(1)
Big O Fetch Time | O(1)
--


----- File Guide -----
-- proj3D.c
Main program file that holds all 3 data structures. 

-- DJIA
Data input file of Dow Jones Records