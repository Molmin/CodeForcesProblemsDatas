## Description

<div><p>Yaroslav likes algorithms. We'll describe one of his favorite algorithms.</p><ol> <li> The algorithm receives a string as the input. We denote this input string as <span class="tex-span"><i>a</i></span>. </li><li> The algorithm consists of some number of command. Сommand number <span class="tex-span"><i>i</i></span> looks either as <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-font-style-tt">&gt;&gt;</span> <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, or as <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-font-style-tt">&lt;&gt;</span> <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> are some possibly empty strings of length at most <span class="tex-span">7</span>, consisting of digits and characters "<span class="tex-font-style-tt">?</span>". </li><li> At each iteration, the algorithm looks for a command with the minimum index <span class="tex-span"><i>i</i></span>, such that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> occurs in <span class="tex-span"><i>a</i></span> as a substring. If this command is not found the algorithm terminates. </li><li> Let's denote the number of the found command as <span class="tex-span"><i>k</i></span>. In string <span class="tex-span"><i>a</i></span> the first occurrence of the string <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span> is replaced by string <span class="tex-span"><i>w</i><sub class="lower-index"><i>k</i></sub></span>. If the found command at that had form <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-font-style-tt">&gt;&gt;</span> <span class="tex-span"><i>w</i><sub class="lower-index"><i>k</i></sub></span>, then the algorithm continues its execution and proceeds to the next iteration. Otherwise, the algorithm terminates. </li><li> The value of string <span class="tex-span"><i>a</i></span> after algorithm termination is considered to be the output of the algorithm. </li></ol><p>Yaroslav has a set of <span class="tex-span"><i>n</i></span> positive integers, he needs to come up with his favorite algorithm that will increase each of the given numbers by one. More formally, if we consider each number as a string representing the decimal representation of the number, then being run on each of these strings separately, the algorithm should receive the output string that is a recording of the corresponding number increased by one.</p><p>Help Yaroslav.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of elements in the set. The next <span class="tex-span"><i>n</i></span> lines contains one positive integer each. All the given numbers are less than <span class="tex-span">10<sup class="upper-index">25</sup></span>.</p></div><div class="output-specification"><p>Print the algorithm which can individually increase each number of the set. In the <span class="tex-span"><i>i</i></span>-th line print the command number <span class="tex-span"><i>i</i></span> without spaces.</p><p>Your algorithm will be launched for each of these numbers. The answer will be considered correct if: &nbsp; </p><ul> <li> Each line will a correct algorithm command (see the description in the problem statement). </li><li> The number of commands should not exceed <span class="tex-span">50</span>. </li><li> The algorithm will increase each of the given numbers by one. </li><li> To get a respond, the algorithm will perform no more than <span class="tex-span">200</span> iterations for each number. </li></ul></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of elements in the set. The next <span class="tex-span"><i>n</i></span> lines contains one positive integer each. All the given numbers are less than <span class="tex-span">10<sup class="upper-index">25</sup></span>.</p>

## Output

<p>Print the algorithm which can individually increase each number of the set. In the <span class="tex-span"><i>i</i></span>-th line print the command number <span class="tex-span"><i>i</i></span> without spaces.</p><p>Your algorithm will be launched for each of these numbers. The answer will be considered correct if: &nbsp; </p><ul> <li> Each line will a correct algorithm command (see the description in the problem statement). </li><li> The number of commands should not exceed <span class="tex-span">50</span>. </li><li> The algorithm will increase each of the given numbers by one. </li><li> To get a respond, the algorithm will perform no more than <span class="tex-span">200</span> iterations for each number. </li></ul>





```input1
2
10
79

```




```output1
10&lt;&gt;11
79&lt;&gt;80

```


