# Java Code Review Checklist

> When reviewing Java/J2EE code, the reviewer might use the following checklist.

1.	Does the code correctly implement the design?
2.	Is every parameter of every method passing mechanism (value or reference) appropriate?
3.	Does every method return the correct value at every method return point?
4.	Are there any requirements of design that were not implemented? 
5.	Are descriptive variable and constant names used in accord with naming conventions?
6.	Is every variable correctly typed?
7.	Is every variable properly initialized?
8.	Are all for-loop control variables declared in the loop header?
9.	Are there variables that should be constants?
10.	Are there attributes that should be local variables?
11.	Do all attributes have appropriate access modifiers (private, protected, public)?
12.	Are there static attributes that should be non-static or vice-versa?
13.	Are descriptive method names used in accord with naming conventions?
14.	Do all methods have appropriate access modifiers (private, protected, public)?
15.	Is every method parameter value checked before being used?
16.	Are there static methods that should be non-static or vice-versa?
17.	Does each class have an appropriate constructor? 
18.	Do any subclasses have common members that should be in the superclass?
19.	Can the class inheritance hierarchy be simplified?
20.	For every array reference: Is each subscript value within the defined bounds?
21.	For every object or array reference: Is the value certain to be non-null? 
22.	Are there any computations with mixed data types?
23.	Is overflow or underflow possible during a computation?
24.	For each expression with more than one operator: Are the assumptions about order of evaluation and precedence correct?
25.	Are parentheses used to avoid ambiguity?
26.	Does the code systematically prevent rounding errors?
27.	Does the code avoid additions and subtractions on numbers with greatly different magnitudes?
28.	Are divisors tested for zero or noise?
29.	Has each boolean expression been simplified by driving negations inward?
30.	For every boolean test: Is the correct condition checked?
31.	Are there any comparisons between variables of inconsistent types? 
32.	Are the comparison operators correct?
33.	Is each boolean expression correct?
34.	Are there improper and unnoticed side-effects of a comparison? 
35.	Has an "&" inadvertently been interchanged with a "&&" or a "|" for a "||"?
36.	Does the code avoid comparing floating-point numbers for equality?
37. Is every three-way branch (less, equal,greater) covered?
38.	For each loop: Is the best choice of looping constructs used?
39.	Will all loops terminate?
40.	When there are multiple exits from a loop, is each exit necessary and handled properly?
41.	Does each switch statement have a default case?
42.	Are missing switch case break statements correct and marked with a comment?
43.	Is the nesting of loops and branches too deep, and is it correct?
44.	Can any nested if statements be converted into a switch statement?
45.	Are null bodied control structures correct and marked with braces or comments?
46.	Does every method terminate?
47.	Are all exceptions handled appropriately?
48.	Do named break statements send control to the right place?
49.	Have all files been opened before use?
50.	Are the attributes of the open statement consistent with the use of the file?
51.	Have all files been closed after use?
52.	Is buffered data flushed?
53.	Are there spelling or grammatical errors in any text printed or displayed?
54.	Are error conditions checked?
55.	Are files checked for existence before attempting to access them?
56.	Are all I/O exceptions handled in a reasonable way?
57.	Are the number, order, types, and values of parameters in every method call in agreement with the called method's declaration?
58.	Do the values in units agree (e.g., inches versus yards)?
59.	If an object or array is passed, does it get changed, and changed correctly by the called method?
60.	Does every method, class, and file have an appropriate header comment?
61.	Does every attribute,variable or constant declaration have a comment?
62.	Is the underlying behavior of each method and class expressed in plain language?
63.	Is the header comment for each method and class consistent with the behavior of the method or class?
64.	Are all comments consistent with the code?
65.	Do the comments help in understanding the code?
66.	Are there enough comments in the code?
67.	Are there too many comments in the code?
68.	Is a standard indentation and layout format used consistently?
69.	For each method: Is it no more than about 60 lines long?
70.	For each compile module: Is no more than about 600 lines long?
71.	Is there a low level of coupling between modules (methods and classes)?
72.	Is there a high level of cohesion within each module (methods or class)?
73.	Is there repetitive code that could be replaced by a call to a method that provides the behavior of the repetitive code? 
74.	Are the Java class libraries used where and when appropriate?
75.	Are arrays large enough?
76.	Are object and array references set to null once the object or array is no longer needed?
77.	Can better data structures or more efficient algorithms be used?
78.	Are logical tests arranged such that the often successful and inexpensive tests precede the more pensive and less frequently successful tests?
79.	Can the cost of recomputing a value be reduced by computing it once and storing the results?
80.	Is every result that is computed and stored actually used?
81.	Can a computation be moved outside a loop?
82.	Are there tests within a loop that do not need to be done?
83.	Can a short loop be unrolled?
84.	Are there two loops operating on the same data that can be combined into one?
85.	Are frequently used variables declared register?
86.	Are short and commonly called methods declared inline?
87.	Are timeouts or error traps used for external device accesses?
88.	Are there any code implement in inconsistent way?
89.	Are there variables with confusingly similar names?
90.	Are all variables properly defined with meaningful, consistent, and clear names?
91.	Are any modules excessively complex and should be restructured or split into multiple routines?
92.	Are there any redundant or unused variables or attributes?
93.	Could any non-local variables be made local?
94.	Are there any uncalled or unneeded methods?
95.	Can any code be replaced by calls to external reusable objects?
96.	Are there any blocks of repeated code that could be condensed into a single method?
97.	After changing of prototype of method, Have class which calls it considered yet?
98.	Do Upgrading and Migration process follow up changing of structures or contents of a project’s data base?
99.	Is class marked as final, if not being used for inheritance?
100.	Restrict privileges: Is application run with the least privilege mode required for functioning?
101.	Is Input into a system, checked for valid data size and range?
102.	Is excessive logs for unusual behavior avoided?
103.	Is sensitive information from exceptions (exposing file path, internals of the system, configuration) masked?
104.	Highly sensitive information is not logged is ensured? 
105.	Consider purging highly sensitive from memory after use is ensured?
106.	Is prepared statements used instead of dynamic SQL?
107.	Make public static fields final (to avoid caller changing the value)
108.	Exposing constructors of sensitive classes is avoided?
109.	Serialization for security-sensitive classes is avoided?
110.	Sensitive data during serialization is gaurded?
111.	Caching results of potentially privileged operations is avoided?
112.	Is use of JNI restricted?
113.	JUnit tests passed( 100% success) ?
114.	Code coverage is meeting the target range ?
115.	SoapUI tests passed (Functionality validated against Spec with Functional Analyst) ?
116.	No critical error are found in the code (based on Sonar report)
117.	Code is well formatted as per Java standards?
