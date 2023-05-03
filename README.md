Download Link: https://assignmentchef.com/product/solved-cs-457-assignment-3
<br>
Database Management Systems

<strong>Programming Assignment 3: Table Joins </strong>

<h1>Overview</h1>

In this assignment you will write a program that allows a database user to make queries over multiple tables. That is, you will implement table joins using techniques we discussed in the class (e.g., nested loop). This assignment assumes the metadata and data manipulations on singular tables are already available, which should have been provided (implemented) in the first two programming assignments.

<h1>System Design</h1>

<ul>

 <li>You will decide how to implement the join operations o In lectures: nested loop o As always, you are free (in fact, encouraged) to come up with your own design</li>

 <li>In the design document, you should clearly explain how your program joins tuples from two source tables. If in your first assignment you decided to use the mapping of directory-database and file-table, and if in your second assignment you followed the following physical layout of for an example table <strong><em>Product (pid, name, price)</em></strong> pid int | name varchar(20) | price float

  <ul>

   <li>| laptop | 1999.99</li>

   <li>| mobile phone | 899.99 3 | monitor | 1399.99 then the pseudocode for a join could be (omitting the column headers):</li>

  </ul></li>

</ul>

for each line of table_file1     for each line of table_file2

check the condition parsed from the given query

<h1>Implementation</h1>

<ul>

 <li>The program should not use external database library/application.</li>

 <li>The program should persist metadata and data somewhere (e.g., local file system, cloud storage).</li>

 <li>Any programming language is acceptable, e.g., Python, Java, C/C++, Go o Just pick one(s) that you are most comfortable/proficient with</li>

</ul>

o But keep in mind we will test your code in Linux with OS-level utilities (e.g., files) &#x25aa;           So, probably not: C#, Object-C, JavaScript, Prolog…

<ul>

 <li>Functionalities: o SQL: inner join, left outer join</li>

</ul>

<strong> </strong>




<strong> </strong>

<h1>Interface</h1>

<ul>

 <li>A similar interface than Sqlite3</li>

 <li>Please contact the TA if you are unsure about your programming interface.</li>

</ul>

<h1>Testing</h1>

<ul>

 <li>We will test your program on Ubuntu (version 14 or above)</li>

 <li>If the TA cannot compile your code, you will be asked to demo its compilation and execution o Try not to use many exotic libraries and/or heavy frameworks.</li>

 <li>A full test script will be provided o # ~/cs457/pa3/[your_program] &lt;sql (if your program supports redirection) o # [expected output] o You don’t need to parse the comment lines (i.e., starting with “- -“) o We will not to test your programs with any other scripts</li>

</ul>

&#x25aa;   It’s always good to consider more corner cases

<h1>Grading (20 points)</h1>

<ul>

 <li>This is an individual assignment</li>

 <li>Design document that clarifies the followings: (5 points) o At a very high level, how you implement different joins.</li>

</ul>

o Be very specific on how to compile and execute your code

<ul>

 <li>Source code (15 points) o Coding style and clarity, 5 points

  <ul>

   <li>Appropriate parenthesis locations, indention, etc.</li>

   <li>Always write comments at the beginning of any files</li>

  </ul></li>

 <li>Author, date, history, etc.</li>

</ul>

&#x25aa;   Always write comments at the beginning of any non-trivial class/function

<ul>

 <li>What this class/function does, high-level algorithm if needed

  <ul>

   <li>Write in-line comments for non-trivial blocks of code o Functionality, 10 points</li>

   <li>Refer to the test script for detailed breakdowns</li>

  </ul></li>

</ul>

<h1>Submission</h1>

<ul>

 <li>WebCampus</li>

 <li>Compress all your source code and documents into one package in this format:</li>

</ul>

o &lt;your_netid&gt;_pa3

<ul>

 <li>Late penalty: 10% per day</li>

</ul>


