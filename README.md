Download Link: https://assignmentchef.com/product/solved-metcs526-module4
<br>
<strong>Problem 1 </strong>. Consider the following heap, which shows integer keys in the nodes:

Show the resulting tree if you add an entry with key = 27 to the above tree? You need to describe, step by step, how the resulting tree is generated.

<strong>Problem 2 .</strong> Consider the following heap, which shows integer keys in the nodes:

Suppose that you execute the <em>removeMin</em>( ) operation on the above tree. Show the resulting tree. You need to describe, step by step, how the resulting tree is generated.

<strong>Problem 3 </strong> This problem is about the chaining method we discussed in the class. Consider a hash table of size N = 11. Suppose that you insert the following sequence of keys to an initially empty hash table. Show, step by step, the content of the hash table.

Sequence of keys to be inserted: &lt;5, 8, 44, 23, 30, 34, 52, 32, 15, 16&gt;

<strong>Problem 4</strong>. This problem is about linear probing method we discussed in the class. Consider a hash table of size N = 11. Suppose that you insert the following sequence of keys to an initially empty hash table. Show, step by step, the content of the hash table.

Sequence of keys to be inserted: &lt;5, 8, 44, 23, 30, 34, 52, 32, 15, 16&gt;

<strong>Problem 5  </strong>Suppose that your hash function resolves collisions using open addressing with double hashing, which we discussed in the class. The double hashing method uses two hash functions <em>h</em> and <em>h</em>’.

Assume that the table size <em>N = </em>13, <em>h</em>(<em>k</em>) = <em>k</em> mod 13, <em>h’</em>(<em>k</em>)<em> = </em>1 <em>+ </em>(<em>k mod </em>11), and the current content of the hash table is:

0       1       2       3       4       5       6       7       8              9 10 11 12

<table width="468">

 <tbody>

  <tr>

   <td width="36"> </td>

   <td width="36"> </td>

   <td width="36">28</td>

   <td width="36"> </td>

   <td width="36"> </td>

   <td width="36">98</td>

   <td width="36"> </td>

   <td width="36">59</td>

   <td width="36"> </td>

   <td width="36">22</td>

   <td width="36"> </td>

   <td width="36">43</td>

   <td width="36">51</td>

  </tr>

 </tbody>

</table>




If you insert <em>k</em> = 15 to this hash table, where will it be placed in the hash table? You must describe, step by step, how the location of the key is determined.

<strong>Problem 6). </strong>The goal of this problem is to give students an opportunity to observe differences among three data structures in Java – Java’s <em>HashMap</em>, <em>ArrayList</em>, <em>LinkedList</em> – in terms of insertion time and search time.

Students are required to write a program that implements the following pseudocode:

create a HashMap instance myMap create an ArrayList instance myArrayList create a LinkedList instance myLinkedList

Repeat the following 10 times and calculate average total insertion time and average total search time for each data structure

generate 100,000 random integers in the range [1, 1,000,000] and store them in the array of integers insertKeys[ ]

// begin with empty myHap, myArrayList, and myLinkedList each time




// Insert keys one at a time but measure only the total time (not individual insert  // time)

// Use <em>put</em> method for HashMap

// Use <em>add</em> method for ArrayList and LinkedList




insert all keys in insertKeys [ ] into myMap and measure the total insert time insert all keys in insertKeys [ ] into  myArrayList and measure the total insert time insert all keys in insertKeys [ ] into myLinkedList and measure the total insert time




generate 100,000 random integers in the range [1, 2,000,000] and store them in the array searchKeys[ ].




// Search keys one at a time but measure only total time (not individual search // time)

// Use <em>containsKey</em> method for HashMap

// Use <em>contains</em> method for ArrayList and Linked List




search myMap for all keys in searchKeys[ ] and measure the total search time search myArrayList for all keys in searchKeys[ ] and measure the total search time  search myLinkedList for all keys in searchKeys[ ] and measure the total search time




Print your output on the screen using the following format:




Number of keys = 100000




HashMap average total insert time = xxxxx

ArrayList average total insert time = xxxxx

LinkedList average total insert time = xxxxx




HashMap average total search time = xxxxx

ArrayList average total search time = xxxxx

LinkedList average total search time = xxxxx




You can generate <em>n</em> random integers between 1 and N in the following way:




Random r = new Random(System.<em>currentTimeMillis</em>() );

for <em>i</em> = 0 to <em>n</em> – 1

a[i] = r.nextInt(N) + 1




When you generate random numbers, it is a good practice to reset the seed. When you first create an instance of the Random class, you can pass a seed as an argument, as shown below:




Random r = <strong>new</strong> Random(System.<em>currentTimeMillis</em>());




You can pass any long integer as an argument. The above example uses the current time as a seed.




Later, when you want to generate another sequence of random numbers using the same Random instance, you can reset the seed as follows:




r.setSeed(System.<em>currentTimeMillis</em>());




You can also use the <em>Math.random</em>( ) method. Refer to a Java tutorial or reference manual on how to use this method.




We cannot accurately measure the execution time of a code segment. However, we can estimate it by measuring an elapsed time, as shown below:




long startTime, endTime, elapsedTime; startTime = System.<em>currentTimeMillis</em>();

// code segment

endTime = System.<em>currentTimeMillis</em>(); elapsedTime = endTime ‐ startTime;




We can use the <em>elapsedTime</em> as an estimate of the execution time of the code segment.




Name the program <em>Hw4_P6.java</em>.

<strong> </strong>

<strong>Deliverable</strong>




You need to submit the following files:

<ul>

 <li><em>P1_P5pdf</em>: This file must include:</li>

 <li>Answers to problems 1 through 5.</li>

 <li>Discussion/observation of Problem 6: This part must include what you observed and learned from this experiment and it must be “substantive.”</li>

 <li><em>java</em></li>

 <li>Other files, if any.</li>

</ul>




Combine all files into a single archive file and name it <em>LastName_FirstName_hw4.EXT</em>, where <em>EXT</em> is an appropriate archive file extension, such as <em>zip</em> or <em>rar</em>.

<strong> </strong>

<strong>Grading </strong>