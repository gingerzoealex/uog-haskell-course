https://www.futurelearn.com/courses/functional-programming-haskell/6/steps/605834
_____

### Assigning expressions to variables


Python - `def hello(name):
						return "Hello, "+name
`


haskell - `hello name = "Hello, "++name`

### all functionality is based on expressions.
Expression will evaluate to a result. 
e --> r
uses the same maths as other languages, ie BODMAS. Don't be a dick and forget that again. 

- Call functions in expressions
in an expression, call a function with an argument. Do stuff with the argument within the function & returns the result.
Seeems similar to what a generator would be in Python??

- If an expression is being used as an argument, put it in parens. Precedence & shite.

- assign a name to an equation like in any other language. basically declares a constant (doesn't change value, so the name can only be used once)

"This is part of the meaning of “pure” and “no side effects”


`n = n + 1` or `n := n + 1` ==> recursion. This assigns the value of n + 1 to n. Wtff.


___


## Functions

abs  - absolute value
min
max

___


## Good practice notes
Parens (bodmas?)
___





Types

C has types, for example:

    int f (int x, int y) {
        return x*y+x+y;
    }

Haskell has much more powerful types than C, and we will talk a lot about types:

    f :: Int -> Int -> Int
    f x y =  x*y+x+y

Lists

In many languages, e.g. Python, JavaScript, Ruby, … you can create lists such as:

    lst = [ "A", "list", "of", "strings"]

Haskell also uses this syntax for lists.

To join lists, in Python you could write

    lst = [1,2] + [3,4]

In Haskell this would be very similar:

    lst = [1,2] ++ [3,4]

Anonymous functions

In JavaScript you can define anonymous functions (functions without a name) such as:

    var f = function(x,y){return x*y+x+y};

In Haskell, such anonymous functions are called lambda functions and they are actually the basis of the language. Again, the syntax is very compact:

    f = \x y -> x*y+x+y

Higher-order functions

Finally, in many languages, functions can operate on functions. For example, in Perl you can modify the elements in a list using:

    map sub ($x){$x*2+1}, [1..10]

Haskell provides many of these so-called higher-order functions, and lets you define your own.

    map (\x -> x*2+1) [1..10]

