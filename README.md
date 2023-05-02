Download Link: https://assignmentchef.com/product/solved-comp-352-data-structure-and-algorithms-assignment-3
<br>
<strong> </strong>




Computer Science and Software Engineering

<strong>                                             </strong>




<strong> </strong>




<ol>

 <li>Written Questions</li>

</ol>




<h1>Question 1</h1>

<strong> </strong>

Assume a hash table utilizes an array of 13 elements and that collisions are handled by <em><u>separate chaining</u></em>. Considering the hash function is defined as: h(k) = k mod (13).

<strong> </strong>

<ol>

 <li>Draw the contents of the table after inserting elements with the following keys:</li>

</ol>

{245, 28, 10, 49, 70, 225, 122, 12, 180, 140, 177, 65, 223, 85, 111, 256, 18, 69, 59, 185, 105, 120, 44}.




<ol>

 <li>What is the total number of collisions caused by the above insertions?</li>

</ol>




<h1>Question 2</h1>







Assume an <em><u>open addressing</u> </em>hash table implementation, where the size of the array <em>N </em>= 19, and the <em><u>double</u> <u>hashing</u> </em>is performed for collision handling. The second hash function is defined as:

<em>d(k) = q – k mod q</em>, where <em>k </em>is the key being inserted in the table and the prime number <em>q = 11</em>. Use simple modular operation (<em>k mod N</em>) for the first hash function.

<ol>

 <li>Show the content of the table after performing the following operations, in order:</li>

</ol>

put(37), put(17), put(24), put(36), put(62), put(28), put(58),put(47), put(19).

<ol>

 <li>What is the size of the longest cluster caused by the above insertions?</li>

 <li>What is the number of occurred collisions as a result of the above operations?</li>

 <li>What is the current value of the table’s <em>load factor</em>?</li>

</ol>







<h1>Question 3</h1>




Assume the utilization of <em><u>linear probing</u> </em>instead of <em>double hashing </em>for the implementation given in Question 2.

Still, the size of the array <em>N </em>= 19, and that simple modular operation (<em>k </em>mod N) is used for the hash function.

<ol>

 <li>Show the contents of the table after performing the following operations, in order: put(37), put(17), put(24), put(36), remove(62), remove(28), put(58), put(47), remove(19).</li>

 <li>What is the size of the longest cluster caused by the above insertions? Using Big-O notation, indicate the complexity of the above operations.</li>

 <li>What is the number of occurred collisions as a result of the above operations?</li>

</ol>

<strong> </strong>




<h1>Question 4</h1>




<u>Note:</u> Part (a) and (b) are independent in this question.

Consider the following AVL tree:













<ol>

 <li>Draw the AVL tree resulting from the insertion of an entry with key 56 in the AVL tree shown above.</li>

</ol>




<ol>

 <li>Draw the AVL tree resulting from the removal of the entry with key 28 in the AVL tree shown above.</li>

</ol>







<h1>Question 5</h1>




Consider the following elements:

12, 47, 74,19, 89, 4, 63, 26, 53, 8, 93, 71, 15, 87, 50, 17, 82




Trace the steps when sorting these values into ascending order using:

<ol>

 <li>Merge Sort</li>

 <li>Quick Sort (using (middle +1) element as pivot point)</li>

 <li>Bucket Sort – We know that the numbers are less than 99 and there are 10 buckets. d) Radix Sort</li>

</ol>

<strong> </strong>




<h1>Question 6</h1>




Consider the graph shown below:







<ol>

 <li>Give the adjacency matrix representing this graph.</li>

 <li>Give the adjacency lists representing this graph.</li>

 <li>Show the breadth-first search trees for the graph starting at node 0.</li>

 <li>Show the depth-first search trees for the graph starting at node 0.</li>

</ol>

<h1>Question 7</h1>




Use <em>Dijkstra’s </em>Algorithm to find the shortest path of the following graph from node H to each of the other nodes.













<h1>Programming Questions</h1>




In these programming questions you will experimenting writing  your own Binary Search Tree with a couple  of methods.




A <em>Binary Search Tree</em> (BST) is a tree-based data structure in which each node has at most two children, which are referred to as the left child and the right child, and the topmost node in the tree is called the root. It additionally satisfies the binary search property, which states that the key in each node must be greater than or equal to any key stored in the left subtree, and less than or equal to any key stored in the right subtree.




<u>Important Note:</u>  For all the questions below you must provide a solution that does not refer to the given example. (i.e.  it should be able to output the appropriate output for any given collection of integer keys).




Question 1:




In this first question, you will be developing your own Binary Search Tree <em>MyBST</em> program (i.e., class) in two versions.

<ol>

 <li>In version 1 of your <em>MyBST</em>, you implement <u>a recursive</u> method to insert random integer keys in the BST.</li>

 <li>In version 2 of your <em>MyBST</em>, you implement <u>an iterative</u> method to insert random integer keys in the BST.</li>

</ol>

Your program should take a set of random integer keys such as:




<table width="249">

 <tbody>

  <tr>

   <td colspan="2" width="249">15   25   20   22   30   18   10   8   9   12   6</td>

  </tr>

  <tr>

   <td width="206">and output the corresponding BST:</td>

   <td width="43"> </td>

  </tr>

  <tr>

   <td colspan="2" width="249">6   8   9   10   12   15   18   20   22   25   30</td>

  </tr>

 </tbody>

</table>







Question 2:




In this question you will be using one version of your <em>MyBST</em> program from question 1, and add a method that finds the total subtrees of the BST that are within the given range.




Example, given a set of random integer keys such as:

<table width="227">

 <tbody>

  <tr>

   <td colspan="2" width="227">18  23  12  28  15  9  33  25  13  11  21</td>

  </tr>

  <tr>

   <td width="83">and the range</td>

   <td width="144">[8, 23]</td>

  </tr>

 </tbody>

</table>

Your program should output:  The total number of subtrees is 6.




Figure 1 depicts the details of this results:







Figure 1




Question 3:




In this question you will be using one version of your <em>MyBST</em> program from question 1, and add a method that remove nodes from your BST that have keys outside a given valid range.




Example, given a set of random integer keys such as:

<table width="314">

 <tbody>

  <tr>

   <td width="314">22, 48, 19, 4, 13, 78, 83, 59, 29, 17, 66 and the range</td>

  </tr>

 </tbody>

</table>

[5,40]




Your program should output:  The key within the valid range are:  13 17 19 22 29.








