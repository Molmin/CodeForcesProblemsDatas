## Description

<div><p>A long time ago, in a galaxy far far away two giant IT-corporations Pineapple and Gogol continue their fierce competition. Crucial moment is just around the corner: Gogol is ready to release it's new tablet Lastus 3000.</p><p>This new device is equipped with specially designed artificial intelligence (AI). Employees of Pineapple did their best to postpone the release of Lastus 3000 as long as possible. Finally, they found out, that the name of the new artificial intelligence is similar to the name of the phone, that Pineapple released 200 years ago. As all rights on its name belong to Pineapple, they stand on changing the name of Gogol's artificial intelligence.</p><p>Pineapple insists, that the name of their phone occurs in the name of AI as a substring. Because the name of technology was already printed on all devices, the Gogol's director decided to replace some characters in AI name with "<span class="tex-font-style-tt">#</span>". As this operation is pretty expensive, you should find the minimum number of characters to replace with "<span class="tex-font-style-tt">#</span>", such that the name of AI doesn't contain the name of the phone as a substring.</p><p>Substring is a continuous subsequence of a string.</p></div><div class="input-specification"><p>The first line of the input contains the name of AI designed by Gogol, its length doesn't exceed <span class="tex-span">100 000</span> characters. Second line contains the name of the phone released by Pineapple 200 years ago, its length doesn't exceed <span class="tex-span">30</span>. Both string are non-empty and consist of only small English letters.</p></div><div class="output-specification"><p>Print the minimum number of characters that must be replaced with "<span class="tex-font-style-tt">#</span>" in order to obtain that the name of the phone doesn't occur in the name of AI as a substring.</p></div>

## Input

<p>The first line of the input contains the name of AI designed by Gogol, its length doesn't exceed <span class="tex-span">100 000</span> characters. Second line contains the name of the phone released by Pineapple 200 years ago, its length doesn't exceed <span class="tex-span">30</span>. Both string are non-empty and consist of only small English letters.</p>

## Output

<p>Print the minimum number of characters that must be replaced with "<span class="tex-font-style-tt">#</span>" in order to obtain that the name of the phone doesn't occur in the name of AI as a substring.</p>





```input1
intellect
tell

```




```input2
google
apple

```




```input3
sirisiri
sir

```




```output1
1
```




```output2
0
```




```output3
2
```



## Note

<p>In the first sample AI's name may be replaced with "<span class="tex-font-style-tt">int#llect</span>".</p><p>In the second sample Gogol can just keep things as they are.</p><p>In the third sample one of the new possible names of AI may be "<span class="tex-font-style-tt">s#ris#ri</span>".</p>
