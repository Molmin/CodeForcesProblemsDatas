## Description

<div><p>Every year a race takes place on the motorway between cities A and B. This year Vanya decided to take part in the race and drive his own car that has been around and bears its own noble name — The Huff-puffer.</p><p>So, Vasya leaves city A on the Huff-puffer, besides, at the very beginning he fills the petrol tank with <span class="tex-span">α</span> liters of petrol (<span class="tex-span">α ≥ 10</span> is Vanya's favorite number, it is not necessarily integer). Petrol stations are located on the motorway at an interval of <span class="tex-span">100</span> kilometers, i.e. the first station is located <span class="tex-span">100</span> kilometers away from the city A, the second one is <span class="tex-span">200</span> kilometers away from the city A, the third one is <span class="tex-span">300</span> kilometers away from the city A and so on. The Huff-puffer spends <span class="tex-span">10</span> liters of petrol every <span class="tex-span">100</span> kilometers. </p><p>Vanya checks the petrol tank every time he passes by a petrol station. If the petrol left in the tank is not enough to get to the next station, Vanya fills the tank with <span class="tex-span">α</span> liters of petrol. Otherwise, he doesn't stop at the station and drives on. </p><p>For example, if <span class="tex-span">α = 43.21</span>, then the car will be fuelled up for the first time at the station number <span class="tex-span">4</span>, when there'll be <span class="tex-span">3.21</span> petrol liters left. After the fuelling up the car will have <span class="tex-span">46.42</span> liters. Then Vanya stops at the station number <span class="tex-span">8</span> and ends up with <span class="tex-span">6.42 + 43.21 = 49.63</span> liters. The next stop is at the station number <span class="tex-span">12</span>, <span class="tex-span">9.63 + 43.21 = 52.84</span>. The next stop is at the station number <span class="tex-span">17</span> and so on. </p><p>You won't believe this but the Huff-puffer has been leading in the race! Perhaps it is due to unexpected snow. Perhaps it is due to video cameras that have been installed along the motorway which register speed limit breaking. Perhaps it is due to the fact that Vanya threatened to junk the Huff-puffer unless the car wins. Whatever the reason is, the Huff-puffer is leading, and jealous people together with other contestants wrack their brains trying to think of a way to stop that outrage.</p><p>One way to do this is to mine the next petrol station where Vanya will stop. Your task is to calculate at which station this will happen and warn Vanya. You don't know the <span class="tex-span">α</span> number, however, you are given the succession of the numbers of the stations where Vanya has stopped. Find the number of the station where the next stop will be.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) which represents the number of petrol stations where Vanya has stopped. The next line has <span class="tex-span"><i>n</i></span> space-separated integers which represent the numbers of the stations. The numbers are positive and do not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>, they are given in the increasing order. No two numbers in the succession match. It is guaranteed that there exists at least one number <span class="tex-span">α ≥ 10</span>, to which such a succession of stops corresponds.</p></div><div class="output-specification"><p>Print in the first line "unique" (without quotes) if the answer can be determined uniquely. In the second line print the number of the station where the next stop will take place. If the answer is not unique, print in the first line "not unique".</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) which represents the number of petrol stations where Vanya has stopped. The next line has <span class="tex-span"><i>n</i></span> space-separated integers which represent the numbers of the stations. The numbers are positive and do not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>, they are given in the increasing order. No two numbers in the succession match. It is guaranteed that there exists at least one number <span class="tex-span">α ≥ 10</span>, to which such a succession of stops corresponds.</p>

## Output

<p>Print in the first line "unique" (without quotes) if the answer can be determined uniquely. In the second line print the number of the station where the next stop will take place. If the answer is not unique, print in the first line "not unique".</p>





```input1
3
1 2 4

```




```input2
2
1 2

```




```output1
unique
5

```




```output2
not unique

```



## Note

<p>In the second example the answer is not unique. For example, if <span class="tex-span">α = 10</span>, we'll have such a sequence as <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, and if <span class="tex-span">α = 14</span>, the sequence will be <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">4</span>.</p>
