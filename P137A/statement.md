## Description

<div><p>Polycarpus has postcards and photos hung in a row on the wall. He decided to put them away to the closet and hang on the wall a famous painter's picture. Polycarpus does it like that: he goes from the left to the right and removes the objects consecutively. As Polycarpus doesn't want any mix-ups to happen, he will not carry in his hands objects of two different types. In other words, Polycarpus can't carry both postcards and photos simultaneously. Sometimes he goes to the closet and puts the objects there, thus leaving his hands free. Polycarpus must put <span class="tex-font-style-bf">all</span> the postcards and photos to the closet. He cannot skip objects. What minimum number of times he should visit the closet if he cannot carry more than 5 items?</p></div><div class="input-specification"><p>The only line of the input data contains a non-empty string consisting of letters <span class="tex-font-style-tt">"С"</span> and <span class="tex-font-style-tt">"P"</span> whose length does not exceed <span class="tex-span">100</span> characters. If the <span class="tex-span"><i>i</i></span>-th character in the string is the letter <span class="tex-font-style-tt">"С"</span>, that means that the <span class="tex-span"><i>i</i></span>-th object (the numbering goes from the left to the right) on Polycarpus' wall is a postcard. And if the <span class="tex-span"><i>i</i></span>-th character is the letter <span class="tex-font-style-tt">"P"</span>, than the <span class="tex-span"><i>i</i></span>-th object on the wall is a photo.</p></div><div class="output-specification"><p>Print the only number — the minimum number of times Polycarpus has to visit the closet.</p></div>

## Input

<p>The only line of the input data contains a non-empty string consisting of letters <span class="tex-font-style-tt">"С"</span> and <span class="tex-font-style-tt">"P"</span> whose length does not exceed <span class="tex-span">100</span> characters. If the <span class="tex-span"><i>i</i></span>-th character in the string is the letter <span class="tex-font-style-tt">"С"</span>, that means that the <span class="tex-span"><i>i</i></span>-th object (the numbering goes from the left to the right) on Polycarpus' wall is a postcard. And if the <span class="tex-span"><i>i</i></span>-th character is the letter <span class="tex-font-style-tt">"P"</span>, than the <span class="tex-span"><i>i</i></span>-th object on the wall is a photo.</p>

## Output

<p>Print the only number — the minimum number of times Polycarpus has to visit the closet.</p>





```input1
CPCPCPC

```




```input2
CCCCCCPPPPPP

```




```input3
CCCCCCPPCPPPPPPPPPP

```




```input4
CCCCCCCCCC

```




```output1
7

```




```output2
4

```




```output3
6

```




```output4
2

```



## Note

<p>In the first sample Polycarpus needs to take one item to the closet 7 times.</p><p>In the second sample Polycarpus can first take 3 postcards to the closet; then 3 more. He can take the 6 photos that are left in the similar way, going to the closet twice.</p><p>In the third sample Polycarpus can visit the closet twice, both times carrying 3 postcards. Then he can take there 2 photos at once, then one postcard and finally, he can carry the last 10 photos if he visits the closet twice.</p><p>In the fourth sample Polycarpus can visit the closet twice and take there all 10 postcards (5 items during each go).</p>
