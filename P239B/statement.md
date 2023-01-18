## Description

<div><p>There is a programming language in which every program is a non-empty sequence of "<span class="tex-font-style-tt">&lt;</span>" and "<span class="tex-font-style-tt">&gt;</span>" signs and digits. Let's explain how the interpreter of this programming language works. A program is interpreted using movement of instruction pointer (IP) which consists of two parts.</p><ul> <li> Current character pointer (CP); </li><li> Direction pointer (DP) which can point left or right; </li></ul><p>Initially CP points to the leftmost character of the sequence and DP points to the right.</p><p>We repeat the following steps until the first moment that CP points to somewhere outside the sequence.</p><ul> <li> If CP is pointing to a digit the interpreter prints that digit then CP moves one step according to the direction of DP. After that the value of the printed digit in the sequence decreases by one. If the printed digit was <span class="tex-span">0</span> then it cannot be decreased therefore it's erased from the sequence and the length of the sequence decreases by one. </li><li> If CP is pointing to "<span class="tex-font-style-tt">&lt;</span>" or "<span class="tex-font-style-tt">&gt;</span>" then the direction of DP changes to "left" or "right" correspondingly. Then CP moves one step according to DP. If the new character that CP is pointing to is "<span class="tex-font-style-tt">&lt;</span>" or "<span class="tex-font-style-tt">&gt;</span>" then the previous character will be erased from the sequence. </li></ul><p>If at any moment the CP goes outside of the sequence the execution is terminated.</p><p>It's obvious the every program in this language terminates after some steps.</p><p>We have a sequence <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> of "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>" and digits. You should answer <span class="tex-span"><i>q</i></span> queries. Each query gives you <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> and asks how many of each digit will be printed if we run the sequence <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i></sub>, <i>s</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>s</i><sub class="lower-index"><i>r</i></sub></span> as an independent program in this language.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>q</i> ≤ 100)</span> — represents the length of the sequence <span class="tex-span"><i>s</i></span> and the number of queries. </p><p>The second line contains <span class="tex-span"><i>s</i></span>, a sequence of "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>" and digits (<span class="tex-font-style-tt">0..9</span>) written from left to right. Note, that the characters of <span class="tex-span"><i>s</i></span> are not separated with spaces. </p><p>The next <span class="tex-span"><i>q</i></span> lines each contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>For each query print <span class="tex-span">10</span> space separated integers: <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index">9</sub></span> where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> equals the number of times the interpreter prints <span class="tex-span"><i>i</i></span> while running the corresponding program. Print answers to the queries in the order they are given in input.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>q</i> ≤ 100)</span> — represents the length of the sequence <span class="tex-span"><i>s</i></span> and the number of queries. </p><p>The second line contains <span class="tex-span"><i>s</i></span>, a sequence of "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>" and digits (<span class="tex-font-style-tt">0..9</span>) written from left to right. Note, that the characters of <span class="tex-span"><i>s</i></span> are not separated with spaces. </p><p>The next <span class="tex-span"><i>q</i></span> lines each contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>For each query print <span class="tex-span">10</span> space separated integers: <span class="tex-span"><i>x</i><sub class="lower-index">0</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index">9</sub></span> where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> equals the number of times the interpreter prints <span class="tex-span"><i>i</i></span> while running the corresponding program. Print answers to the queries in the order they are given in input.</p>





```input1
7 4
1&gt;3&gt;22&lt;
1 3
4 7
7 7
1 7

```




```output1
0 1 0 1 0 0 0 0 0 0 
2 2 2 0 0 0 0 0 0 0 
0 0 0 0 0 0 0 0 0 0 
2 3 2 1 0 0 0 0 0 0 

```


