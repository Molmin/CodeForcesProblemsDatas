## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Imur Ishakov decided to organize a club for people who love to play the famous game «The hat». The club was visited by <span class="tex-span"><i>n</i></span> students, where <span class="tex-span"><i>n</i></span> is even. Imur arranged them all in a circle and held a draw to break the students in pairs, but something went wrong. The participants are numbered so that participant <span class="tex-span"><i>i</i></span> and participant <span class="tex-span"><i>i</i> + 1</span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>) are adjacent, as well as participant <span class="tex-span"><i>n</i></span> and participant <span class="tex-span">1</span>. Each student was given a piece of paper with a number in such a way, that for every two adjacent students, these numbers differ exactly by one. The plan was to form students with the same numbers in a pair, but it turned out that not all numbers appeared exactly twice.</p><p>As you know, the most convenient is to explain the words to the partner when he is sitting exactly across you. Students with numbers <span class="tex-span"><i>i</i></span> and <img align="middle" class="tex-formula" src="file://Jyk5uLDA.png" style="max-width: 100.0%;max-height: 100.0%;"> sit across each other. Imur is wondering if there are two people sitting across each other with the same numbers given. Help him to find such pair of people if it exists.</p><p>You can ask questions of form «which number was received by student <span class="tex-span"><i>i</i></span>?», and the goal is to determine whether the desired pair exists in no more than <span class="tex-span">60</span> questions.</p></div><div class="input-specification"><p>At the beginning the even integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) is given&nbsp;— the total number of students.</p><p>You are allowed to ask no more than <span class="tex-span">60</span> questions.</p></div><div class="output-specification"><p>To ask the question about the student <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), you should print «<span class="tex-font-style-tt">? <span class="tex-span"><i>i</i></span></span>». Then from standard output you can read the number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> received by student <span class="tex-span"><i>i</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>When you find the desired pair, you should print «<span class="tex-font-style-tt">! <span class="tex-span"><i>i</i></span></span>», where <span class="tex-span"><i>i</i></span> is any student who belongs to the pair (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). If you determined that such pair doesn't exist, you should output «<span class="tex-font-style-tt">! -1</span>». In both cases you should immediately terminate the program.</p><p>The query that contains your answer is not counted towards the limit of <span class="tex-span">60</span> queries.</p><p>Please make sure to flush the standard output after each command. For example, in C++ use function <span class="tex-font-style-tt">fflush(stdout)</span>, in Java call <span class="tex-font-style-tt">System.out.flush()</span>, in Pascal use <span class="tex-font-style-tt">flush(output)</span> and <span class="tex-font-style-tt">stdout.flush()</span> for Python language.</p><p><span class="tex-font-style-bf">Hacking</span></p><p>Use the following format for hacking:</p><p>In the first line, print one even integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the total number of students.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) separated by spaces, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number to give to <span class="tex-span"><i>i</i></span>-th student. Any two adjacent elements, including <span class="tex-span"><i>n</i></span> and <span class="tex-span">1</span>, must differ by <span class="tex-span">1</span> or <span class="tex-span"> - 1</span>.</p><p>The hacked solution will not have direct access to the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>At the beginning the even integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) is given&nbsp;— the total number of students.</p><p>You are allowed to ask no more than <span class="tex-span">60</span> questions.</p>

## Output

<p>To ask the question about the student <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), you should print «<span class="tex-font-style-tt">? <span class="tex-span"><i>i</i></span></span>». Then from standard output you can read the number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> received by student <span class="tex-span"><i>i</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>When you find the desired pair, you should print «<span class="tex-font-style-tt">! <span class="tex-span"><i>i</i></span></span>», where <span class="tex-span"><i>i</i></span> is any student who belongs to the pair (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). If you determined that such pair doesn't exist, you should output «<span class="tex-font-style-tt">! -1</span>». In both cases you should immediately terminate the program.</p><p>The query that contains your answer is not counted towards the limit of <span class="tex-span">60</span> queries.</p><p>Please make sure to flush the standard output after each command. For example, in C++ use function <span class="tex-font-style-tt">fflush(stdout)</span>, in Java call <span class="tex-font-style-tt">System.out.flush()</span>, in Pascal use <span class="tex-font-style-tt">flush(output)</span> and <span class="tex-font-style-tt">stdout.flush()</span> for Python language.</p><p><span class="tex-font-style-bf">Hacking</span></p><p>Use the following format for hacking:</p><p>In the first line, print one even integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the total number of students.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) separated by spaces, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number to give to <span class="tex-span"><i>i</i></span>-th student. Any two adjacent elements, including <span class="tex-span"><i>n</i></span> and <span class="tex-span">1</span>, must differ by <span class="tex-span">1</span> or <span class="tex-span"> - 1</span>.</p><p>The hacked solution will not have direct access to the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
8
<span class="tex-span"></span>
2
<span class="tex-span"></span>
2

```




```input2
6
<span class="tex-span"></span>
1
<span class="tex-span"></span>
2
<span class="tex-span"></span>
3 
<span class="tex-span"></span>
2
<span class="tex-span"></span>
1
<span class="tex-span"></span>
0
```




```output1
<span class="tex-span"></span>
? 4
<span class="tex-span"></span>
? 8
<span class="tex-span"></span>
! 4

```




```output2
<span class="tex-span"></span>
? 1
<span class="tex-span"></span>
? 2
<span class="tex-span"></span>
? 3
<span class="tex-span"></span>
? 4
<span class="tex-span"></span>
? 5
<span class="tex-span"></span>
? 6
<span class="tex-span"></span>
! -1
```



## Note

<p>Input-output in statements illustrates example interaction.</p><p>In the first sample the selected sequence is <span class="tex-span">1, 2, 1, 2, 3, 4, 3, 2</span></p><p>In the second sample the selection sequence is <span class="tex-span">1, 2, 3, 2, 1, 0</span>.</p>
