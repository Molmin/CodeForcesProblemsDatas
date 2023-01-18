## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers very much. Everybody knows that lucky numbers are positive integers whose decimal record contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya has sequence <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> integers.</p><p>The subsequence of the sequence <span class="tex-span"><i>a</i></span> is such subsequence that can be obtained from <span class="tex-span"><i>a</i></span> by removing zero or more of its elements.</p><p>Two sequences are considered different if index sets of numbers included in them are different. That is, the values ​of the elements ​do not matter in the comparison of subsequences. In particular, any sequence of length <span class="tex-span"><i>n</i></span> has exactly <span class="tex-span">2<sup class="upper-index"><i>n</i></sup></span> different subsequences (including an empty subsequence).</p><p>A subsequence is considered lucky if it has a length exactly <span class="tex-span"><i>k</i></span> and does not contain two identical lucky numbers (unlucky numbers can be repeated any number of times).</p><p>Help Petya find the number of different lucky subsequences of the sequence <span class="tex-span"><i>a</i></span>. As Petya's parents don't let him play with large numbers, you should print the result modulo prime number <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the sequence <span class="tex-span"><i>a</i></span>. </p></div><div class="output-specification"><p>On the single line print the single number — the answer to the problem modulo prime number <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the sequence <span class="tex-span"><i>a</i></span>. </p>

## Output

<p>On the single line print the single number — the answer to the problem modulo prime number <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
3 2
10 10 10

```




```input2
4 2
4 4 7 7

```




```output1
3

```




```output2
4

```



## Note

<p>In the first sample all <span class="tex-span">3</span> subsequences of the needed length are considered lucky.</p><p>In the second sample there are <span class="tex-span">4</span> lucky subsequences. For them the sets of indexes equal (the indexation starts from <span class="tex-span">1</span>): <span class="tex-span">{1, 3}</span>, <span class="tex-span">{1, 4}</span>, <span class="tex-span">{2, 3}</span> and <span class="tex-span">{2, 4}</span>.</p>
