## Description

<div><p>Peter likes to travel by train. He likes it so much that on the train he falls asleep. </p><p>Once in summer Peter was going by train from city A to city B, and as usual, was sleeping. Then he woke up, started to look through the window and noticed that every railway station has a flag of a particular colour.</p><p>The boy started to memorize the order of the flags' colours that he had seen. But soon he fell asleep again. Unfortunately, he didn't sleep long, he woke up and went on memorizing the colours. Then he fell asleep again, and that time he slept till the end of the journey.</p><p>At the station he told his parents about what he was doing, and wrote two sequences of the colours that he had seen before and after his sleep, respectively.</p><p>Peter's parents know that their son likes to fantasize. They give you the list of the flags' colours at the stations that the train passes sequentially on the way from A to B, and ask you to find out if Peter could see those sequences on the way from A to B, or from B to A. Remember, please, that Peter had two periods of wakefulness.</p><p>Peter's parents put lowercase Latin letters for colours. The same letter stands for the same colour, different letters — for different colours.</p></div><div class="input-specification"><p>The input data contains three lines. The first line contains a non-empty string, whose length does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>, the string consists of lowercase Latin letters — the flags' colours at the stations on the way from A to B. On the way from B to A the train passes the same stations, but in reverse order. </p><p>The second line contains the sequence, written by Peter during the first period of wakefulness. The third line contains the sequence, written during the second period of wakefulness. Both sequences are non-empty, consist of lowercase Latin letters, and the length of each does not exceed 100 letters. Each of the sequences is written in chronological order. </p></div><div class="output-specification"><p>Output one of the four words without inverted commas: </p><ul> <li> «<span class="tex-font-style-tt">forward</span>» — if Peter could see such sequences only on the way from A to B; </li><li> «<span class="tex-font-style-tt">backward</span>» — if Peter could see such sequences on the way from B to A; </li><li> «<span class="tex-font-style-tt">both</span>» — if Peter could see such sequences both on the way from A to B, and on the way from B to A; </li><li> «<span class="tex-font-style-tt">fantasy</span>» — if Peter could not see such sequences. </li></ul></div>

## Input

<p>The input data contains three lines. The first line contains a non-empty string, whose length does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>, the string consists of lowercase Latin letters — the flags' colours at the stations on the way from A to B. On the way from B to A the train passes the same stations, but in reverse order. </p><p>The second line contains the sequence, written by Peter during the first period of wakefulness. The third line contains the sequence, written during the second period of wakefulness. Both sequences are non-empty, consist of lowercase Latin letters, and the length of each does not exceed 100 letters. Each of the sequences is written in chronological order. </p>

## Output

<p>Output one of the four words without inverted commas: </p><ul> <li> «<span class="tex-font-style-tt">forward</span>» — if Peter could see such sequences only on the way from A to B; </li><li> «<span class="tex-font-style-tt">backward</span>» — if Peter could see such sequences on the way from B to A; </li><li> «<span class="tex-font-style-tt">both</span>» — if Peter could see such sequences both on the way from A to B, and on the way from B to A; </li><li> «<span class="tex-font-style-tt">fantasy</span>» — if Peter could not see such sequences. </li></ul>





```input1
atob
a
b

```




```input2
aaacaaa
aca
aa

```




```output1
forward

```




```output2
both

```



## Note

<p>It is assumed that the train moves all the time, so one flag cannot be seen twice. There are no flags at stations A and B.</p>
