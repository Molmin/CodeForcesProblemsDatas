## Description

<div><p>Once upon a time an old man and his wife lived by the great blue sea. One day the old man went fishing and caught a real live gold fish. The fish said: "Oh ye, old fisherman! Pray set me free to the ocean and I will grant you with <span class="tex-span"><i>n</i></span> gifts, any gifts you wish!". Then the fish gave the old man a list of gifts and their prices. Some gifts on the list can have the same names but distinct prices. However, there can't be two gifts with the same names and the same prices. Also, there can be gifts with distinct names and the same prices. The old man can ask for <span class="tex-span"><i>n</i></span> names of items from the list. If the fish's list has <span class="tex-span"><i>p</i></span> occurrences of the given name, then the old man can't ask for this name of item more than <span class="tex-span"><i>p</i></span> times.</p><p>The old man knows that if he asks for <span class="tex-span"><i>s</i></span> gifts of the same name, the fish will randomly (i.e. uniformly amongst all possible choices) choose <span class="tex-span"><i>s</i></span> gifts of distinct prices with such name from the list. The old man wants to please his greedy wife, so he will choose the <span class="tex-span"><i>n</i></span> names in such a way that he can get <span class="tex-span"><i>n</i></span> gifts with the maximum price. Besides, he isn't the brightest of fishermen, so if there are several such ways, he chooses one of them uniformly.</p><p>The old man wondered, what is the probability that he can get <span class="tex-span"><i>n</i></span> most expensive gifts. As the old man isn't good at probability theory, he asks you to help him.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the number of the old man's wishes and the number of distinct names in the goldfish's list, correspondingly. Then <span class="tex-span"><i>m</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line first contains integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>k</i><sub class="lower-index"><i>i</i></sub> &gt; 0)</span>&nbsp;— the number of distinct prices of gifts with the <span class="tex-span"><i>i</i></span>-th name, then <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the gifts' prices. </p><p>It is guaranteed that the sum of all <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed 1000. It is guaranteed that <span class="tex-span"><i>n</i></span> is not greater than the total number of the gifts.</p></div><div class="output-specification"><p>On a single line print one real number — the probability of getting <span class="tex-span"><i>n</i></span> most valuable gifts. The answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the number of the old man's wishes and the number of distinct names in the goldfish's list, correspondingly. Then <span class="tex-span"><i>m</i></span> lines follow: the <span class="tex-span"><i>i</i></span>-th line first contains integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>k</i><sub class="lower-index"><i>i</i></sub> &gt; 0)</span>&nbsp;— the number of distinct prices of gifts with the <span class="tex-span"><i>i</i></span>-th name, then <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the gifts' prices. </p><p>It is guaranteed that the sum of all <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed 1000. It is guaranteed that <span class="tex-span"><i>n</i></span> is not greater than the total number of the gifts.</p>

## Output

<p>On a single line print one real number — the probability of getting <span class="tex-span"><i>n</i></span> most valuable gifts. The answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
3 1
3 10 20 30

```




```input2
3 2
1 40
4 10 20 30 40

```




```output1
1.000000000

```




```output2
0.166666667

```


