## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem. In the output section below you will see the information about flushing the output.</span></p><p>Bear Limak thinks of some hidden number&nbsp;— an integer from interval <span class="tex-span">[2, 100]</span>. Your task is to say if the hidden number is prime or composite.</p><p>Integer <span class="tex-span"><i>x</i> &gt; 1</span> is called prime if it has exactly two distinct divisors, <span class="tex-span">1</span> and <span class="tex-span"><i>x</i></span>. If integer <span class="tex-span"><i>x</i> &gt; 1</span> is not prime, it's called composite.</p><p>You can ask up to <span class="tex-span">20</span> queries about divisors of the hidden number. In each query you should print an integer from interval <span class="tex-span">[2, 100]</span>. The system will answer "<span class="tex-font-style-tt">yes</span>" if your integer is a divisor of the hidden number. Otherwise, the answer will be "<span class="tex-font-style-tt">no</span>".</p><p>For example, if the hidden number is <span class="tex-span">14</span> then the system will answer "<span class="tex-font-style-tt">yes</span>" only if you print <span class="tex-span">2</span>, <span class="tex-span">7</span> or <span class="tex-span">14</span>.</p><p>When you are done asking queries, print "<span class="tex-font-style-tt">prime</span>" or "<span class="tex-font-style-tt">composite</span>" and terminate your program.</p><p>You will get the <span class="tex-font-style-tt">Wrong Answer</span> verdict if you ask more than <span class="tex-span">20</span> queries, or if you print an integer not from the range <span class="tex-span">[2, 100]</span>. Also, you will get the <span class="tex-font-style-tt">Wrong Answer</span> verdict if the printed answer isn't correct.</p><p>You will get the <span class="tex-font-style-tt">Idleness Limit Exceeded</span> verdict if you don't print anything (but you should) or if you forget about flushing the output (more info below).</p></div><div class="input-specification"><p>After each query you should read one string from the input. It will be "<span class="tex-font-style-tt">yes</span>" if the printed integer is a divisor of the hidden number, and "<span class="tex-font-style-tt">no</span>" otherwise.</p></div><div class="output-specification"><p>Up to <span class="tex-span">20</span> times you can ask a query&nbsp;— print an integer from interval <span class="tex-span">[2, 100]</span> in one line. You have to both print the end-of-line character and <span class="tex-font-style-tt">flush</span> the output. After flushing you should read a response from the input.</p><p>In any moment you can print the answer "<span class="tex-font-style-tt">prime</span>" or "<span class="tex-font-style-tt">composite</span>" (without the quotes). After that, flush the output and terminate your program.</p><p>To flush you can use (just after printing an integer and end-of-line): </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> See the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacking.</span> To hack someone, as the input you should print the hidden number&nbsp;— one integer from the interval <span class="tex-span">[2, 100]</span>. Of course, his/her solution won't be able to read the hidden number from the input.</p></div>

## Input

<p>After each query you should read one string from the input. It will be "<span class="tex-font-style-tt">yes</span>" if the printed integer is a divisor of the hidden number, and "<span class="tex-font-style-tt">no</span>" otherwise.</p>

## Output

<p>Up to <span class="tex-span">20</span> times you can ask a query&nbsp;— print an integer from interval <span class="tex-span">[2, 100]</span> in one line. You have to both print the end-of-line character and <span class="tex-font-style-tt">flush</span> the output. After flushing you should read a response from the input.</p><p>In any moment you can print the answer "<span class="tex-font-style-tt">prime</span>" or "<span class="tex-font-style-tt">composite</span>" (without the quotes). After that, flush the output and terminate your program.</p><p>To flush you can use (just after printing an integer and end-of-line): </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> See the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacking.</span> To hack someone, as the input you should print the hidden number&nbsp;— one integer from the interval <span class="tex-span">[2, 100]</span>. Of course, his/her solution won't be able to read the hidden number from the input.</p>





```input1
yes
no
yes

```




```input2
no
yes
no
no
no

```




```output1
2
80
5
composite

```




```output2
58
59
78
78
2
prime

```



## Note

<p>The hidden number in the first query is <span class="tex-span">30</span>. In a table below you can see a better form of the provided example of the communication process.</p><p><img align="middle" class="tex-formula" src="file://7JjjVXxS.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The hidden number is divisible by both <span class="tex-span">2</span> and <span class="tex-span">5</span>. Thus, it must be composite. Note that it isn't necessary to know the exact value of the hidden number. In this test, the hidden number is <span class="tex-span">30</span>.</p><p><img align="middle" class="tex-formula" src="file://RPsf6UBX.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><span class="tex-span">59</span> is a divisor of the hidden number. In the interval <span class="tex-span">[2, 100]</span> there is only one number with this divisor. The hidden number must be <span class="tex-span">59</span>, which is prime. Note that the answer is known even after the second query and you could print it then and terminate. Though, it isn't forbidden to ask unnecessary queries (unless you exceed the limit of <span class="tex-span">20</span> queries).</p>
