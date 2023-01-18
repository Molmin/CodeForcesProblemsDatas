## Description

<div><p>Last week, Hamed learned about a new type of equations in his math class called Modular Equations. Lets define <span class="tex-span"><i>i</i></span> modulo <span class="tex-span"><i>j</i></span> as the remainder of division of <span class="tex-span"><i>i</i></span> by <span class="tex-span"><i>j</i></span> and denote it by <img align="middle" class="tex-formula" src="file://TQ1igQh2.png" style="max-width: 100.0%;max-height: 100.0%;">. A Modular Equation, as Hamed's teacher described, is an equation of the form <img align="middle" class="tex-formula" src="file://gdvpohgn.png" style="max-width: 100.0%;max-height: 100.0%;"> in which <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are two non-negative integers and <span class="tex-span"><i>x</i></span> is a variable. We call a positive integer <span class="tex-span"><i>x</i></span> for which <img align="middle" class="tex-formula" src="file://8zoPggCE.png" style="max-width: 100.0%;max-height: 100.0%;"> a <span class="tex-font-style-underline">solution</span> of our equation.</p><p>Hamed didn't pay much attention to the class since he was watching a movie. He only managed to understand the definitions of these equations.</p><p>Now he wants to write his math exercises but since he has no idea how to do that, he asked you for help. He has told you all he knows about Modular Equations and asked you to write a program which given two numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> determines how many answers the Modular Equation <img align="middle" class="tex-formula" src="file://AlA5vqMR.png" style="max-width: 100.0%;max-height: 100.0%;"> has.</p></div><div class="input-specification"><p>In the only line of the input two space-separated integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>) are given.</p></div><div class="output-specification"><p>If there is an infinite number of answers to our equation, print "infinity" (without the quotes). Otherwise print the number of solutions of the Modular Equation <img align="middle" class="tex-formula" src="file://QYwYpZ1k.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>In the only line of the input two space-separated integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>) are given.</p>

## Output

<p>If there is an infinite number of answers to our equation, print "infinity" (without the quotes). Otherwise print the number of solutions of the Modular Equation <img align="middle" class="tex-formula" src="file://QYwYpZ1k.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
21 5

```




```input2
9435152 272

```




```input3
10 10

```




```output1
2

```




```output2
282

```




```output3
infinity

```



## Note

<p>In the first sample the answers of the Modular Equation are 8 and 16 since <img align="middle" class="tex-formula" src="file://L2QxDCXQ.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
