## Description

<div><p>Two good friends were trying to make a new programming language called Perse-script.</p><p>The most important part of this language is <span class="tex-font-style-underline">strings</span>. A string in Perse-script is put between characters <span class="tex-font-style-tt">"</span></p><p>So for example <span class="tex-font-style-tt">"Hello"</span> is a string. But <span class="tex-font-style-tt">Hello</span> is a variable name or a keyword, which are not considered in this problem.</p><p>Perse-script is function-based. So there are no operators in this language. For example for summing two numbers you have to write <span class="tex-font-style-tt">sum(a,b)</span> and not <span class="tex-font-style-tt">a+b</span>.</p><p>There are several functions for working on strings. These include: </p><ul> <li> <span class="tex-font-style-tt">concat(x,y)</span> is a function which gets two strings <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> and puts <span class="tex-span"><i>y</i></span> at the end of <span class="tex-span"><i>x</i></span> and returns the result. For example <span class="tex-font-style-tt">concat("Hello","World")</span> returns <span class="tex-font-style-tt">"HelloWorld"</span>. </li><li> <span class="tex-font-style-tt">reverse(x)</span> gets a single string <span class="tex-span"><i>x</i></span> and reverses it. For example <span class="tex-font-style-tt">reverse("Hello")</span> returns <span class="tex-font-style-tt">"olleH"</span>. </li><li> <span class="tex-font-style-tt">substr(x,a,b)</span> gets a string <span class="tex-span"><i>x</i></span> and two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>n</i></span>, where <span class="tex-span"><i>n</i></span> is the length of <span class="tex-span"><i>x</i></span>). And returns the substring of <span class="tex-span"><i>x</i></span> between indexes <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, inclusive. For example <span class="tex-font-style-tt">substr("Hello",2,4)</span> returns <span class="tex-font-style-tt">"ell"</span>. </li><li> <span class="tex-font-style-tt">substr(x,a,b,c)</span> is another version of substr which works just like the last one but <span class="tex-span"><i>c</i></span> is the step of adding. <span class="tex-span"><i>c</i></span> is <span class="tex-font-style-underline">positive</span>. For example <span class="tex-font-style-tt">substr("HelloWorld",1,10,2)</span> returns <span class="tex-font-style-tt">"Hlool"</span>. This substr means that you put the <span class="tex-span"><i>a</i></span>th character , and then every <span class="tex-span"><i>c</i></span>th character until you reach <span class="tex-span"><i>b</i></span>.</li></ul><p>You're going to manipulate the string part of Perse-script. Given a string expression, you should print its result. It is guaranteed that the expression contains only strings shown by characters <span class="tex-font-style-tt">"</span> and the above functions.</p><p>Commands in Perse-script are case-insensitive. So to call <span class="tex-font-style-tt">substr</span> function you can write <span class="tex-font-style-tt">SUBsTr()</span>. But you can't print as the result <span class="tex-font-style-tt">"hElLo"</span> instead of printing <span class="tex-font-style-tt">"Hello"</span>.</p><p>See the samples for more information.</p></div><div class="input-specification"><p>A single line containing the correct expression. It is guaranteed that the total length of this expression does not exceed <span class="tex-span">10<sup class="upper-index">3</sup></span> and that all the integers used in it are less than or equal to <span class="tex-span">100</span> by absolute value. The given string is non-empty.</p><p>All strings in the input which are placed between <span class="tex-font-style-tt">"</span>s consist of uppercase and lowercase Latin letters only.</p></div><div class="output-specification"><p>Print in single line the resulting string. It is guaranteed that an answer exists and that the length of the answer does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. It is guaranteed that the answer is non-empty.</p></div>

## Input

<p>A single line containing the correct expression. It is guaranteed that the total length of this expression does not exceed <span class="tex-span">10<sup class="upper-index">3</sup></span> and that all the integers used in it are less than or equal to <span class="tex-span">100</span> by absolute value. The given string is non-empty.</p><p>All strings in the input which are placed between <span class="tex-font-style-tt">"</span>s consist of uppercase and lowercase Latin letters only.</p>

## Output

<p>Print in single line the resulting string. It is guaranteed that an answer exists and that the length of the answer does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. It is guaranteed that the answer is non-empty.</p>





```input1
"HelloWorld"

```




```input2
REVerse(substr("helloworld",1,5))

```




```input3
conCAT(rEveRSE("olleh"),"world")

```




```input4
reversE(concAT(substr("hello",1,2),sUbstr("world",1,5,1)))

```




```input5
suBstr("Noruz",1,4,2)

```




```output1
"HelloWorld"

```




```output2
"olleh"

```




```output3
"helloworld"

```




```output4
"dlroweh"

```




```output5
"Nr"

```


