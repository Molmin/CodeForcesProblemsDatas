## Description

<div><p>Recently, Valery have come across an entirely new programming language. Most of all the language attracted him with template functions and procedures. Let us remind you that templates are tools of a language, designed to encode generic algorithms, without reference to some parameters (e.g., data types, buffer sizes, default values).</p><p>Valery decided to examine template procedures in this language in more detail. The description of a template procedure consists of the procedure name and the list of its parameter types. The generic type <span class="tex-font-style-tt">T</span> parameters can be used as parameters of template procedures.</p><p>A procedure call consists of a procedure name and a list of variable parameters. Let's call a procedure <span class="tex-font-style-it">suitable</span> for this call if the following conditions are fulfilled: </p><ul> <li> its name equals to the name of the called procedure; </li><li> the number of its parameters equals to the number of parameters of the procedure call; </li><li> the types of variables in the procedure call match the corresponding types of its parameters. The variable type matches the type of a parameter if the parameter has a generic type <span class="tex-font-style-tt">T</span> or the type of the variable and the parameter are the same. </li></ul><p>You are given a description of some set of template procedures. You are also given a list of variables used in the program, as well as direct procedure calls that use the described variables. For each call you need to count the number of procedures that are suitable for this call.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of template procedures. The next <span class="tex-span"><i>n</i></span> lines contain the description of the procedures specified in the following format:</p><p>"<span class="tex-font-style-tt">void procedureName (type_1, type_2, ..., type_t)</span>" (<span class="tex-span">1 ≤ <i>t</i> ≤ 5</span>), where <span class="tex-font-style-tt">void</span> is the keyword, <span class="tex-font-style-tt">procedureName</span> is the procedure name, <span class="tex-font-style-tt">type_i</span> is the type of the next parameter. Types of language parameters can be "<span class="tex-font-style-tt">int</span>", "<span class="tex-font-style-tt">string</span>", "<span class="tex-font-style-tt">double</span>", and the keyword "<span class="tex-font-style-tt">T</span>", which denotes the generic type.</p><p>The next line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>) — the number of used variables. Next <span class="tex-span"><i>m</i></span> lines specify the description of the variables in the following format:</p><p>"<span class="tex-font-style-tt">type variableName"</span>, where <span class="tex-font-style-tt">type</span> is the type of variable that can take values "<span class="tex-font-style-tt">int</span>", "<span class="tex-font-style-tt">string</span>", "<span class="tex-font-style-tt">double</span>", <span class="tex-font-style-tt">variableName</span> — the name of the variable.</p><p>The next line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) — the number of procedure calls. Next <span class="tex-span"><i>k</i></span> lines specify the procedure calls in the following format:</p><p>"<span class="tex-font-style-tt">procedureName (var_1, var_2, ..., var_t)"</span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 5</span>), where <span class="tex-font-style-tt">procedureName</span> is the name of the procedure, <span class="tex-font-style-tt">var_i</span> is the name of a variable.</p><p>The lines describing the variables, template procedures and their calls may contain spaces at the beginning of the line and at the end of the line, before and after the brackets and commas. Spaces may be before and after keyword <span class="tex-font-style-tt">void</span>. The length of each input line does not exceed <span class="tex-span">100</span> characters. The names of variables and procedures are non-empty strings of lowercase English letters and numbers with lengths of not more than <span class="tex-span">10</span> characters. Note that this is the only condition at the names. Only the specified variables are used in procedure calls. The names of the variables are distinct. No two procedures are the same. Two procedures are the same, if they have identical names and identical ordered sets of types of their parameters.</p></div><div class="output-specification"><p>On each of <span class="tex-span"><i>k</i></span> lines print a single number, where the <span class="tex-span"><i>i</i></span>-th number stands for the number of suitable template procedures for the <span class="tex-span"><i>i</i></span>-th call.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of template procedures. The next <span class="tex-span"><i>n</i></span> lines contain the description of the procedures specified in the following format:</p><p>"<span class="tex-font-style-tt">void procedureName (type_1, type_2, ..., type_t)</span>" (<span class="tex-span">1 ≤ <i>t</i> ≤ 5</span>), where <span class="tex-font-style-tt">void</span> is the keyword, <span class="tex-font-style-tt">procedureName</span> is the procedure name, <span class="tex-font-style-tt">type_i</span> is the type of the next parameter. Types of language parameters can be "<span class="tex-font-style-tt">int</span>", "<span class="tex-font-style-tt">string</span>", "<span class="tex-font-style-tt">double</span>", and the keyword "<span class="tex-font-style-tt">T</span>", which denotes the generic type.</p><p>The next line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>) — the number of used variables. Next <span class="tex-span"><i>m</i></span> lines specify the description of the variables in the following format:</p><p>"<span class="tex-font-style-tt">type variableName"</span>, where <span class="tex-font-style-tt">type</span> is the type of variable that can take values "<span class="tex-font-style-tt">int</span>", "<span class="tex-font-style-tt">string</span>", "<span class="tex-font-style-tt">double</span>", <span class="tex-font-style-tt">variableName</span> — the name of the variable.</p><p>The next line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>) — the number of procedure calls. Next <span class="tex-span"><i>k</i></span> lines specify the procedure calls in the following format:</p><p>"<span class="tex-font-style-tt">procedureName (var_1, var_2, ..., var_t)"</span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 5</span>), where <span class="tex-font-style-tt">procedureName</span> is the name of the procedure, <span class="tex-font-style-tt">var_i</span> is the name of a variable.</p><p>The lines describing the variables, template procedures and their calls may contain spaces at the beginning of the line and at the end of the line, before and after the brackets and commas. Spaces may be before and after keyword <span class="tex-font-style-tt">void</span>. The length of each input line does not exceed <span class="tex-span">100</span> characters. The names of variables and procedures are non-empty strings of lowercase English letters and numbers with lengths of not more than <span class="tex-span">10</span> characters. Note that this is the only condition at the names. Only the specified variables are used in procedure calls. The names of the variables are distinct. No two procedures are the same. Two procedures are the same, if they have identical names and identical ordered sets of types of their parameters.</p>

## Output

<p>On each of <span class="tex-span"><i>k</i></span> lines print a single number, where the <span class="tex-span"><i>i</i></span>-th number stands for the number of suitable template procedures for the <span class="tex-span"><i>i</i></span>-th call.</p>





```input1
4
void f(int,T)
void  f(T, T)
 void foo123   ( int,  double,  string,string  ) 
  void  p(T,double)
3
int a
 string    s
double x123 
5
f(a,  a)
  f(s,a   )
foo   (a,s,s)
 f  (  s  ,x123)
proc(a)

```




```input2
6
void f(string,double,int)
void f(int)
   void f  ( T  )
void procedure(int,double)
void f  (T, double,int)   
void f(string, T,T)
4
 int a
 int x
string  t
double  val  
5
f(t, a, a)
f(t,val,a)
f(val,a, val)
 solve300(val, val)
f  (x)

```




```output1
2
1
0
1
0

```




```output2
1
3
0
0
2

```


