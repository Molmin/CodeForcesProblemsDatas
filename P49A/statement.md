## Description

<div><p>Vasya plays the sleuth with his friends. The rules of the game are as follows: those who play for the first time, that is Vasya is the sleuth, he should investigate a "crime" and find out what is happening. He can ask any questions whatsoever that can be answered with "Yes" or "No". All the rest agree beforehand to answer the questions like that: if the question’s last letter is a vowel, they answer "Yes" and if the last letter is a consonant, they answer "No". Of course, the sleuth knows nothing about it and his task is to understand that.</p><p>Unfortunately, Vasya is not very smart. After 5 hours of endless stupid questions everybody except Vasya got bored. That’s why Vasya’s friends ask you to write a program that would give answers instead of them.</p><p>The English alphabet vowels are: A, E, I, O, U, Y</p><p>The English alphabet consonants are: B, C, D, F, G, H, J, K, L, M, N, P, Q, R, S, T, V, W, X, Z</p></div><div class="input-specification"><p>The single line contains a question represented by a non-empty line consisting of large and small Latin letters, spaces and a question mark. The line length does not exceed 100. It is guaranteed that the question mark occurs exactly once in the line — as the last symbol and that the line contains at least one letter.</p></div><div class="output-specification"><p>Print answer for the question in a single line: <span class="tex-font-style-tt">YES</span> if the answer is "Yes", <span class="tex-font-style-tt">NO</span> if the answer is "No".</p><p>Remember that in the reply to the question the last <span class="tex-font-style-bf">letter</span>, not the last character counts. I. e. the spaces and the question mark do not count as letters.</p></div>

## Input

<p>The single line contains a question represented by a non-empty line consisting of large and small Latin letters, spaces and a question mark. The line length does not exceed 100. It is guaranteed that the question mark occurs exactly once in the line — as the last symbol and that the line contains at least one letter.</p>

## Output

<p>Print answer for the question in a single line: <span class="tex-font-style-tt">YES</span> if the answer is "Yes", <span class="tex-font-style-tt">NO</span> if the answer is "No".</p><p>Remember that in the reply to the question the last <span class="tex-font-style-bf">letter</span>, not the last character counts. I. e. the spaces and the question mark do not count as letters.</p>





```input1
Is it a melon?

```




```input2
Is it an apple?

```




```input3
Is     it a banana ?

```




```input4
Is   it an apple  and a  banana   simultaneouSLY?

```




```output1
NO

```




```output2
YES

```




```output3
YES

```




```output4
YES

```


