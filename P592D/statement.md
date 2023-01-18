## Description

<div><p>Ari the monster is not an ordinary monster. She is the hidden identity of Super M, the Byteforces’ superhero. Byteforces is a country that consists of <span class="tex-span"><i>n</i></span> cities, connected by <span class="tex-span"><i>n</i> - 1</span> bidirectional roads. Every road connects exactly two distinct cities, and the whole road system is designed in a way that one is able to go from any city to any other city using only the given roads. There are <span class="tex-span"><i>m</i></span> cities being attacked by humans. So Ari... we meant Super M have to immediately go to each of the cities being attacked to scare those bad humans. Super M can pass from one city to another only using the given roads. Moreover, passing through one road takes her exactly one kron - the time unit used in Byteforces. </p><center> <img class="tex-graphics" src="file://ptlRALZp.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>However, Super M is not on Byteforces now - she is attending a training camp located in a nearby country Codeforces. Fortunately, there is a special device in Codeforces that allows her to instantly teleport from Codeforces to any city of Byteforces. The way back is too long, so for the purpose of this problem teleportation is used exactly once.</p><p>You are to help Super M, by calculating the city in which she should teleport at the beginning in order to end her job in the minimum time (measured in krons). Also, provide her with this time so she can plan her way back to Codeforces.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 123456</span>) - the number of cities in Byteforces, and the number of cities being attacked respectively.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines, describing the road system. Each line contains two city numbers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) - the ends of the road <span class="tex-span"><i>i</i></span>.</p><p>The last line contains <span class="tex-span"><i>m</i></span> distinct integers - numbers of cities being attacked. These numbers are given in no particular order.</p></div><div class="output-specification"><p>First print the number of the city Super M should teleport to. If there are many possible optimal answers, print the one with the lowest city number.</p><p>Then print the minimum possible time needed to scare all humans in cities being attacked, measured in Krons.</p><p>Note that the correct answer is always unique.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 123456</span>) - the number of cities in Byteforces, and the number of cities being attacked respectively.</p><p>Then follow <span class="tex-span"><i>n</i> - 1</span> lines, describing the road system. Each line contains two city numbers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) - the ends of the road <span class="tex-span"><i>i</i></span>.</p><p>The last line contains <span class="tex-span"><i>m</i></span> distinct integers - numbers of cities being attacked. These numbers are given in no particular order.</p>

## Output

<p>First print the number of the city Super M should teleport to. If there are many possible optimal answers, print the one with the lowest city number.</p><p>Then print the minimum possible time needed to scare all humans in cities being attacked, measured in Krons.</p><p>Note that the correct answer is always unique.</p>





```input1
7 2
1 2
1 3
1 4
3 5
3 6
3 7
2 7

```




```input2
6 4
1 2
2 3
2 4
4 5
4 6
2 4 5 6

```




```output1
2
3

```




```output2
2
4

```



## Note

<p>In the first sample, there are two possibilities to finish the Super M's job in <span class="tex-span">3</span> krons. They are:</p><p><img align="middle" class="tex-formula" src="file://ehEv4dQ3.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://2IzBnbdR.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>However, you should choose the first one as it starts in the city with the lower number.</p>
