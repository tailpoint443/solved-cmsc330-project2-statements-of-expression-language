Download Link: https://assignmentchef.com/product/solved-cmsc330-project2-statements-of-expression-language
<br>
The second project involves completing and extending the C++ program that evaluates statements of an expression language contained in the module 3 case study.

The statements of that expression language consist of an arithmetic expression followed by a list of assignments. Assignments are separated from the expression and each other by commas. A semicolon terminates the expression. The arithmetic expressions are fully parenthesized infix expressions containing integer literals and variables. The valid arithmetic operators are +, –, *, /. Tokens can be separated by any number of spaces. Variable names begin with an alphabetic character, followed by any number of alphanumeric characters. Variable names are case sensitive. This syntax is described by BNF and regular expressions in the case study.

The program reads in the arithmetic expression and encodes the expression as a binary tree. After the expression has been read in, the variable assignments are read in and the variables and their values of the variables are placed into the symbol table. Finally the expression is evaluated recursively.

Your first task is to complete the program provided by providing the three missing classes, Minus, Times and Divide.

Next, you should extend the program so that it supports relational, logical and conditional expression operators as defined by the following extension to the grammar:

&lt;exp&gt; -&gt; ‘(‘ &lt;operand&gt; &lt;op&gt; &lt;operand&gt; ‘)’ |

‘(‘ &lt;operand&gt; ‘:’ &lt;operand&gt; ‘?’ &lt;operand&gt;  ‘)’ |

‘(‘ &lt;operand&gt; ‘!’ ‘)’

&lt;op&gt; -&gt; ‘+’ | ‘-‘ | ‘*’ | ‘/’ | ‘&gt;’ | ‘&lt;‘ | ‘=’ | ‘&amp;’ | ‘|’

Note that there are a few differences in the use of these operators compared to their customary use in the C family of languages. Their differences are:

<ul>

 <li>In the conditional expression operator, the symbols are reversed and the third operand represents the condition. The first operand is the value when true and the second the value when false</li>

 <li>The logical operators use single symbols not double, for example the <em>and</em> operator is &amp; not &amp;&amp;</li>

 <li>The negation operator ! is a postfix operator, not a prefix one</li>

 <li>There are only three relational operators not the usual six and the operator for equality is = not ==</li>

</ul>

Like C and C++, any arithmetic expression can be interpreted as a logical value, taking 0 as false and anything else as true

Your final task is to make the following two modifications to the program:

<ul>

 <li>The program should accept input from a file, allowing for multiple expressions arranged one per line.</li>

 <li>All results should be changed from double to int. In particular the evaluate function should return an int.</li>

</ul>

You may assume that all input to the program is syntactically correct.

<strong>Deliverables: </strong>

Deliverables for this project include the following:

<ol>

 <li>Source code correctly implementing all required functionality. Your program must compile with Microsoft Visual C++ or any modern C/C++ compiler on your O/S.</li>

 <li>Word or PDF file providing screen shots of successfully compiling and executing the program.</li>

 <li>Description of the process and lesson learned while completing this project (to be included in the Word or PDF document).</li>

 <li>A test plan that contains test cases that test all of the required operators. Each test case should include the expression and its expected value (to be included in the Word or PDF document).</li>

</ol>