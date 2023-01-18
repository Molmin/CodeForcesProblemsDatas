## Description

<div><p>There are <span class="tex-span"><i>n</i></span> phone numbers in Polycarp's contacts on his phone. Each number is a 9-digit integer, starting with a digit different from <span class="tex-span">0</span>. All the numbers are distinct.</p><p>There is the latest version of Berdroid OS installed on Polycarp's phone. If some number is entered, is shows up all the numbers in the contacts for which there is a substring equal to the entered sequence of digits. For example, is there are three phone numbers in Polycarp's contacts: <span class="tex-span">123456789</span>, <span class="tex-span">100000000</span> and <span class="tex-span">100123456</span>, then:</p><ul> <li> if he enters <span class="tex-span">00</span> two numbers will show up: <span class="tex-span">100000000</span> and <span class="tex-span">100123456</span>, </li><li> if he enters <span class="tex-span">123</span> two numbers will show up <span class="tex-span">123456789</span> and <span class="tex-span">100123456</span>, </li><li> if he enters <span class="tex-span">01</span> there will be only one number <span class="tex-span">100123456</span>. </li></ul><p>For each of the phone numbers in Polycarp's contacts, find the minimum in length sequence of digits such that if Polycarp enters this sequence, Berdroid shows this only phone number.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 70000</span>) — the total number of phone contacts in Polycarp's contacts.</p><p>The phone numbers follow, one in each line. Each number is a positive 9-digit integer starting with a digit from <span class="tex-span">1</span> to <span class="tex-span">9</span>. All the numbers are distinct.</p></div><div class="output-specification"><p>Print exactly <span class="tex-span"><i>n</i></span> lines: the <span class="tex-span"><i>i</i></span>-th of them should contain the shortest non-empty sequence of digits, such that if Polycarp enters it, the Berdroid OS shows up only the <span class="tex-span"><i>i</i></span>-th number from the contacts. If there are several such sequences, print any of them.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 70000</span>) — the total number of phone contacts in Polycarp's contacts.</p><p>The phone numbers follow, one in each line. Each number is a positive 9-digit integer starting with a digit from <span class="tex-span">1</span> to <span class="tex-span">9</span>. All the numbers are distinct.</p>

## Output

<p>Print exactly <span class="tex-span"><i>n</i></span> lines: the <span class="tex-span"><i>i</i></span>-th of them should contain the shortest non-empty sequence of digits, such that if Polycarp enters it, the Berdroid OS shows up only the <span class="tex-span"><i>i</i></span>-th number from the contacts. If there are several such sequences, print any of them.</p>





```input1
3
123456789
100000000
100123456

```




```input2
4
123456789
193456789
134567819
934567891

```




```output1
9
000
01

```




```output2
2
193
81
91

```


