## Description

<div><p>Some dwarves that are finishing the StUDY (State University for Dwarven Youngsters) Bachelor courses, have been told "no genome, no degree". That means that all dwarves should write a thesis on genome. Dwarven genome is far from simple. It is represented by a string that consists of lowercase Latin letters.</p><p>Dwarf Misha has already chosen the subject for his thesis: determining by two dwarven genomes, whether they belong to the same race. Two dwarves belong to the same race if we can swap two characters in the first dwarf's genome and get the second dwarf's genome as a result. Help Dwarf Misha and find out whether two gnomes belong to the same race or not.</p></div><div class="input-specification"><p>The first line contains the first dwarf's genome: a non-empty string, consisting of lowercase Latin letters.</p><p>The second line contains the second dwarf's genome: a non-empty string, consisting of lowercase Latin letters.</p><p>The number of letters in each genome doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. It is guaranteed that the strings that correspond to the genomes are different. The given genomes may have different length.</p></div><div class="output-specification"><p>Print "YES", if the dwarves belong to the same race. Otherwise, print "NO".</p></div>

## Input

<p>The first line contains the first dwarf's genome: a non-empty string, consisting of lowercase Latin letters.</p><p>The second line contains the second dwarf's genome: a non-empty string, consisting of lowercase Latin letters.</p><p>The number of letters in each genome doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. It is guaranteed that the strings that correspond to the genomes are different. The given genomes may have different length.</p>

## Output

<p>Print "YES", if the dwarves belong to the same race. Otherwise, print "NO".</p>





```input1
ab
ba

```




```input2
aa
ab

```




```output1
YES

```




```output2
NO

```



## Note

<ul> <li> First example: you can simply swap two letters in string "ab". So we get "ba". </li><li> Second example: we can't change string "aa" into string "ab", because "aa" does not contain letter "b". </li></ul>
