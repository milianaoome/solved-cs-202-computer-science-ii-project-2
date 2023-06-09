Download Link: https://assignmentchef.com/product/solved-cs-202-computer-science-ii-project-2
<br>



<strong> </strong>




<strong>Objectives:  </strong>The two main objectives of this project is to test your ability to (1) create and use structs with arrays, (2) work with pointers, pointer arithmetic, pass by-Value, pass by-Reference, pass by-Address, and (3) design, implement and test a solution to a given problem. A review of your knowledge of arrays, iostream, file I/O and C-style strings is also included.

<strong>Description: </strong>

For this project, you are to create a program that will assist users who want to rent a car. You are given a <strong>datafile with 5 different cars file</strong> (the file is a priori <u>known to have exactly 5</u> entries, each following the <u>same data layout</u>), and you must <strong>read in</strong> <strong>all</strong> of the <strong>car data</strong> from the <strong>file</strong> and <strong>store</strong> it in an <strong>array of structs</strong>. You must also <strong>create a menu</strong> with the functionality defined below. Although an example file is provided (Cars.txt), for grading purposes your project will be tested against a different test file that will not be provided to you beforehand. Our test file will be in the same format as the example file.




<strong>The RentalCar struct will contain the following data members: </strong>

<ul>

 <li><strong>year</strong>, an int (year of production)</li>

 <li><strong>make</strong>, a C-string (char array of 10 maximum size)</li>

 <li><strong>model</strong>, a C-string (char array of 10 maximum size)</li>

 <li><strong>price</strong>, a float (price per day)</li>

 <li><strong>available</strong>, a bool (1 = true; 0 = false; try to display true/false using the</li>

</ul>

“std::boolalpha” manipulator like: cout &lt;&lt; boolalpha &lt;&lt; boolVariable; )




<strong>The menu must have the following entries, each implementing a functionality: </strong>

<ul>

 <li><strong>1) Ask</strong> the user for the<strong> input file name</strong>, and then <strong>read ALL</strong> data from that <strong>file</strong>. The data have to be stored into an <strong>array of structs</strong>.</li>

 <li><strong>2) Print out ALL</strong> data for all of the cars to the <strong>terminal</strong>.</li>

 <li><strong>3) Print out ALL</strong> data for all of the cars to a <strong>separate output file</strong> (when the user chooses menu entry 2, they should also get <strong>asked</strong> for an <strong>output file name</strong>).</li>

 <li><strong>4) Sort </strong>the cars (i.e. sort the array of structs) by <strong>ascending price</strong>.</li>

 <li><strong>5) Ask </strong>the user for <strong>how many days</strong> they want to rent a car. Then <strong>print to the terminal </strong><strong>only the available</strong> cars, <strong>sorted</strong> by ascending price, as well as the <strong>total estimated cost</strong> to make the rent (number of days multiplied by price per day).</li>

 <li><strong>6) Ask </strong>the user <strong>which car</strong> they want to rent (expected user input is an <strong>index number</strong> for the array of structs) and for <strong>how many days</strong>. If the corresponding car is <strong>not available</strong>, print a <strong>warning message</strong> to <strong>terminal</strong>. If it is <strong>available</strong>, mark it as rented (modify the available member appropriately) and print out to <strong>terminal</strong> a <strong>success message</strong> that mentions the <strong>total cost</strong> (number of days multiplied by price per day).</li>

 <li><strong>7) Exit</strong></li>

</ul>




<strong> </strong>

<strong>The following minimum functionality and structure is required: </strong>

<ul>

 <li>Ask the <strong>user</strong> for the <strong>input file </strong></li>

 <li>The list of cars must be stored in an <strong>array of structs</strong>.</li>

 <li>Use <strong>character arrays</strong> to hold your strings (i.e., C-style) exclusively (using the string data type is still not allowed).</li>

 <li>Write <strong>multiple functions</strong> (Hint: each menu option should be a function).</li>

 <li>You are free to use <strong>pass by-Value, pass by-Reference</strong>, <strong>pass by-Address</strong> for your function parameters. (<em>Note</em>: Remember that using pass by-Value will make the function work on a local internal copy of whatever variable you pass as an argument, therefore the change will not be made on the actual argument itself, and it will be left unaffected after the function call is complete).</li>

 <li>Write your <strong>own C-string copy</strong>, <strong>C-string compare</strong> Their prototypes will have the form (you must use the prototypes exactly as provided, with <strong>char *</strong> parameters):</li>

</ul>

<strong>// copies characters from source to destination until a NULLcharacter ‘ ’ is found in source, then it NULL-terminates destination too, and returns  </strong><strong>void</strong> <strong>myStringCopy</strong><strong>(</strong><strong>char *</strong><strong> destination, </strong><strong>const char * </strong><strong>source);</strong>

<strong> </strong>

<strong>// returns 0 when the strings match, i.e. their characters are equal one-by-one until a NULL-character ‘ ’ is found in both strings and at the same position as well </strong>

<strong>// returns a value &lt;1 if the first character that does not match has a lower value in str1 than in str2 </strong>

<strong>// returns a value &gt;1 if the first character that does not match has a higher value in str1 than in str2  </strong><strong>int </strong><strong>myStringCompare</strong><strong>(</strong><strong>const char *</strong><strong> str1, </strong><strong>const char *</strong><strong> str2);</strong>




<sup>  </sup>Ø The other functionality and structure of the program should remain the <strong>same as Project #1</strong>, including <strong>writing to screen</strong> and <strong>file</strong> and<strong> restrictions on string</strong> libraries, <strong>global variables</strong> and <strong>constants</strong>, etc.




<strong>Sample Output for menu option 2 (before sorting the array by ascending price): </strong>




<ul>

 <li>Toyota Tacoma , $115.12 per day , Available: false</li>

</ul>




<ul>

 <li>Ford Fusion , $90.89 per day , Available: true</li>

</ul>




2009 Dodge Neon , $45.25 per day , Available: false




<ul>

 <li>Ford F150 , $112.83 per day , Available: true</li>

</ul>




<ul>

 <li>Subaru Outback , $71.27 per day , Available: true</li>

</ul>




<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong>Sample Output for menu option 5 (for 2 days of renting, only showing available ones, and with the array already sorted by ascending price): </strong>




2016 Subaru Outback , Total Cost: $142.54




2015 Ford Fusion , Total Cost: $181.78




2015 Ford F150 , Total Cost: $225.66

<strong> </strong>

<strong> </strong>

<strong>The completed project should have the following properties: </strong> Ø Written, compiled and tested using Linux.

<ul>

 <li>It must compile successfully using the g++ compiler on department machines. Instructions how to remotely connect to department machines are included in the Projects folder in WebCampus.</li>

 <li>The code must be commented and indented properly.</li>

</ul>

Header comments are required on all files and recommended for the rest of the program. Descriptions of functions commented properly.

<ul>

 <li>A one page (minimum) typed sheet documenting your code. This should include the overall purpose of the program, your design, problems (if any), and any changes you would make given more time.</li>

</ul>




<strong>Turn in:</strong> Compressed .cpp file and project documentation.
































