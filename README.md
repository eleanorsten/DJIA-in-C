# DJIA Analysis Overview
This project performs data analysis across multiple dictionary (key–value store) implementations in C by storing and retrieving historical DJIA opening prices (1970–2022). Using array-based, linked list–based, and hash table–based (double hashing) structures, it measures insertion speed, lookup efficiency, and correctness.
By benchmarking these approaches on real-world financial data, the project delivers a clear outcome: identifying the fastest and most efficient data structure for large-scale analytical tasks.The work demonstrates the trade-offs between simplicity, memory usage, and efficiency when applying classic data structures to large real-world datasets.
**Reads DJIA data** (date → opening price) from a file.
**Dictionary Implementations:**
Array-based dictionary
Linked list-based dictionary
Hash table-based dictionary (double hashing)
**Performance Analysis:**
Measures storage time
Measures retrieval (fetch) time
Ensures correctness of lookups across all dictionary types

How It Works
1. Load the DJIA data from a CSV file (date and opening price).
2. Store all entries in each dictionary implementation.
3. Fetch ~13,000 dates (one intentionally missing) to validate correctness.
4. Compare execution time for storing and fetching across all implementations.
5. Print results for each dictionary type.

Installation 
Ensure DJIA file and C file are in the same directory
Compile C file
gcc DJIA_Assess.c -o myFile
Run File
./myFile

Output
Example output:
Store time with Array-Based Dictionary is 0.45s
All fetches matched for Array-Based Dictionary, time is 0.62s!
Store time with Linked List-Based Dictionary is 0.51s
All fetches matched for Linked List-Based Dictionary, time is 0.70s
Store time with Hash Table-Based Dictionary is 0.09s
All fetches matched for Hash Table-Based Dictionary, time is 0.12s!
This output shows performance comparisons across all three dictionary types.Features
Reads and processes historical DJIA data (1970–2022).
Implements three dictionary types:
Array-based
Linked list-based
Hash table (double hashing)
Measures and reports store and fetch times.
Provides insights into data structure trade-offs.

Implementation Components
Programming Language: C
Libraries:
printf, fprintf, malloc, free, exit,fopen, fclose, getline, strcmp, sscanf, strdup
Dataset: Historical DJIA data

Big-O Analysis
Array-Based Dictionary
- **Store:** O(1) per insert → O(n) total  
- **Fetch:** O(n) (linear search by key)  
- **Use Case:** Simple, but inefficient for large datasets
Linked List-Based Dictionary
- **Store:** O(1) per insert (append at head/tail) → O(n) total  
- **Fetch:** O(n) (linear traversal)  
- **Use Case:** Flexible size, but poor lookup performance	
Hash Table-Based Dictionary (Double Hashing)
- **Store:** O(1) average per insert → O(n) total  
- **Fetch:** O(1) average, O(n) worst-case (with collisions)  
- **Use Case:** Scales well, efficient for large datasets
Acknowledgments
Developed by: Eleanor Stenberg
Acknowledgments:
Prof. Jieyang Chen, Computer Science, University of Oregon
Prof. Hank Childs, Computer Science, University of Oregon
University of Oregon, CS Department


