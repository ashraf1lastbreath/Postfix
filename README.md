# Algorithm for Conversion Of An Expression From Infix to Postfix

> 1.  In this Algorithm we are reading token from Left to Right and Postfix expression is generated 
> 2. So Entered Token may be –
- Alphabet from A-Z or a-Z
- Numerical Digit from 0-9
- Operator
- Opening And Closing Braces ( or )
> 3. If Entered Character is Alphabet then Following Action Should be taken-
-       Print Alphabet as Output
> 4. If Entered Character is Digit then Following Action Should be taken-
-       Print Digit as Output
> 5. If Entered Character is Opening Bracket then Following Action Should be taken-
-       Push ‘(‘ Onto Stack
- If any Operator Appears before ‘ ) ’ then 

-       Push it onto Stack.
-   If Corresponding ‘)’ bracket appears then Start Removing Elements
-        [Pop] from Stack till ‘(‘ is removed.
> 6. If Entered Character is Operator then Following Action Should be taken-
- Check Whether There is any Operator Already present in Stack or not.
- If Stack is Empty then :
-       Push Operator Onto Stack.
- If Present then :
-       Check Whether Priority of Incoming Operator is greater than Priority of Topmost Stack Operator.
- If Priority of Incoming Operator is Greater then :
-       Push Incoming Operator Onto Stack.
- Else :
-       Pop Operator From Stack again goto Step 6.


# Algorithm for Evaluation of a Postfix Expression :
> 1.  Initialize empty stack
> 2.  For every token in the postfix expression (scanned from left to right):
>> -    If the token is an operand (number) :
-       push it on the stack
- Otherwise, if the token is an operator (or function):

-       Check if the stack contains sufficient number of values (usually two) for given operator
- If there are not enough values, finish the algorithm with an error
- If sufficient number of values (operands) are present :
-       Pop the appropriate number of values (usually two) from the stack
-       Evaluate the operator using the popped values and
-       push the single result on the stack
- If the stack contains only one value :
-       return it as a final result of the calculation
-  Otherwise, finish the algorithm with an error


License
----

Ashraf


**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
