# calclang
Calc-Lang is a simple calculator language. (each line is interpreted)

Calc-Lang has the notion of Variables, and inbuilt functions. The names of the
inbuilt functions cannot be used for variable names.

Some examples of the syntax could be:

    $ ./calculator.py
    >>> x = sin(3.1415)
    >>> 12 + 3**3
    39
    >>> 12 + max(3,2,4)
    16
    >>> 12 % 5
    2
    >>> 4**.5
    2
    >>> max(sin(3), sin(4), sin(5))
    0.1411200080598672
    >>> 

Operators supported:

+   addition
-   subtration
*   multiplication
/   division
%   remainder
**  power (supports fraction power too)
=   Assignment (all varables are of type 'number' i.e. float)

Convenience operators are
+=
-=
*=
/=
%=
**=


Underscore is a special variable that stores the value of the last expression,
but not when there is an explicit assignment.

Semicolon at the end of the statments is optional, but when multiple statments 
are present, semicolon has to be used.

Note that, 'var = expr' is not an expression. So usage like,

>>> max(x=sin(3), y=sin(5))

are not allowed.



Inbuilt fuctions names (hence reserved names) and values:

int(number)     //truncates the fractional part of the number
abs(number)     //absolute value
ceil(number)    //ceiling
floor(number)   //floor
round(number,int(number))   //round the value to int(number) digits
sin(number)
cos(number)
tan(number)

