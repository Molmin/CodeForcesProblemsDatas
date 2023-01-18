## Description

<div><p>It turns out that you are a great fan of rock band AC/PE. Peter learned that and started the following game: he plays the first song of the list of <span class="tex-span"><i>n</i></span> songs of the group, and you have to find out the name of the song. After you tell the song name, Peter immediately plays the following song in order, and so on.</p><p>The <span class="tex-span"><i>i</i></span>-th song of AC/PE has its recognizability <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. This means that if the song has not yet been recognized by you, you listen to it for exactly one more second and with probability of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> percent you recognize it and tell it's name. Otherwise you continue listening it. Note that you can only try to guess it only when it is integer number of seconds after the moment the song starts playing.</p><p>In all AC/PE songs the first words of chorus are the same as the title, so when you've heard the first <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> seconds of <span class="tex-span"><i>i</i></span>-th song and its chorus starts, you immediately guess its name for sure.</p><p>For example, in the song Highway To Red the chorus sounds pretty late, but the song has high recognizability. In the song Back In Blue, on the other hand, the words from the title sound close to the beginning of the song, but it's hard to name it before hearing those words. You can name both of these songs during a few more first seconds.</p><p>Determine the expected number songs of you will recognize if the game lasts for exactly <span class="tex-span"><i>T</i></span> seconds (i. e. you can make the last guess on the second <span class="tex-span"><i>T</i></span>, after that the game stops).</p><p><span class="tex-font-style-bf">If all songs are recognized faster than in <span class="tex-span"><i>T</i></span> seconds, the game stops after the last song is recognized.</span></p></div><div class="input-specification"><p>The first line of the input contains numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>T</i> ≤ 5000</span>), separated by a space. Next <span class="tex-span"><i>n</i></span> lines contain pairs of numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>T</i></span>). The songs are given in the same order as in Petya's list.</p></div><div class="output-specification"><p>Output a single number — the expected number of the number of songs you will recognize in <span class="tex-span"><i>T</i></span> seconds. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of the input contains numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>T</i> ≤ 5000</span>), separated by a space. Next <span class="tex-span"><i>n</i></span> lines contain pairs of numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>T</i></span>). The songs are given in the same order as in Petya's list.</p>

## Output

<p>Output a single number — the expected number of the number of songs you will recognize in <span class="tex-span"><i>T</i></span> seconds. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 2
50 2
10 1

```




```input2
2 2
0 2
100 2

```




```input3
3 3
50 3
50 2
25 2

```




```input4
2 2
0 2
0 2

```




```output1
1.500000000

```




```output2
1.000000000

```




```output3
1.687500000

```




```output4
1.000000000

```


