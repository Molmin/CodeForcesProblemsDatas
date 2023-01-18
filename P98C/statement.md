## Description

<div><p>A very unusual citizen lives in a far away kingdom — Dwarf Gracula. However, his unusual name is not the weirdest thing (besides, everyone long ago got used to calling him simply Dwarf Greg). What is special about Dwarf Greg — he's been living for over 200 years; besides, he lives in a crypt on an abandoned cemetery and nobody has ever seen him out in daytime. Moreover, nobody has ever seen Greg buy himself any food. That's why nobody got particularly surprised when after the infernal dragon's tragic death cattle continued to disappear from fields. The people in the neighborhood were long sure that the harmless dragon was never responsible for disappearing cattle (considering that the dragon used to be sincere about his vegetarian views). But even that's not the worst part of the whole story.</p><p>The worst part is that merely several minutes ago Dwarf Greg in some unintelligible way got inside your house and asked you to help him solve a problem. The point is that a short time ago Greg decided to order a new coffin (knowing his peculiar character, you are not surprised at all). But the problem is: a very long in both directions L-shaped corridor leads to Greg's crypt, and you can't drag just any coffin through that corridor. That's why he asked you to help.</p><center> <img class="tex-graphics" src="file://UTSE4ocF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You've formalized the task on a plane like this: let the corridor's width before and after the turn be equal to <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> correspondingly (see the picture). The corridor turns directly at a right angle, the coffin is a rectangle whose length and width are equal to <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span"><i>l</i> ≥ <i>w</i></span>) correspondingly. Dwarf Greg has already determined the coffin's length (<span class="tex-span"><i>l</i></span>), which is based on his height; your task is to determine the coffin's maximally possible width (<span class="tex-span"><i>w</i></span>), at which it can be brought to the crypt. Besides, due to its large mass (pure marble!) the coffin is equipped with rotating wheels; therefore it is impossible to lift it off the ground, however, arbitrary moves and rotations of the coffin in the plane become possible. The coffin may be rotated arbitrarily just before you drag it into crypt and move through the corridor.</p><p>Greg promised that if you help him, he will grant you immortality (I wonder how?). And if you don't, well... trust me, you don't want to know what happens if you don't help him...</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>l</i></span> from the problem's statement (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>l</i> ≤ 10<sup class="upper-index">4</sup></span>).</p></div><div class="output-specification"><p>Print the maximally possible width of a coffin with absolute or relative error no more than <span class="tex-span">10<sup class="upper-index"> - 7</sup></span>. If a coffin with the given length and positive width (the coffin that would meet the conditions from the problem's statement) does not exist, print "<span class="tex-font-style-tt">My poor head =(</span>" (without quotes).</p><p>It is guaranteed that if the answer is positive, it will be not less than <span class="tex-span">10<sup class="upper-index"> - 7</sup></span>. All the hacks will also be checked to meet that condition.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>l</i></span> from the problem's statement (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>l</i> ≤ 10<sup class="upper-index">4</sup></span>).</p>

## Output

<p>Print the maximally possible width of a coffin with absolute or relative error no more than <span class="tex-span">10<sup class="upper-index"> - 7</sup></span>. If a coffin with the given length and positive width (the coffin that would meet the conditions from the problem's statement) does not exist, print "<span class="tex-font-style-tt">My poor head =(</span>" (without quotes).</p><p>It is guaranteed that if the answer is positive, it will be not less than <span class="tex-span">10<sup class="upper-index"> - 7</sup></span>. All the hacks will also be checked to meet that condition.</p>





```input1
2 2 1

```




```input2
2 2 2

```




```input3
2 2 3

```




```input4
2 2 6

```




```output1
1.0000000

```




```output2
2.0000000
```




```output3
1.3284271

```




```output4
My poor head =(

```



## Note

<p>In the first example the answer is restricted by the coffin's length (remember — coffin's widths should not be larger than it's length).</p><p>In the second example it is possible to drag the coffin through the corridor thanks to rotating wheels: firstly, drag it forward by one side while it will not be hampered by the wall, then move it forward by adjacent side perpendicularly to the initial movement direction (remember — arbitrary moves and rotations of the coffin are possible).</p>
