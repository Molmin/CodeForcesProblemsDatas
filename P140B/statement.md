## Description

<div><p>As meticulous Gerald sets the table, Alexander finished another post on Codeforces and begins to respond to New Year greetings from friends. Alexander has <span class="tex-span"><i>n</i></span> friends, and each of them sends to Alexander exactly one e-card. Let us number his friends by numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order in which they send the cards. Let's introduce the same numbering for the cards, that is, according to the numbering the <span class="tex-span"><i>i</i></span>-th friend sent to Alexander a card number <span class="tex-span"><i>i</i></span>.</p><p>Alexander also sends cards to friends, but he doesn't look for the new cards on the Net. He simply uses the cards previously sent to him (sometimes, however, he does need to add some crucial details). Initially Alexander doesn't have any cards. Alexander always follows the two rules:</p><ol> <li> He will never send to a firend a card that this friend has sent to him. </li><li> Among the other cards available to him at the moment, Alexander always chooses one that Alexander himself likes most. </li></ol><p>Alexander plans to send to each friend exactly one card. Of course, Alexander can send the same card multiple times.</p><p>Alexander and each his friend has the list of preferences, which is a permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The first number in the list is the number of the favorite card, the second number shows the second favorite, and so on, the last number shows the least favorite card.</p><p>Your task is to find a schedule of sending cards for Alexander. Determine at which moments of time Alexander must send cards to his friends, to please each of them as much as possible. In other words, so that as a result of applying two Alexander's rules, each friend receives the card that is preferred for him as much as possible.</p><p>Note that Alexander doesn't choose freely what card to send, but he always strictly follows the two rules.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 300</span>) — the number of Alexander's friends, equal to the number of cards. Next <span class="tex-span"><i>n</i></span> lines contain his friends' preference lists. Each list consists of <span class="tex-span"><i>n</i></span> different integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The last line contains Alexander's preference list in the same format.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space-separated numbers: the <span class="tex-span"><i>i</i></span>-th number should be the number of the friend, whose card Alexander receives right before he should send a card to the <span class="tex-span"><i>i</i></span>-th friend. If there are several solutions, print any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 300</span>) — the number of Alexander's friends, equal to the number of cards. Next <span class="tex-span"><i>n</i></span> lines contain his friends' preference lists. Each list consists of <span class="tex-span"><i>n</i></span> different integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The last line contains Alexander's preference list in the same format.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> space-separated numbers: the <span class="tex-span"><i>i</i></span>-th number should be the number of the friend, whose card Alexander receives right before he should send a card to the <span class="tex-span"><i>i</i></span>-th friend. If there are several solutions, print any of them.</p>





```input1
4
1 2 3 4
4 1 3 2
4 3 1 2
3 4 2 1
3 1 2 4

```




```output1
2 1 1 4

```



## Note

<p>In the sample, the algorithm of actions Alexander and his friends perform is as follows: </p><ol> <li> Alexander receives card <span class="tex-span">1</span> from the first friend. </li><li> Alexander sends the card he has received (at the moment he only has one card, and therefore it is the most preferable for him) to friends with the numbers <span class="tex-span">2</span> and <span class="tex-span">3</span>. </li><li> Alexander receives card <span class="tex-span">2</span> from the second friend, now he has two cards — <span class="tex-span">1</span> and <span class="tex-span">2</span>. </li><li> Alexander sends a card to the first friend. Despite the fact that Alexander likes card <span class="tex-span">1</span> more, he sends card <span class="tex-span">2</span> as he cannot send a friend the card sent by that very friend. </li><li> Alexander receives card <span class="tex-span">3</span> from the third friend. </li><li> Alexander receives card <span class="tex-span">4</span> from the fourth friend. </li><li> Among the cards Alexander has number <span class="tex-span">3</span> is his favorite and he sends it to the fourth friend. </li></ol><p>Note that Alexander can send cards to multiple friends at a time (in this case the second and the third one). Alexander can send card <span class="tex-span">3</span> to the fourth friend after he receives the third card or after he receives the fourth card (both variants are correct).</p>
