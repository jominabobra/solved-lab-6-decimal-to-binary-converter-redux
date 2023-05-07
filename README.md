Download Link: https://assignmentchef.com/product/solved-lab-6-decimal-to-binary-converter-redux
<br>
<strong>Lab Objectives: </strong>

With some time spent in MIPS and specifically to do with hardware, we are now going to code something more complex, but very familiar.  We are going to make another decimal to binary converter.  This one will not accept input from the keyboard but will instead read a string from memory.  Serial communications are always tricky to get right in embedded applications and this will make the program much easier to work with.




<strong>Part 1: </strong>

Refer back to your flowchart for Lab 3 and think about how you would do it with the extra operations now available to you.  Revise your flowchart to leverage these new features being sure to use the shift operators instead of loading masks.

The loops should be easier and being able to directly compare registers will make life easier.




<strong>Part 2: </strong>

We have given a starter file that handles the setup for you.  If you run this file without any added code it will print out the incoming number and the string where you will be storing the binary string.  You should only need to add code between the two comments and should not need to add any output but feel free to customize the welcome message if you desire.  Implement your new flowchart ensuring that it works with a wide range of numbers.

<ul>

 <li>Remember that the Uno32 is 32-bit, not 16.</li>

 <li>The input string is of unknown length but is properly terminated.</li>

 <li>The output string is 32 bits long.</li>

 <li><em>inNumericString</em> holds the input string and <em>outBinaryString</em> holds the binary string. o The binary string is initialized to all ‘z’’s.</li>

 <li>Some Useful Assembly Commands:

  <ul>

   <li>MUL: This will multiply two registers together. As the end number needs to fit in 32 bits we don’t need to use the full MULT.</li>

   <li>SB/LB: Allows loading and storing of bytes instead of words</li>

   <li>SLR: Shifts all the bits of a register to the right. This allows us to instead of making static masks to shift the bit over instead to generate our new mask.</li>

   <li>The different branch commands to make this process simpler. o SLTU is also very useful, read the documentation on what it does.</li>

  </ul></li>

</ul>

<h1>Lab Requirements</h1>

You must do the following for this lab:

<ul>

 <li>Convert decimal strings to binary leveraging the advanced features of MIPS.</li>

 <li>Demonstrate this ability for any number given by the Teaching staff.</li>

</ul>