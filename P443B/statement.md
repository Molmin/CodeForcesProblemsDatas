## Description

<div><p>Kolya got string <span class="tex-span"><i>s</i></span> for his birthday, the string consists of small English letters. He immediately added <span class="tex-span"><i>k</i></span> more characters to the right of the string.</p><p>Then Borya came and said that the new string contained a <span class="tex-font-style-it">tandem repeat</span> of length <span class="tex-span"><i>l</i></span> as a substring. How large could <span class="tex-span"><i>l</i></span> be?</p><p>See notes for definition of a <span class="tex-font-style-it">tandem repeat</span>.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 200</span>). This string contains only small English letters. The second line contains number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 200</span>) — the number of the added characters.</p></div><div class="output-specification"><p>Print a single number — the maximum length of the tandem repeat that could have occurred in the new string.</p></div>

## Input

<p>The first line contains <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 200</span>). This string contains only small English letters. The second line contains number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 200</span>) — the number of the added characters.</p>

## Output

<p>Print a single number — the maximum length of the tandem repeat that could have occurred in the new string.</p>





```input1
aaba
2

```




```input2
aaabbbb
2

```




```input3
abracadabra
10

```




```output1
6

```




```output2
6

```




```output3
20

```



## Note

<p>A tandem repeat of length <span class="tex-span">2<i>n</i></span> is string <span class="tex-span"><i>s</i></span>, where for any position <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) the following condition fulfills: <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>i</i> + <i>n</i></sub></span>.</p><p>In the first sample Kolya could obtain a string <span class="tex-font-style-tt">aabaab</span>, in the second — <span class="tex-font-style-tt">aaabbbbbb</span>, in the third — <span class="tex-font-style-bf">abracadabrabracadabra</span>.</p>
