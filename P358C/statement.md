## Description

<div><p>Dima has a birthday soon! It's a big day! Saryozha's present to Dima is that Seryozha won't be in the room and won't disturb Dima and Inna as they celebrate the birthday. Inna's present to Dima is a stack, a queue and a deck.</p><p>Inna wants her present to show Dima how great a programmer he is. For that, she is going to give Dima commands one by one. There are two types of commands:</p><ol> <li> Add a given number into one of containers. For the queue and the stack, you can add elements only to the end. For the deck, you can add elements to the beginning and to the end. </li><li> Extract a number from each of at most three distinct containers. Tell all extracted numbers to Inna and then empty all containers. In the queue container you can extract numbers only from the beginning. In the stack container you can extract numbers only from the end. In the deck number you can extract numbers from the beginning and from the end. You cannot extract numbers from empty containers. </li></ol><p>Every time Dima makes a command of the second type, Inna kisses Dima some (possibly zero) number of times. Dima knows Inna perfectly well, he is sure that this number equals the sum of numbers he extracts from containers during this operation.</p><p>As we've said before, Dima knows Inna perfectly well and he knows which commands Inna will give to Dima and the order of the commands. Help Dima find the strategy that lets him give as more kisses as possible for his birthday!</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of Inna's commands. Then <span class="tex-span"><i>n</i></span> lines follow, describing Inna's commands. Each line consists an integer:</p><ol> <li> Integer <span class="tex-span"><i>a</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ 10<sup class="upper-index">5</sup>)</span> means that Inna gives Dima a command to add number <span class="tex-span"><i>a</i></span> into one of containers. </li><li> Integer <span class="tex-span">0</span> shows that Inna asks Dima to make at most three extractions from different containers. </li></ol></div><div class="output-specification"><p>Each command of the input must correspond to one line of the output — Dima's action.</p><p>For the command of the first type (adding) print one word that corresponds to Dima's choice:</p><ul> <li> pushStack — add to the end of the stack; </li><li> pushQueue — add to the end of the queue; </li><li> pushFront — add to the beginning of the deck; </li><li> pushBack — add to the end of the deck. </li></ul><p>For a command of the second type first print an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 3)</span>, that shows the number of extract operations, then print <span class="tex-span"><i>k</i></span> words separated by space. The words can be:</p><ul> <li> popStack — extract from the end of the stack; </li><li> popQueue — extract from the beginning of the line; </li><li> popFront — extract from the beginning from the deck; </li><li> popBack — extract from the end of the deck. </li></ul><p>The printed operations mustn't extract numbers from empty containers. Also, they must extract numbers from distinct containers.</p><p>The printed sequence of actions must lead to the maximum number of kisses. If there are multiple sequences of actions leading to the maximum number of kisses, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of Inna's commands. Then <span class="tex-span"><i>n</i></span> lines follow, describing Inna's commands. Each line consists an integer:</p><ol> <li> Integer <span class="tex-span"><i>a</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ 10<sup class="upper-index">5</sup>)</span> means that Inna gives Dima a command to add number <span class="tex-span"><i>a</i></span> into one of containers. </li><li> Integer <span class="tex-span">0</span> shows that Inna asks Dima to make at most three extractions from different containers. </li></ol>

## Output

<p>Each command of the input must correspond to one line of the output — Dima's action.</p><p>For the command of the first type (adding) print one word that corresponds to Dima's choice:</p><ul> <li> pushStack — add to the end of the stack; </li><li> pushQueue — add to the end of the queue; </li><li> pushFront — add to the beginning of the deck; </li><li> pushBack — add to the end of the deck. </li></ul><p>For a command of the second type first print an integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(0 ≤ <i>k</i> ≤ 3)</span>, that shows the number of extract operations, then print <span class="tex-span"><i>k</i></span> words separated by space. The words can be:</p><ul> <li> popStack — extract from the end of the stack; </li><li> popQueue — extract from the beginning of the line; </li><li> popFront — extract from the beginning from the deck; </li><li> popBack — extract from the end of the deck. </li></ul><p>The printed operations mustn't extract numbers from empty containers. Also, they must extract numbers from distinct containers.</p><p>The printed sequence of actions must lead to the maximum number of kisses. If there are multiple sequences of actions leading to the maximum number of kisses, you are allowed to print any of them.</p>





```input1
10
0
1
0
1
2
0
1
2
3
0

```




```input2
4
1
2
3
0

```




```output1
0
pushStack
1 popStack
pushStack
pushQueue
2 popStack popQueue
pushStack
pushQueue
pushFront
3 popStack popQueue popFront

```




```output2
pushStack
pushQueue
pushFront
3 popStack popQueue popFront

```


