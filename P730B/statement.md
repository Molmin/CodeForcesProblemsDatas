## Description

<div><p><span class="tex-font-style-it">This is an interactive problem. You have to use <span class="tex-font-style-tt">flush</span> operation right after printing each line. For example, in C++ you should use function <span class="tex-font-style-tt">fflush(stdout)</span>, in Java — <span class="tex-font-style-tt">System.out.flush()</span>, in Pascal — <span class="tex-font-style-tt">flush(output)</span> and in Python — <span class="tex-font-style-tt">sys.stdout.flush()</span>.</span></p><p>In this problem, you need to find maximal and minimal elements of an array. What could be simpler?</p><p>You can imagine that the jury has an array, and initially you know the only number <span class="tex-span"><i>n</i></span> — array's length.</p><p>Array's elements are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. You are allowed to compare two elements of the array by using their indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. There are three possible responses to this query: '<span class="tex-font-style-tt">&lt;</span>' (if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is less than <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>), '<span class="tex-font-style-tt">=</span>' (if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>) and finally '<span class="tex-font-style-tt">&gt;</span>' (if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is greater than <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>).</p><p>It's known that it's always possible to find both maximal and minimal elements of the array by using no more than <img align="middle" class="tex-formula" src="file://NAtvoldA.png" style="max-width: 100.0%;max-height: 100.0%;"> comparisons, where <span class="tex-span">⌈ <i>x</i>⌉</span> is the result of rounding <span class="tex-span"><i>x</i></span> up.</p><p>Write the program that will find positions of the minimum and the maximum in the jury's array of length <span class="tex-span"><i>n</i></span>, by using no more than <span class="tex-span"><i>f</i>(<i>n</i>)</span> comparisons.</p></div><div><h2>Interaction</h2><p>Each test for this problem will contain one or more arrays. You have to find positions of minimal and maximal elements for each of these arrays. The first line of the input contains integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 1000</span>) — number of arrays in the test.</p><p>Thus, at the beginning, you program should read number <span class="tex-span"><i>T</i></span>, and then it should solve the problem for <span class="tex-span"><i>T</i></span> jury's arrays one by one.</p><p>Then input for each array goes. Firstly, your program has to read the number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the length of the array. It will be provided in the next line of the input.</p><p>Further, your program can perform comparisons or report that the answer is found.</p><ul> <li> To perform a comparison, you have to output string of the following pattern «<span class="tex-font-style-tt">? i j</span>» (<span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> must be integer numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>) — the indices of the elements to compare in the current query. </li><li> To report the indices of minimal and maximal elements of the hidden array, your program have to output a line in the form «<span class="tex-font-style-tt">! i j</span>» (<span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> must be integer numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>), where <span class="tex-span"><i>i</i></span> is an index of the minimal element of array, and <span class="tex-span"><i>j</i></span> is an index of the maximal element of the array. If there are several possible answers to the problem, you can output any of them. </li></ul><p>There are several possible responses for a comparison:</p><ul> <li> '<span class="tex-font-style-tt">&lt;</span>' — if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is less than <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, </li><li> '<span class="tex-font-style-tt">=</span>' — if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, </li><li> '<span class="tex-font-style-tt">&gt;</span>' — if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is greater than <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>. </li></ul><p>For an array of length <span class="tex-span"><i>n</i></span> your program can make at most <img align="middle" class="tex-formula" src="file://ZPgAIjzu.png" style="max-width: 100.0%;max-height: 100.0%;"> comparisons. Note that the operation of reporting an answer («<span class="tex-font-style-tt">! i j</span>» ) is not included into the value of <span class="tex-span"><i>f</i>(<i>n</i>)</span>.</p><p>After the answer is reported, your program has to solve the problem for the next array or it should terminate if all <span class="tex-span"><i>T</i></span> arrays are processed.</p></div>





```input1
2
2
&nbsp;
&gt;
&nbsp;
3
&nbsp;
=
&nbsp;
=
&nbsp;
```




```output1
&nbsp;
&nbsp;
? 1 2
&nbsp;
! 2 1
&nbsp;
? 3 1
&nbsp;
? 2 1
&nbsp;
! 2 3
```


