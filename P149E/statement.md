## Description

<div><p>During the study of the Martians Petya clearly understood that the Martians are absolutely lazy. They like to sleep and don't like to wake up. </p><p>Imagine a Martian who has exactly <span class="tex-span"><i>n</i></span> eyes located in a row and numbered from the left to the right from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. When a Martian sleeps, he puts a patch on each eye (so that the Martian morning doesn't wake him up). The inner side of each patch has an uppercase Latin letter. So, when a Martian wakes up and opens all his eyes he sees a string <span class="tex-span"><i>s</i></span> consisting of uppercase Latin letters. The string's length is <span class="tex-span"><i>n</i></span>. </p><p>"Ding dong!" — the alarm goes off. A Martian has already woken up but he hasn't opened any of his eyes. He feels that today is going to be a hard day, so he wants to open his eyes and see something good. The Martian considers only <span class="tex-span"><i>m</i></span> Martian words beautiful. Besides, it is hard for him to open all eyes at once so early in the morning. So he opens two non-overlapping segments of consecutive eyes. <span class="tex-font-style-bf">More formally, the Martian chooses four numbers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> &lt; <i>c</i> ≤ <i>d</i> ≤ <i>n</i></span>) and opens all eyes with numbers <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>a</i> ≤ <i>i</i> ≤ <i>b</i></span> or <span class="tex-span"><i>c</i> ≤ <i>i</i> ≤ <i>d</i></span>.</span> After the Martian opens the eyes he needs, he reads all the visible characters from the left to the right and thus, he sees some word.</p><p>Let's consider all different words the Martian can see in the morning. Your task is to find out how many beautiful words are among them.</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span> consisting of uppercase Latin letters. The strings' length is <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>) — the number of beautiful words. Next <span class="tex-span"><i>m</i></span> lines contain the beautiful words <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, consisting of uppercase Latin letters. Their length is from <span class="tex-span">1</span> to <span class="tex-span">1000</span>. All beautiful strings are pairwise different.</p></div><div class="output-specification"><p>Print the single integer — the number of different beautiful strings the Martian can see this morning.</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span> consisting of uppercase Latin letters. The strings' length is <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>) — the number of beautiful words. Next <span class="tex-span"><i>m</i></span> lines contain the beautiful words <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, consisting of uppercase Latin letters. Their length is from <span class="tex-span">1</span> to <span class="tex-span">1000</span>. All beautiful strings are pairwise different.</p>

## Output

<p>Print the single integer — the number of different beautiful strings the Martian can see this morning.</p>





```input1
ABCBABA
2
BAAB
ABBA

```




```output1
1

```



## Note

<p>Let's consider the sample test. There the Martian can get only the second beautiful string if he opens segments of eyes <span class="tex-span"><i>a</i> = 1, <i>b</i> = 2</span> and <span class="tex-span"><i>c</i> = 4, <i>d</i> = 5</span> or of he opens segments of eyes <span class="tex-span"><i>a</i> = 1, <i>b</i> = 2</span> and <span class="tex-span"><i>c</i> = 6, <i>d</i> = 7</span>. </p>
