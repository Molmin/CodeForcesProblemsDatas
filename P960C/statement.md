## Description

<div><p>Pikachu had an array with him. He wrote down all the non-empty subsequences of the array on paper. Note that an array of size <span class="tex-span"><i>n</i></span> has <span class="tex-span">2<sup class="upper-index"><i>n</i></sup> - 1</span> non-empty subsequences in it. </p><p>Pikachu being mischievous as he always is, removed all the subsequences in which <span class="tex-font-style-tt">Maximum_element_of_the_subsequence</span> <span class="tex-span"> - </span> <span class="tex-font-style-tt">Minimum_element_of_subsequence</span> <span class="tex-span"> ≥ <i>d</i></span></p><p>Pikachu was finally left with <span class="tex-span"><i>X</i></span> subsequences. </p><p>However, he lost the initial array he had, and now is in serious trouble. He still remembers the numbers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>d</i></span>. He now wants you to construct any such array which will satisfy the above conditions. All the numbers in the final array should be positive integers less than <span class="tex-span">10<sup class="upper-index">18</sup></span>. </p><p>Note the number of elements in the output array should not be more than <span class="tex-span">10<sup class="upper-index">4</sup></span>. If no answer is possible, print <span class="tex-span"> - 1</span>.</p></div><div class="input-specification"><p>The only line of input consists of two space separated integers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>X</i>, <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output should consist of two lines.</p><p>First line should contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>)— the number of integers in the final array.</p><p>Second line should consist of <span class="tex-span"><i>n</i></span> space separated integers — <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">18</sup></span>).</p><p>If there is no answer, print a single integer <span class="tex-font-style-tt">-1</span>. If there are multiple answers, print any of them.</p></div>

## Input

<p>The only line of input consists of two space separated integers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>X</i>, <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output should consist of two lines.</p><p>First line should contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>)— the number of integers in the final array.</p><p>Second line should consist of <span class="tex-span"><i>n</i></span> space separated integers — <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">18</sup></span>).</p><p>If there is no answer, print a single integer <span class="tex-font-style-tt">-1</span>. If there are multiple answers, print any of them.</p>





```input1
10 5

```




```input2
4 2

```




```output1
6
5 50 7 15 6 100
```




```output2
4
10 100 1000 10000
```



## Note

<p>In the output of the first example case, the remaining subsequences after removing those with <span class="tex-font-style-tt">Maximum_element_of_the_subsequence</span> <span class="tex-span"> - </span> <span class="tex-font-style-tt">Minimum_element_of_subsequence</span> <span class="tex-span"> ≥ 5</span> are <span class="tex-span">[5], [5, 7], [5, 6], [5, 7, 6], [50], [7], [7, 6], [15], [6], [100]</span>. There are <span class="tex-span">10</span> of them. Hence, the array <span class="tex-span">[5, 50, 7, 15, 6, 100]</span> is valid.</p><p>Similarly, in the output of the second example case, the remaining sub-sequences after removing those with <span class="tex-font-style-tt">Maximum_element_of_the_subsequence</span> <span class="tex-span"> - </span> <span class="tex-font-style-tt">Minimum_element_of_subsequence</span> <span class="tex-span"> ≥ 2</span> are <span class="tex-span">[10], [100], [1000], [10000]</span>. There are <span class="tex-span">4</span> of them. Hence, the array <span class="tex-span">[10, 100, 1000, 10000]</span> is valid.</p>
