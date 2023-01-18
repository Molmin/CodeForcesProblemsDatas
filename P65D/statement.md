## Description

<div><p>As you know, Hogwarts has four houses: Gryffindor, Hufflepuff, Ravenclaw and Slytherin. The sorting of the first-years into houses is done by the Sorting Hat. The pupils are called one by one in the alphabetical order, each of them should put a hat on his head and, after some thought, the hat solemnly announces the name of the house the student should enter.</p><p>At that the Hat is believed to base its considerations on the student's personal qualities: it sends the brave and noble ones to Gryffindor, the smart and shrewd ones — to Ravenclaw, the persistent and honest ones — to Hufflepuff and the clever and cunning ones — to Slytherin. However, a first year student Hermione Granger got very concerned about the forthcoming sorting. She studied all the literature on the Sorting Hat and came to the conclusion that it is much simpler than that. If the relatives of the student have already studied at Hogwarts, the hat puts the student to the same house, where his family used to study. In controversial situations, when the relatives studied in different houses or when they were all Muggles like Hermione's parents, then the Hat sorts the student to the house, to which the least number of first years has been sent at that moment. If there are several such houses, the choice is given to the student himself. Then the student can choose any of the houses, to which the least number of first years has been sent so far. </p><p>Hermione has already asked the students that are on the list before her about their relatives. Now she and her new friends Harry Potter and Ron Weasley want to find out into what house the Hat will put Hermione.</p></div><div class="input-specification"><p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>). It is the number of students who are in the list before Hermione. The next line contains <span class="tex-span"><i>n</i></span> symbols. If all the relatives of a student used to study in the same house, then the <span class="tex-span"><i>i</i></span>-th character in the string coincides with the first letter of the name of this house. Otherwise, the <span class="tex-span"><i>i</i></span>-th symbol is equal to "?".</p></div><div class="output-specification"><p>Print all the possible houses where Hermione can be sent. The names of the houses should be printed in the alphabetical order, one per line.</p></div>

## Input

<p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>). It is the number of students who are in the list before Hermione. The next line contains <span class="tex-span"><i>n</i></span> symbols. If all the relatives of a student used to study in the same house, then the <span class="tex-span"><i>i</i></span>-th character in the string coincides with the first letter of the name of this house. Otherwise, the <span class="tex-span"><i>i</i></span>-th symbol is equal to "?".</p>

## Output

<p>Print all the possible houses where Hermione can be sent. The names of the houses should be printed in the alphabetical order, one per line.</p>





```input1
11
G????SS???H

```




```input2
2
H?

```




```output1
Gryffindor
Ravenclaw

```




```output2
Gryffindor
Ravenclaw
Slytherin

```



## Note

<p>Consider the second example. There are only two students before Hermione. The first student is sent to Hufflepuff. The second disciple is given the choice between the houses where the least number of students has been sent, i.e. Gryffindor, Slytherin and Ravenclaw. If he chooses Gryffindor, Hermione is forced to choose between Ravenclaw and Slytherin, if he chooses Ravenclaw, Hermione will choose between Gryffindor and Slytherin, if he chooses Slytherin, Hermione will choose between Gryffindor and Ravenclaw. In the end, the following situation is possible (it depends on the choice of the second student and Hermione). Hermione will end up 1) in Gryffindor, 2) in Ravenclaw, 3) in Slytherin. Note that, despite the fact that in neither case Hermione will be given a choice between all the three options, they are all possible and they should all be printed in the answer. Hermione will not, under any circumstances, end up in Hufflepuff.</p>
