## Description

<div><p>You're playing a game called Osu! Here's a simplified version of it. There are <span class="tex-span"><i>n</i></span> clicks in a game. For each click there are two outcomes: correct or bad. Let us denote correct as "<span class="tex-font-style-tt">O</span>", bad as "<span class="tex-font-style-tt">X</span>", then the whole play can be encoded as a sequence of <span class="tex-span"><i>n</i></span> characters "<span class="tex-font-style-tt">O</span>" and "<span class="tex-font-style-tt">X</span>".</p><p>Using the play sequence you can calculate the score for the play as follows: for every maximal consecutive "<span class="tex-font-style-tt">O</span>"s block, add the square of its length (the number of characters "<span class="tex-font-style-tt">O</span>") to the score. For example, if your play can be encoded as "<span class="tex-font-style-tt">OOXOOOXXOO</span>", then there's three maximal consecutive "<span class="tex-font-style-tt">O</span>"s block "<span class="tex-font-style-tt">OO</span>", "<span class="tex-font-style-tt">OOO</span>", "<span class="tex-font-style-tt">OO</span>", so your score will be <span class="tex-span">2<sup class="upper-index">2</sup> + 3<sup class="upper-index">2</sup> + 2<sup class="upper-index">2</sup> = 17</span>. If there are no correct clicks in a play then the score for the play equals to <span class="tex-span">0</span>.</p><p>You know that the probability to click the <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> click correctly is <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. In other words, the <span class="tex-span"><i>i</i></span>-th character in the play sequence has <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> probability to be "<span class="tex-font-style-tt">O</span>", <span class="tex-span">1 - <i>p</i><sub class="lower-index"><i>i</i></sub></span> to be "<span class="tex-font-style-tt">X</span>". You task is to calculate the expected score for your play.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of clicks. The second line contains <span class="tex-span"><i>n</i></span> space-separated real numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span>.</p><p>There will be at most six digits after the decimal point in the given <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print a single real number — the expected score for your play. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of clicks. The second line contains <span class="tex-span"><i>n</i></span> space-separated real numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span>.</p><p>There will be at most six digits after the decimal point in the given <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print a single real number — the expected score for your play. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3
0.5 0.5 0.5

```




```input2
4
0.7 0.2 0.1 0.9

```




```input3
5
1 1 1 1 1

```




```output1
2.750000000000000

```




```output2
2.489200000000000

```




```output3
25.000000000000000

```



## Note

<p>For the first example. There are 8 possible outcomes. Each has a probability of 0.125.</p><ul> <li> "<span class="tex-font-style-tt">OOO</span>" <span class="tex-span"> → </span> <span class="tex-span">3<sup class="upper-index">2</sup> = 9</span>; </li><li> "<span class="tex-font-style-tt">OOX</span>" <span class="tex-span"> → </span> <span class="tex-span">2<sup class="upper-index">2</sup> = 4</span>; </li><li> "<span class="tex-font-style-tt">OXO</span>" <span class="tex-span"> → </span> <span class="tex-span">1<sup class="upper-index">2</sup> + 1<sup class="upper-index">2</sup> = 2</span>; </li><li> "<span class="tex-font-style-tt">OXX</span>" <span class="tex-span"> → </span> <span class="tex-span">1<sup class="upper-index">2</sup> = 1</span>; </li><li> "<span class="tex-font-style-tt">XOO</span>" <span class="tex-span"> → </span> <span class="tex-span">2<sup class="upper-index">2</sup> = 4</span>; </li><li> "<span class="tex-font-style-tt">XOX</span>" <span class="tex-span"> → </span> <span class="tex-span">1<sup class="upper-index">2</sup> = 1</span>; </li><li> "<span class="tex-font-style-tt">XXO</span>" <span class="tex-span"> → </span> <span class="tex-span">1<sup class="upper-index">2</sup> = 1</span>; </li><li> "<span class="tex-font-style-tt">XXX</span>" <span class="tex-span"> → </span> <span class="tex-span">0</span>. </li></ul><p>So the expected score is <img align="middle" class="tex-formula" src="file://Xv93Mw2s.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
