## Description

<div><p>Nastya received a gift on New Year&nbsp;— a magic wardrobe. It is magic because in the end of each month the number of dresses in it doubles (i.e. the number of dresses becomes twice as large as it is in the beginning of the month).</p><p>Unfortunately, right after the doubling the wardrobe eats one of the dresses (if any) with the <span class="tex-span">50%</span> probability. It happens every month except the last one in the year. </p><p>Nastya owns <span class="tex-span"><i>x</i></span> dresses now, so she became interested in the <a href="https://en.wikipedia.org/wiki/Expected_value">expected number</a> of dresses she will have in one year. Nastya lives in Byteland, so the year lasts for <span class="tex-span"><i>k</i> + 1</span> months.</p><p>Nastya is really busy, so she wants you to solve this problem. You are the programmer, after all. Also, you should find the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>, because it is easy to see that it is always integer.</p></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>x</i>, <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>), where <span class="tex-span"><i>x</i></span> is the initial number of dresses and <span class="tex-span"><i>k</i> + 1</span> is the number of months in a year in Byteland.</p></div><div class="output-specification"><p>In the only line print a single integer&nbsp;— the expected number of dresses Nastya will own one year later modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>x</i>, <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>), where <span class="tex-span"><i>x</i></span> is the initial number of dresses and <span class="tex-span"><i>k</i> + 1</span> is the number of months in a year in Byteland.</p>

## Output

<p>In the only line print a single integer&nbsp;— the expected number of dresses Nastya will own one year later modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2 0

```




```input2
2 1

```




```input3
3 2

```




```output1
4

```




```output2
7

```




```output3
21

```



## Note

<p>In the first example a year consists on only one month, so the wardrobe does not eat dresses at all.</p><p>In the second example after the first month there are <span class="tex-span">3</span> dresses with <span class="tex-span">50%</span> probability and <span class="tex-span">4</span> dresses with <span class="tex-span">50%</span> probability. Thus, in the end of the year there are <span class="tex-span">6</span> dresses with <span class="tex-span">50%</span> probability and <span class="tex-span">8</span> dresses with <span class="tex-span">50%</span> probability. This way the answer for this test is <span class="tex-span">(6 + 8) / 2 = 7</span>.</p>
