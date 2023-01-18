## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. Everybody knows that lucky numbers are positive integers whose decimal representation contains only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya has a number consisting of <span class="tex-span"><i>n</i></span> digits without leading zeroes. He represented it as an array of digits without leading zeroes. Let's call it <span class="tex-span"><i>d</i></span>. The numeration starts with <span class="tex-span">1</span>, starting from the most significant digit. Petya wants to perform the following <span class="tex-font-style-underline">operation</span> <span class="tex-span"><i>k</i></span> times: find the minimum <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> &lt; <i>n</i>)</span> such that <span class="tex-span"><i>d</i><sub class="lower-index"><i>x</i></sub> = 4</span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>x</i> + 1</sub> = 7</span>, if <span class="tex-span"><i>x</i></span> is odd, then to assign <span class="tex-span"><i>d</i><sub class="lower-index"><i>x</i></sub> = <i>d</i><sub class="lower-index"><i>x</i> + 1</sub> = 4</span>, otherwise to assign <span class="tex-span"><i>d</i><sub class="lower-index"><i>x</i></sub> = <i>d</i><sub class="lower-index"><i>x</i> + 1</sub> = 7</span>. Note that if no <span class="tex-span"><i>x</i></span> was found, then the operation counts as completed and the array doesn't change at all.</p><p>You are given the initial number as an array of digits and the number <span class="tex-span"><i>k</i></span>. Help Petya find the result of completing <span class="tex-span"><i>k</i></span> operations.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the number of digits in the number and the number of completed operations. The second line contains <span class="tex-span"><i>n</i></span> digits without spaces representing the array of digits <span class="tex-span"><i>d</i></span>, starting with <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span>. It is guaranteed that the first digit of the number does not equal zero.</p></div><div class="output-specification"><p>In the single line print the result without spaces — the number after the <span class="tex-span"><i>k</i></span> operations are fulfilled.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the number of digits in the number and the number of completed operations. The second line contains <span class="tex-span"><i>n</i></span> digits without spaces representing the array of digits <span class="tex-span"><i>d</i></span>, starting with <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span>. It is guaranteed that the first digit of the number does not equal zero.</p>

## Output

<p>In the single line print the result without spaces — the number after the <span class="tex-span"><i>k</i></span> operations are fulfilled.</p>





```input1
7 4
4727447

```




```input2
4 2
4478

```




```output1
4427477

```




```output2
4478

```



## Note

<p>In the first sample the number changes in the following sequence: <span class="tex-span">4727447 → 4427447 → 4427477 → 4427447 → 4427477</span>.</p><p>In the second sample: <span class="tex-span">4478 → 4778 → 4478</span>.</p>
