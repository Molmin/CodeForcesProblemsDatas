## Description

<div><p>Mahmoud wants to send a message to his friend Ehab. Their language consists of <span class="tex-span"><i>n</i></span> words numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Some words have the same meaning so there are <span class="tex-span"><i>k</i></span> groups of words such that all the words in some group have the same meaning.</p><p>Mahmoud knows that the <span class="tex-span"><i>i</i></span>-th word can be sent with cost <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. For each word in his message, Mahmoud can either replace it with another word of the same meaning or leave it as it is. Can you help Mahmoud determine the minimum cost of sending the message?</p><p>The cost of sending the message is the sum of the costs of sending every word in it.</p></div><div class="input-specification"><p>The first line of input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>&nbsp;— the number of words in their language, the number of groups of words, and the number of words in Mahmoud's message respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> strings consisting of lowercase English letters of length not exceeding 20 which represent the words. It's guaranteed that the words are <span class="tex-font-style-bf">distinct</span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the cost of sending the <span class="tex-span"><i>i</i></span>-th word.</p><p>The next <span class="tex-span"><i>k</i></span> lines describe the groups of words of same meaning. The next <span class="tex-span"><i>k</i></span> lines each start with an integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>)</span> which means that there are <span class="tex-span"><i>x</i></span> words in this group, followed by <span class="tex-span"><i>x</i></span> integers which represent the indices of words in this group. It's guaranteed that each word appears in exactly one group.</p><p>The next line contains <span class="tex-span"><i>m</i></span> space-separated words which represent Mahmoud's message. Each of these words appears in the list of language's words.</p></div><div class="output-specification"><p>The only line should contain the minimum cost to send the message after replacing some words (maybe none) with some words of the same meaning.</p></div>

## Input

<p>The first line of input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>&nbsp;— the number of words in their language, the number of groups of words, and the number of words in Mahmoud's message respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> strings consisting of lowercase English letters of length not exceeding 20 which represent the words. It's guaranteed that the words are <span class="tex-font-style-bf">distinct</span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the cost of sending the <span class="tex-span"><i>i</i></span>-th word.</p><p>The next <span class="tex-span"><i>k</i></span> lines describe the groups of words of same meaning. The next <span class="tex-span"><i>k</i></span> lines each start with an integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>)</span> which means that there are <span class="tex-span"><i>x</i></span> words in this group, followed by <span class="tex-span"><i>x</i></span> integers which represent the indices of words in this group. It's guaranteed that each word appears in exactly one group.</p><p>The next line contains <span class="tex-span"><i>m</i></span> space-separated words which represent Mahmoud's message. Each of these words appears in the list of language's words.</p>

## Output

<p>The only line should contain the minimum cost to send the message after replacing some words (maybe none) with some words of the same meaning.</p>





```input1
5 4 4
i loser am the second
100 1 1 5 10
1 1
1 3
2 2 5
1 4
i am the second

```




```input2
5 4 4
i loser am the second
100 20 1 5 10
1 1
1 3
2 2 5
1 4
i am the second

```




```output1
107
```




```output2
116
```



## Note

<p>In the first sample, Mahmoud should replace the word "<span class="tex-font-style-tt">second</span>" with the word "<span class="tex-font-style-tt">loser</span>" because it has less cost so the cost will be 100+1+5+1=107.</p><p>In the second sample, Mahmoud shouldn't do any replacement so the cost will be 100+1+5+10=116.</p>
