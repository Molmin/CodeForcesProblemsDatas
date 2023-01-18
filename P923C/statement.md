## Description

<div><p>Alice has a very important message <span class="tex-span"><i>M</i></span> consisting of some non-negative integers that she wants to keep secret from Eve. Alice knows that the only theoretically secure cipher is one-time pad. Alice generates a random key <span class="tex-span"><i>K</i></span> of the length equal to the message's length. Alice computes the bitwise xor of each element of the message and the key (<img align="middle" class="tex-formula" src="file://M8y6UaC9.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://ccmn4S60.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>) and stores this encrypted message <span class="tex-span"><i>A</i></span>. Alice is smart. Be like Alice.</p><p>For example, Alice may have wanted to store a message <span class="tex-span"><i>M</i> = (0, 15, 9, 18)</span>. She generated a key <span class="tex-span"><i>K</i> = (16, 7, 6, 3)</span>. The encrypted message is thus <span class="tex-span"><i>A</i> = (16, 8, 15, 17)</span>.</p><p>Alice realised that she cannot store the key with the encrypted message. Alice sent her key <span class="tex-span"><i>K</i></span> to Bob and deleted her own copy. Alice is smart. Really, be like Alice.</p><p>Bob realised that the encrypted message is only secure as long as the key is secret. Bob thus randomly permuted the key before storing it. Bob thinks that this way, even if Eve gets both the encrypted message and the key, she will not be able to read the message. Bob is not smart. Don't be like Bob.</p><p>In the above example, Bob may have, for instance, selected a permutation <span class="tex-span">(3, 4, 1, 2)</span> and stored the permuted key <span class="tex-span"><i>P</i> = (6, 3, 16, 7)</span>.</p><p>One year has passed and Alice wants to decrypt her message. Only now Bob has realised that this is impossible. As he has permuted the key randomly, the message is lost forever. Did we mention that Bob isn't smart?</p><p>Bob wants to salvage at least some information from the message. Since he is not so smart, he asks for your help. You know the encrypted message <span class="tex-span"><i>A</i></span> and the permuted key <span class="tex-span"><i>P</i></span>. What is the lexicographically smallest message that could have resulted in the given encrypted text?</p><p>More precisely, for given <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>P</i></span>, find the lexicographically smallest message <span class="tex-span"><i>O</i></span>, for which there exists a permutation <span class="tex-span">π</span> such that <img align="middle" class="tex-formula" src="file://X7zBbtxD.png" style="max-width: 100.0%;max-height: 100.0%;"> for every <span class="tex-span"><i>i</i></span>.</p><p>Note that the sequence <span class="tex-span"><i>S</i></span> is lexicographically smaller than the sequence <span class="tex-span"><i>T</i></span>, if there is an index <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>S</i><sub class="lower-index"><i>i</i></sub> &lt; <i>T</i><sub class="lower-index"><i>i</i></sub></span> and for all <span class="tex-span"><i>j</i> &lt; <i>i</i></span> the condition <span class="tex-span"><i>S</i><sub class="lower-index"><i>j</i></sub> = <i>T</i><sub class="lower-index"><i>j</i></sub></span> holds. </p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 300000</span>), the length of the message. </p><p>The second line contains <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>A</i><sub class="lower-index">1</sub>, <i>A</i><sub class="lower-index">2</sub>, ..., <i>A</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">0 ≤ <i>A</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) representing the encrypted message.</p><p>The third line contains <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>P</i><sub class="lower-index">1</sub>, <i>P</i><sub class="lower-index">2</sub>, ..., <i>P</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">0 ≤ <i>P</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) representing the permuted encryption key.</p></div><div class="output-specification"><p>Output a single line with <span class="tex-span"><i>N</i></span> integers, the lexicographically smallest possible message <span class="tex-span"><i>O</i></span>. Note that all its elements should be non-negative.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 300000</span>), the length of the message. </p><p>The second line contains <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>A</i><sub class="lower-index">1</sub>, <i>A</i><sub class="lower-index">2</sub>, ..., <i>A</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">0 ≤ <i>A</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) representing the encrypted message.</p><p>The third line contains <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>P</i><sub class="lower-index">1</sub>, <i>P</i><sub class="lower-index">2</sub>, ..., <i>P</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span">0 ≤ <i>P</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) representing the permuted encryption key.</p>

## Output

<p>Output a single line with <span class="tex-span"><i>N</i></span> integers, the lexicographically smallest possible message <span class="tex-span"><i>O</i></span>. Note that all its elements should be non-negative.</p>





```input1
3
8 4 13
17 2 7

```




```input2
5
12 7 87 22 11
18 39 9 12 16

```




```input3
10
331415699 278745619 998190004 423175621 42983144 166555524 843586353 802130100 337889448 685310951
226011312 266003835 342809544 504667531 529814910 684873393 817026985 844010788 993949858 1031395667

```




```output1
10 3 28

```




```output2
0 14 69 6 44

```




```output3
128965467 243912600 4281110 112029883 223689619 76924724 429589 119397893 613490433 362863284

```



## Note

<p>In the first case, the solution is <span class="tex-span">(10, 3, 28)</span>, since <img align="middle" class="tex-formula" src="file://NKjbFRYo.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://k9KWn29l.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://QrXRwXuJ.png" style="max-width: 100.0%;max-height: 100.0%;">. Other possible permutations of key yield messages <span class="tex-span">(25, 6, 10)</span>, <span class="tex-span">(25, 3, 15)</span>, <span class="tex-span">(10, 21, 10)</span>, <span class="tex-span">(15, 21, 15)</span> and <span class="tex-span">(15, 6, 28)</span>, which are all lexicographically larger than the solution.</p>
