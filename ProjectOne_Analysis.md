
Runtime Analysis Table
Operation	             Vector     	Hash Table          	  BST
Load File	             O(n)   	    O(n)	                  O(n log n)
Searching for Course   O(n)	        O(1)avg             	  O(log n)
Printing Sorted List   O(n log n) 	O(n log n)	            O(n)
Usage of memory	       Moderate	    Higher(hash overhead)  	Moderate


Advantages / Disadvantages
Structure                                          	Advantages                                                      	Disadvantages
Vector	               Simple and easy to implement, keeps the original inserting order        Slower search (O(n)) since theres sorting needed each time

Hash Table	           Method of fast searching O(1) avg, also has direct key lookup	         Needs more memory and needs conversion to a list for sorting

BST	                   Always sorted, fast search O(log n)	                                   A bit slower insertions, since it needs a balanced tree for best performance


Conclusion: 

Considering the trade-offs, run-time performance, and memory usage of the three data structures, the Binary Search Tree (BST) is the best option for ABCU's
course management system. While vectors are the easiest data structure to implement, if searching time takes linear time, and sorting time is potentially 
repeated, a developed dataset would quickly become unmanageable. Hash tables have the best average search times, but require additional overhead in memory 
and do not maintain information in sorted order. Maintaining courses in a sorted order is an essential requirement for the course management system.
Students and administrators must be able to view courses in alphanumeric order. The BST maintains a sorted course list "automagically," maintains efficient 
search times in logarithmic time, uses memory more efficiently than a hash table, and even supports efficient search times if the dataset becomes unbalanced.
Insertions may have a slower expected time complexity if the tree is unbalanced. To mitigate unbalanced times, either a balanced BST or a self-balancing tree
may be used. After exhausting the search for the best combination of speed, memory usage, and functionality, the BST provides the most reliable and scalable
data structure for managing and accessing ABCU's course catalog.
