## Description

<div><p>Alas, finding one's true love is not easy. Masha has been unsuccessful in that yet. Her friend Dasha told Masha about a way to determine the phone number of one's Prince Charming through arithmancy. </p><p>The phone number is divined like that. First one needs to write down one's own phone numbers. For example, let's suppose that Masha's phone number is <span class="tex-span">12345</span>. After that one should write her favorite digit from <span class="tex-span">0</span> to <span class="tex-span">9</span> under the first digit of her number. That will be the first digit of the needed number. For example, Masha's favorite digit is <span class="tex-span">9</span>. The second digit is determined as a half sum of the second digit of Masha's number and the already written down first digit from her beloved one's number. In this case the arithmetic average equals to <span class="tex-span">(2 + 9) / 2 = 5.5</span>. Masha can round the number up or down, depending on her wishes. For example, she chooses the digit <span class="tex-span">5</span>. Having written down the resulting digit under the second digit of her number, Masha moves to finding the third digit in the same way, i.e. finding the half sum the the third digit of her number and the second digit of the new number. The result is <span class="tex-span">(5 + 3) / 2 = 4</span>. In this case the answer is unique. Thus, every <span class="tex-span"><i>i</i></span>-th digit is determined as an arithmetic average of the <span class="tex-span"><i>i</i></span>-th digit of Masha's number and the <span class="tex-span"><i>i</i> - 1</span>-th digit of her true love's number. If needed, the digit can be rounded up or down. For example, Masha can get: </p><center class="tex-equation"><span class="tex-span">12345</span></center> <center class="tex-equation"><span class="tex-span">95444</span></center> Unfortunately, when Masha tried dialing the number, she got disappointed: as it turned out, the number was unavailable or outside the coverage area. But Masha won't give up. Perhaps, she rounded to a wrong digit or chose the first digit badly. That's why she keeps finding more and more new numbers and calling them. Count the number of numbers Masha calls. Masha calls all the possible numbers that can be found by the described means of arithmancy, except for, perhaps, her own one.</div><div class="input-specification"><p>The first line contains nonempty sequence consisting of digits from <span class="tex-span">0</span> to <span class="tex-span">9</span> — Masha's phone number. The sequence length does not exceed <span class="tex-span">50</span>.</p></div><div class="output-specification"><p>Output the single number — the number of phone numbers Masha will dial.</p></div>

## Input

<p>The first line contains nonempty sequence consisting of digits from <span class="tex-span">0</span> to <span class="tex-span">9</span> — Masha's phone number. The sequence length does not exceed <span class="tex-span">50</span>.</p>

## Output

<p>Output the single number — the number of phone numbers Masha will dial.</p>





```input1
12345

```




```input2
09

```




```output1
48

```




```output2
15

```


