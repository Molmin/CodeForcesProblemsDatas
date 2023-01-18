## Description

<div><p>Vasya the Great Magician and Conjurer loves all kinds of miracles and wizardry. In one wave of a magic wand he can turn an object into something else. But, as you all know, there is no better magic in the Universe than the magic of numbers. That's why Vasya adores math and spends a lot of time turning some numbers into some other ones.</p><p>This morning he has <span class="tex-span"><i>n</i></span> cards with integers lined up in front of him. Each integer is not less than 1, but not greater than <span class="tex-span"><i>l</i></span>. When Vasya waves his magic wand, two rightmost cards vanish from the line and a new card magically appears in their place. It contains the difference between the left and the right numbers on the two vanished cards. Vasya was very interested to know what would happen next, and so he waved with his magic wand on and on, until the table had a single card left.</p><p>Suppose that Vasya originally had the following cards: 4, 1, 1, 3 (listed from left to right). Then after the first wave the line would be: 4, 1, -2, and after the second one: 4, 3, and after the third one the table would have a single card with number 1.</p><p>Please note that in spite of the fact that initially all the numbers on the cards were not less than 1 and not greater than <span class="tex-span"><i>l</i></span>, the numbers on the appearing cards can be anything, no restrictions are imposed on them.</p><p>It is now evening. Vasya is very tired and wants to return everything back, but does not remember which cards he had in the morning. He only remembers that there were <span class="tex-span"><i>n</i></span> cards, they contained integers from 1 to <span class="tex-span"><i>l</i></span>, and after all magical actions he was left with a single card containing number <span class="tex-span"><i>d</i></span>.</p><p>Help Vasya to recover the initial set of cards with numbers.</p></div><div class="input-specification"><p>The single line contains three space-separated integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the initial number of cards on the table, <span class="tex-span"><i>d</i></span> (<span class="tex-span">|<i>d</i>| ≤ 10<sup class="upper-index">4</sup></span>) — the number on the card that was left on the table after all the magical actions, and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ 100</span>) — the limits for the initial integers.</p></div><div class="output-specification"><p>If Vasya is mistaken, that is, if there doesn't exist a set that meets the requirements given in the statement, then print a single number -1, otherwise print the sought set containing <span class="tex-span"><i>n</i></span> integers from <span class="tex-span">1</span> to <span class="tex-span"><i>l</i></span>. Separate the integers by spaces. Print the integers in the order, in which they were written on the cards from left to right. If there are several suitable sets of numbers, you can print any of them.</p></div>

## Input

<p>The single line contains three space-separated integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the initial number of cards on the table, <span class="tex-span"><i>d</i></span> (<span class="tex-span">|<i>d</i>| ≤ 10<sup class="upper-index">4</sup></span>) — the number on the card that was left on the table after all the magical actions, and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ 100</span>) — the limits for the initial integers.</p>

## Output

<p>If Vasya is mistaken, that is, if there doesn't exist a set that meets the requirements given in the statement, then print a single number -1, otherwise print the sought set containing <span class="tex-span"><i>n</i></span> integers from <span class="tex-span">1</span> to <span class="tex-span"><i>l</i></span>. Separate the integers by spaces. Print the integers in the order, in which they were written on the cards from left to right. If there are several suitable sets of numbers, you can print any of them.</p>





```input1
3 3 2

```




```input2
5 -4 3

```




```input3
5 -4 4

```




```output1
2 1 2
```




```output2
-1

```




```output3
2 4 1 4 1
```


