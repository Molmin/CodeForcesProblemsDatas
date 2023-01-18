## Description

<div><p>Vasya is developing his own programming language VPL (Vasya Programming Language). Right now he is busy making the system of exceptions. He thinks that the system of exceptions must function like that.</p><p>The exceptions are processed by try-catch-blocks. There are two operators that work with the blocks:</p><ol><li> The <span class="tex-font-style-tt">try</span> operator. It opens a new try-catch-block. </li><li> The <span class="tex-font-style-tt">catch(&lt;exception_type&gt;, &lt;message&gt;)</span> operator. It closes the try-catch-block that was started last and haven't yet been closed. This block can be activated only via exception of type &lt;exception_type&gt;. When we activate this block, the screen displays the &lt;message&gt;. If at the given moment there is no open try-catch-block, then we can't use the <span class="tex-font-style-tt">catch</span> operator.</li></ol><p>The exceptions can occur in the program in only one case: when we use the <span class="tex-font-style-tt">throw</span> operator. The <span class="tex-font-style-tt">throw(&lt;exception_type&gt;)</span> operator creates the exception of the given type.</p><p>Let's suggest that as a result of using some <span class="tex-font-style-tt">throw</span> operator the program created an exception of type <span class="tex-span"><i>a</i></span>. In this case a try-catch-block is activated, such that this block's <span class="tex-font-style-tt">try</span> operator was described in the program earlier than the used <span class="tex-font-style-tt">throw</span> operator. Also, this block's <span class="tex-font-style-tt">catch</span> operator was given an exception type <span class="tex-span"><i>a</i></span> as a parameter and this block's <span class="tex-font-style-tt">catch</span> operator is described later that the used <span class="tex-font-style-tt">throw</span> operator. If there are several such try-catch-blocks, then the system activates the block whose <span class="tex-font-style-tt">catch</span> operator occurs earlier than others. If no try-catch-block was activated, then the screen displays message "<span class="tex-font-style-tt">Unhandled Exception</span>".</p><p>To test the system, Vasya wrote a program that contains only <span class="tex-font-style-tt">try</span>, <span class="tex-font-style-tt">catch</span> and <span class="tex-font-style-tt">throw</span> operators, one line contains no more than one operator, the whole program contains exactly one <span class="tex-font-style-tt">throw</span> operator.</p><p>Your task is: given a program in VPL, determine, what message will be displayed on the screen.</p></div><div class="input-specification"><p>The first line contains a single integer: <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> the number of lines in the program. Next <span class="tex-span"><i>n</i></span> lines contain the program in language VPL. Each line contains no more than one operator. It means that input file can contain empty lines and lines, consisting only of spaces.</p><p>The program contains only operators <span class="tex-font-style-tt">try</span>, <span class="tex-font-style-tt">catch</span> and <span class="tex-font-style-tt">throw</span>. It is guaranteed that the program is correct. It means that each started try-catch-block was closed, the <span class="tex-font-style-tt">catch</span> operators aren't used unless there is an open try-catch-block. The program has exactly one <span class="tex-font-style-tt">throw</span> operator. The program may have spaces at the beginning of a line, at the end of a line, before and after a bracket, a comma or a quote mark.</p><p>The exception type is a nonempty string, that consists only of upper and lower case english letters. The length of the string does not exceed 20 symbols. Message is a nonempty string, that consists only of upper and lower case english letters, digits and spaces. Message is surrounded with quote marks. Quote marks shouldn't be printed. The length of the string does not exceed 20 symbols.</p><p>Length of any line in the input file does not exceed 50 symbols. </p></div><div class="output-specification"><p>Print the message the screen will show after the given program is executed.</p></div>

## Input

<p>The first line contains a single integer: <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> the number of lines in the program. Next <span class="tex-span"><i>n</i></span> lines contain the program in language VPL. Each line contains no more than one operator. It means that input file can contain empty lines and lines, consisting only of spaces.</p><p>The program contains only operators <span class="tex-font-style-tt">try</span>, <span class="tex-font-style-tt">catch</span> and <span class="tex-font-style-tt">throw</span>. It is guaranteed that the program is correct. It means that each started try-catch-block was closed, the <span class="tex-font-style-tt">catch</span> operators aren't used unless there is an open try-catch-block. The program has exactly one <span class="tex-font-style-tt">throw</span> operator. The program may have spaces at the beginning of a line, at the end of a line, before and after a bracket, a comma or a quote mark.</p><p>The exception type is a nonempty string, that consists only of upper and lower case english letters. The length of the string does not exceed 20 symbols. Message is a nonempty string, that consists only of upper and lower case english letters, digits and spaces. Message is surrounded with quote marks. Quote marks shouldn't be printed. The length of the string does not exceed 20 symbols.</p><p>Length of any line in the input file does not exceed 50 symbols. </p>

## Output

<p>Print the message the screen will show after the given program is executed.</p>





```input1
8
try
    try
        throw ( AE ) 
    catch ( BE, "BE in line 3")

    try
    catch(AE, "AE in line 5") 
catch(AE,"AE somewhere")

```




```input2
8
try
    try
        throw ( AE ) 
    catch ( AE, "AE in line 3")

    try
    catch(BE, "BE in line 5") 
catch(AE,"AE somewhere")

```




```input3
8
try
    try
        throw ( CE ) 
    catch ( BE, "BE in line 3")

    try
    catch(AE, "AE in line 5") 
catch(AE,"AE somewhere")

```




```output1
AE somewhere

```




```output2
AE in line 3

```




```output3
Unhandled Exception

```



## Note

<p>In the first sample there are 2 try-catch-blocks such that <span class="tex-font-style-tt">try</span> operator is described earlier than <span class="tex-font-style-tt">throw</span> operator and <span class="tex-font-style-tt">catch</span> operator is described later than <span class="tex-font-style-tt">throw</span> operator: <span class="tex-font-style-tt">try-catch(BE,"BE in line 3")</span> and <span class="tex-font-style-tt">try-catch(AE,"AE somewhere")</span>. Exception type is AE, so the second block will be activated, because operator <span class="tex-font-style-tt">catch(AE,"AE somewhere")</span> has exception type AE as parameter and operator <span class="tex-font-style-tt">catch(BE,"BE in line 3")</span> has exception type BE.</p><p>In the second sample there are 2 try-catch-blocks such that <span class="tex-font-style-tt">try</span> operator is described earlier than <span class="tex-font-style-tt">throw</span> operator and <span class="tex-font-style-tt">catch</span> operator is described later than <span class="tex-font-style-tt">throw</span> operator: <span class="tex-font-style-tt">try-catch(AE,"AE in line 3")</span> and <span class="tex-font-style-tt">try-catch(AE,"AE somewhere")</span>. Exception type is AE, so both blocks can be activated, but only the first one will be activated, because operator <span class="tex-font-style-tt">catch(AE,"AE in line 3")</span> is described earlier than <span class="tex-font-style-tt">catch(AE,"AE somewhere")</span></p><p>In the third sample there is no blocks that can be activated by an exception of type CE.</p>
