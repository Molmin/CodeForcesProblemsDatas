## Description

<div><p>Sometimes Mister B has free evenings when he doesn't know what to do. Fortunately, Mister B found a new game, where the player can play against aliens.</p><p>All characters in this game are lowercase English letters. There are two players: Mister B and his competitor.</p><p>Initially the players have a string <span class="tex-span"><i>s</i></span> consisting of the first <span class="tex-span"><i>a</i></span> English letters in alphabetical order (for example, if <span class="tex-span"><i>a</i> = 5</span>, then <span class="tex-span"><i>s</i></span> equals to "<span class="tex-font-style-tt">abcde</span>").</p><p>The players take turns appending letters to string <span class="tex-span"><i>s</i></span>. Mister B moves first.</p><p>Mister B must append exactly <span class="tex-span"><i>b</i></span> letters on each his move. He can arbitrary choose these letters. His opponent adds exactly <span class="tex-span"><i>a</i></span> letters on each move.</p><p>Mister B quickly understood that his opponent was just a computer that used a simple algorithm. The computer on each turn considers the suffix of string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>a</i></span> and generates a string <span class="tex-span"><i>t</i></span> of length <span class="tex-span"><i>a</i></span> such that all letters in the string <span class="tex-span"><i>t</i></span> are distinct and don't appear in the considered suffix. From multiple variants of <span class="tex-span"><i>t</i></span> lexicographically minimal is chosen (if <span class="tex-span"><i>a</i> = 4</span> and the suffix is "<span class="tex-font-style-tt">bfdd</span>", the computer chooses string <span class="tex-span"><i>t</i></span> equal to "<span class="tex-font-style-tt">aceg</span>"). After that the chosen string <span class="tex-span"><i>t</i></span> is appended to the end of <span class="tex-span"><i>s</i></span>.</p><p>Mister B soon found the game boring and came up with the following question: what can be the minimum possible number of different letters in string <span class="tex-span"><i>s</i></span> on the segment between positions <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>, inclusive. Letters of string <span class="tex-span"><i>s</i></span> are numerated starting from <span class="tex-span">1</span>.</p></div><div class="input-specification"><p>First and only line contains four space-separated integers: <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 12</span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>) — the numbers of letters each player appends and the bounds of the segment.</p></div><div class="output-specification"><p>Print one integer — the minimum possible number of different letters in the segment from position <span class="tex-span"><i>l</i></span> to position <span class="tex-span"><i>r</i></span>, inclusive, in string <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>First and only line contains four space-separated integers: <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 12</span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>) — the numbers of letters each player appends and the bounds of the segment.</p>

## Output

<p>Print one integer — the minimum possible number of different letters in the segment from position <span class="tex-span"><i>l</i></span> to position <span class="tex-span"><i>r</i></span>, inclusive, in string <span class="tex-span"><i>s</i></span>.</p>





```input1
1 1 1 8

```




```input2
4 2 2 6

```




```input3
3 7 4 6

```




```output1
2
```




```output2
3
```




```output3
1
```



## Note

<p>In the first sample test one of optimal strategies generate string <span class="tex-span"><i>s</i> = </span>"<span class="tex-font-style-tt">abababab...</span>", that's why answer is <span class="tex-span">2</span>.</p><p>In the second sample test string <span class="tex-span"><i>s</i> = </span>"<span class="tex-font-style-tt">abcdbcaefg...</span>" can be obtained, chosen segment will look like "<span class="tex-font-style-tt">bcdbc</span>", that's why answer is <span class="tex-span">3</span>.</p><p>In the third sample test string <span class="tex-span"><i>s</i> = </span>"<span class="tex-font-style-tt">abczzzacad...</span>" can be obtained, chosen, segment will look like "<span class="tex-font-style-tt">zzz</span>", that's why answer is <span class="tex-span">1</span>.</p>
