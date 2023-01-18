## Description

<div><p>Polycarpus takes part in the "Field of Wonders" TV show. The participants of the show have to guess a hidden word as fast as possible. Initially all the letters of the word are hidden.</p><p>The game consists of several turns. At each turn the participant tells a letter and the TV show host responds if there is such letter in the word or not. If there is such letter then the host reveals <span class="tex-font-style-bf">all</span> such letters. For example, if the hidden word is "<span class="tex-font-style-tt">abacaba</span>" and the player tells the letter "<span class="tex-font-style-tt">a</span>", the host will reveal letters at all positions, occupied by "<span class="tex-font-style-tt">a</span>": <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">5</span> and <span class="tex-span">7</span> (positions are numbered from left to right starting from 1).</p><p>Polycarpus knows <span class="tex-span"><i>m</i></span> words of exactly the same length as the hidden word. The hidden word is also known to him and appears as one of these <span class="tex-span"><i>m</i></span> words.</p><p>At current moment a number of turns have already been made and some letters (possibly zero) of the hidden word are already revealed. Previously Polycarp has told exactly the letters which are currently revealed.</p><p>It is Polycarpus' turn. He wants to tell a letter in such a way, that the TV show host will assuredly reveal at least one more letter. Polycarpus cannot tell the letters, which are already revealed.</p><p>Your task is to help Polycarpus and find out the number of letters he can tell so that the show host will assuredly reveal at least one of the remaining letters.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the length of the hidden word.</p><p>The following line describes already revealed letters. It contains the string of length <span class="tex-span"><i>n</i></span>, which consists of lowercase Latin letters and symbols "<span class="tex-font-style-tt">*</span>". If there is a letter at some position, then this letter was already revealed. If the position contains symbol "<span class="tex-font-style-tt">*</span>", then the letter at this position has not been revealed yet. It is guaranteed, that at least one letter is still closed.</p><p>The third line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>) — the number of words of length <span class="tex-span"><i>n</i></span>, which Polycarpus knows. The following <span class="tex-span"><i>m</i></span> lines contain the words themselves — <span class="tex-span"><i>n</i></span>-letter strings of lowercase Latin letters. All words are distinct.</p><p>It is guaranteed that the hidden word appears as one of the given <span class="tex-span"><i>m</i></span> words. Before the current move Polycarp has told exactly the letters which are currently revealed.</p></div><div class="output-specification"><p>Output the single integer — the number of letters Polycarpus can tell so that the TV show host definitely reveals at least one more letter. It is possible that this number is zero.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the length of the hidden word.</p><p>The following line describes already revealed letters. It contains the string of length <span class="tex-span"><i>n</i></span>, which consists of lowercase Latin letters and symbols "<span class="tex-font-style-tt">*</span>". If there is a letter at some position, then this letter was already revealed. If the position contains symbol "<span class="tex-font-style-tt">*</span>", then the letter at this position has not been revealed yet. It is guaranteed, that at least one letter is still closed.</p><p>The third line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>) — the number of words of length <span class="tex-span"><i>n</i></span>, which Polycarpus knows. The following <span class="tex-span"><i>m</i></span> lines contain the words themselves — <span class="tex-span"><i>n</i></span>-letter strings of lowercase Latin letters. All words are distinct.</p><p>It is guaranteed that the hidden word appears as one of the given <span class="tex-span"><i>m</i></span> words. Before the current move Polycarp has told exactly the letters which are currently revealed.</p>

## Output

<p>Output the single integer — the number of letters Polycarpus can tell so that the TV show host definitely reveals at least one more letter. It is possible that this number is zero.</p>





```input1
4
a**d
2
abcd
acbd

```




```input2
5
lo*er
2
lover
loser

```




```input3
3
a*a
2
aaa
aba

```




```output1
2

```




```output2
0

```




```output3
1

```



## Note

<p>In the first example Polycarpus can tell letters "<span class="tex-font-style-tt">b</span>" and "<span class="tex-font-style-tt">c</span>", which assuredly will be revealed.</p><p>The second example contains no letters which can be told as it is not clear, which of the letters "<span class="tex-font-style-tt">v</span>" or "<span class="tex-font-style-tt">s</span>" is located at the third position of the hidden word.</p><p>In the third example Polycarpus exactly knows that the hidden word is "<span class="tex-font-style-tt">aba</span>", because in case it was "<span class="tex-font-style-tt">aaa</span>", then the second letter "<span class="tex-font-style-tt">a</span>" would have already been revealed in one of previous turns.</p>
