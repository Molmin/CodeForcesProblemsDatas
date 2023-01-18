## Description

<div><p>Petya has <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. </p><p>His friend Vasya decided to joke and replaced all digits in Petya's numbers with a letters. He used the lowercase letters of the Latin alphabet from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">j</span>' and replaced all digits <span class="tex-font-style-tt">0</span> with one letter, all digits <span class="tex-font-style-tt">1</span> with another letter and so on. For any two different digits Vasya used distinct letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">j</span>'.</p><p>Your task is to restore Petya's numbers. The restored numbers should be <span class="tex-font-style-bf">positive integers</span> without leading zeros. Since there can be multiple ways to do it, determine the <span class="tex-font-style-bf">minimum</span> possible sum of all Petya's numbers after the restoration. It is guaranteed that before Vasya's joke all Petya's numbers did not have leading zeros.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>) — the number of Petya's numbers.</p><p>Each of the following lines contains non-empty string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consisting of lowercase Latin letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">j</span>' — the Petya's numbers after Vasya's joke. The length of each string does not exceed six characters.</p></div><div class="output-specification"><p>Determine the <span class="tex-font-style-bf">minimum</span> sum of all Petya's numbers after the restoration. The restored numbers should be <span class="tex-font-style-bf">positive integers</span> without leading zeros. It is guaranteed that the correct restore (without leading zeros) exists for all given tests.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>) — the number of Petya's numbers.</p><p>Each of the following lines contains non-empty string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consisting of lowercase Latin letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">j</span>' — the Petya's numbers after Vasya's joke. The length of each string does not exceed six characters.</p>

## Output

<p>Determine the <span class="tex-font-style-bf">minimum</span> sum of all Petya's numbers after the restoration. The restored numbers should be <span class="tex-font-style-bf">positive integers</span> without leading zeros. It is guaranteed that the correct restore (without leading zeros) exists for all given tests.</p>





```input1
3
ab
de
aj

```




```input2
5
abcdef
ghij
bdef
accbd
g

```




```input3
3
aa
jj
aa

```




```output1
47

```




```output2
136542

```




```output3
44

```



## Note

<p>In the first example, you need to replace the letter '<span class="tex-font-style-tt">a</span>' with the digit <span class="tex-span">1</span>, the letter '<span class="tex-font-style-tt">b</span>' with the digit <span class="tex-span">0</span>, the letter '<span class="tex-font-style-tt">d</span>' with the digit <span class="tex-span">2</span>, the letter '<span class="tex-font-style-tt">e</span>' with the digit <span class="tex-span">3</span>, and the letter '<span class="tex-font-style-tt">j</span>' with the digit <span class="tex-span">4</span>. So after the restoration numbers will look like <span class="tex-span">[10, 23, 14]</span>. The sum of them is equal to <span class="tex-span">47</span>, which is the minimum possible sum of the numbers after the correct restoration.</p><p>In the second example the numbers after the restoration can look like: <span class="tex-span">[120468, 3579, 2468, 10024, 3]</span>. </p><p>In the second example the numbers after the restoration can look like: <span class="tex-span">[11, 22, 11]</span>. </p>
