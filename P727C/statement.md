## Description

<div><p><span class="tex-font-style-it">This is an interactive problem. You should use <span class="tex-font-style-tt">flush</span> operation after each printed line. For example, in C++ you should use <span class="tex-font-style-tt">fflush(stdout)</span>, in Java you should use <span class="tex-font-style-tt">System.out.flush()</span>, and in Pascal&nbsp;— <span class="tex-font-style-tt">flush(output)</span>.</span></p><p>In this problem you should guess an array <span class="tex-span"><i>a</i></span> which is unknown for you. The only information you have initially is the length <span class="tex-span"><i>n</i></span> of the array <span class="tex-span"><i>a</i></span>.</p><p>The only allowed action is to ask the sum of two elements by their indices. Formally, you can print two indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (the indices should be <span class="tex-font-style-bf">distinct</span>). Then your program should read the response: the single integer equals to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>It is easy to prove that it is always possible to guess the array using at most <span class="tex-span"><i>n</i></span> requests.</p><p>Write a program that will guess the array <span class="tex-span"><i>a</i></span> by making at most <span class="tex-span"><i>n</i></span> requests.</p></div><div><h2>Interaction</h2><p>In each test your program should guess a single array.</p><p>The input starts with a line containing integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the length of the array. Your program should read it at first.</p><p>After that your program should print to the standard output the requests about the sum of two elements or inform that the array is guessed.</p><ul> <li> In case your program is making a request to ask the sum of two elements, it should print line in the format "<span class="tex-font-style-tt">? i j</span>" (<span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> are distinct integers between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>), where <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> are indices in the array <span class="tex-span"><i>a</i></span>.</li><li> In case your program informs that the array is guessed, it should print line in the format "<span class="tex-font-style-tt"><span class="tex-span">!&nbsp;<i>a</i><sub class="lower-index">1</sub>&nbsp;<i>a</i><sub class="lower-index">2</sub>&nbsp;...&nbsp;<i>a</i><sub class="lower-index"><i>n</i></sub></span></span>" (it is guaranteed that all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are positive integers not exceeding <span class="tex-span">10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th element of the array <span class="tex-span"><i>a</i></span>. </li></ul><p>The response on a request is a single integer equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>j</i></sub></span>, printed on a separate line.</p><p>Your program can do at most <span class="tex-span"><i>n</i></span> requests. Note that the final line «<span class="tex-font-style-tt"><span class="tex-span">!&nbsp;<i>a</i><sub class="lower-index">1</sub>&nbsp;<i>a</i><sub class="lower-index">2</sub>&nbsp;...&nbsp;<i>a</i><sub class="lower-index"><i>n</i></sub></span></span>» is not counted as a request.</p><p>Do not forget about <span class="tex-font-style-tt">flush</span> operation after each printed line.</p><p>After you program prints the guessed array, it should terminate normally.</p></div>





```input1
5
&nbsp;
9
&nbsp;
7
&nbsp;
9
&nbsp;
11
&nbsp;
6
&nbsp;
```




```output1
&nbsp;
? 1 5
&nbsp;
? 2 3
&nbsp;
? 4 1
&nbsp;
? 5 2
&nbsp;
? 3 4
&nbsp;
! 4 6 1 5 5
```



## Note

<p>The format of a test to make a hack is:</p><ul> <li> The first line contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the length of the array.</li><li> The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the elements of the array to guess. </li></ul>
