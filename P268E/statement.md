## Description

<div><p>Manao's friends often send him new songs. He never listens to them right away. Instead, he compiles them into a playlist. When he feels that his mind is open to new music, he opens the playlist and starts to listen to the songs.</p><p>Of course, there are some songs that Manao doesn't particuarly enjoy. To get more pleasure from the received songs, he invented the following procedure of listening to the playlist:</p><ul> <li> If after listening to some song Manao realizes that he liked it, then he remembers it and starts to listen to the next unlistened song. </li><li> If after listening to some song Manao realizes that he did not like it, he listens to all the songs he liked up to this point and then begins to listen to the next unlistened song. </li></ul><p>For example, if Manao has four songs in the playlist, A, B, C, D (in the corresponding order) and he is going to like songs A and C in the end, then the order of listening is the following:</p><ol> <li> Manao listens to A, he likes it, he remembers it. </li><li> Manao listens to B, he does not like it, so he listens to A, again. </li><li> Manao listens to C, he likes the song and he remembers it, too. </li><li> Manao listens to D, but does not enjoy it and re-listens to songs A and C. </li></ol><p>That is, in the end Manao listens to song A three times, to song C twice and songs B and D once. Note that if Manao once liked a song, he will never dislike it on a subsequent listening.</p><p>Manao has received <span class="tex-span"><i>n</i></span> songs: the <span class="tex-span"><i>i</i></span>-th of them is <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> seconds long and Manao may like it with a probability of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> percents. The songs could get on Manao's playlist in any order, so Manao wants to know the maximum expected value of the number of seconds after which the listening process will be over, for all possible permutations of the songs in the playlist.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50000</span>). The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains two integers, separated by a single space — <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">15 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the length of the <span class="tex-span"><i>i</i></span>-th song in seconds and the probability that Manao will like the song, in percents.</p></div><div class="output-specification"><p>In a single line print a single real number — the maximum expected listening time over all permutations of songs. The answer will be considered valid if the absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50000</span>). The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains two integers, separated by a single space — <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">15 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the length of the <span class="tex-span"><i>i</i></span>-th song in seconds and the probability that Manao will like the song, in percents.</p>

## Output

<p>In a single line print a single real number — the maximum expected listening time over all permutations of songs. The answer will be considered valid if the absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
3
150 20
150 50
100 50

```




```input2
4
300 0
300 50
240 50
360 80

```




```output1
537.500000000

```




```output2
2121.000000000

```



## Note

<p>Consider the first test case. If Manao listens to the songs in the order in which they were originally compiled, the mathematical expectation will be equal to 467.5 seconds. The maximum expected value is obtained by putting the first song at the end of the playlist.</p><p>Consider the second test case. The song which is 360 seconds long should be listened to first. The song 300 seconds long which Manao will dislike for sure should be put in the end.</p>
