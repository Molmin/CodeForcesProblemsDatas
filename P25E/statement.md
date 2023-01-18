## Description

<div><p>Sometimes it is hard to prepare tests for programming problems. Now Bob is preparing tests to new problem about strings — input data to his problem is one string. Bob has 3 wrong solutions to this problem. The first gives the wrong answer if the input data contains the substring <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, the second enters an infinite loop if the input data contains the substring <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, and the third requires too much memory if the input data contains the substring <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span>. Bob wants these solutions to fail single test. What is the minimal length of test, which couldn't be passed by all three Bob's solutions?</p></div><div class="input-specification"><p>There are exactly 3 lines in the input data. The <span class="tex-span"><i>i</i></span>-th line contains string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. All the strings are non-empty, consists of lowercase Latin letters, the length of each string doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Output one number — what is minimal length of the string, containing <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span> as substrings.</p></div>

## Input

<p>There are exactly 3 lines in the input data. The <span class="tex-span"><i>i</i></span>-th line contains string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. All the strings are non-empty, consists of lowercase Latin letters, the length of each string doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Output one number — what is minimal length of the string, containing <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span> as substrings.</p>





```input1
ab
bc
cd

```




```input2
abacaba
abaaba
x

```




```output1
4

```




```output2
11

```


