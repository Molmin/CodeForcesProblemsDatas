## Description

<div><p>On a cold winter evening our hero Vasya stood in a railway queue to buy a ticket for Codeforces championship final. As it usually happens, the cashier said he was going to be away for 5 minutes and left for an hour. Then Vasya, not to get bored, started to analyze such a mechanism as a queue. The findings astonished Vasya.</p><p>Every man is characterized by two numbers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, which is the importance of his current task (the greater the number is, the more important the task is) and number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, which is a picture of his conscience. Numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> form the permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>Let the queue consist of <span class="tex-span"><i>n</i> - 1</span> people at the moment. Let's look at the way the person who came number <span class="tex-span"><i>n</i></span> behaves. First, he stands at the end of the queue and the does the following: if importance of the task <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of the man in front of him is less than <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>, they swap their places (it looks like this: the man number <span class="tex-span"><i>n</i></span> asks the one before him: "Erm... Excuse me please but it's very important for me... could you please let me move up the queue?"), then he again poses the question to the man in front of him and so on. But in case when <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is greater than <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>, moving up the queue stops. However, the man number <span class="tex-span"><i>n</i></span> can perform the operation no more than <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span> times.</p><p>In our task let us suppose that by the moment when the man number <span class="tex-span"><i>n</i></span> joins the queue, the process of swaps between <span class="tex-span"><i>n</i> - 1</span> will have stopped. If the swap is possible it necessarily takes place.</p><p>Your task is to help Vasya model the described process and find the order in which the people will stand in queue when all the swaps stops.</p></div><div class="input-specification"><p>The first input line contains an integer <span class="tex-span"><i>n</i></span> which is the number of people who has joined the queue (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). In the next <span class="tex-span"><i>n</i></span> lines descriptions of the people are given in order of their coming — space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). Every description is located on s single line. All the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s are different.</p></div><div class="output-specification"><p>Output the permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, which signifies the queue formed according to the above described rules, starting from the beginning to the end. In this succession the <span class="tex-span"><i>i</i></span>-th number stands for the number of a person who will stand in line on the place number <span class="tex-span"><i>i</i></span> after the swaps ends. People are numbered starting with <span class="tex-span">1</span> in the order in which they were given in the input. Separate numbers by a space.</p></div>

## Input

<p>The first input line contains an integer <span class="tex-span"><i>n</i></span> which is the number of people who has joined the queue (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). In the next <span class="tex-span"><i>n</i></span> lines descriptions of the people are given in order of their coming — space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). Every description is located on s single line. All the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s are different.</p>

## Output

<p>Output the permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, which signifies the queue formed according to the above described rules, starting from the beginning to the end. In this succession the <span class="tex-span"><i>i</i></span>-th number stands for the number of a person who will stand in line on the place number <span class="tex-span"><i>i</i></span> after the swaps ends. People are numbered starting with <span class="tex-span">1</span> in the order in which they were given in the input. Separate numbers by a space.</p>





```input1
2
1 0
2 1

```




```input2
3
1 3
2 3
3 3

```




```input3
5
2 3
1 4
4 3
3 1
5 2

```




```output1
2 1
```




```output2
3 2 1
```




```output3
3 1 5 4 2
```


