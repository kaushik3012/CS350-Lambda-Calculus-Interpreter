# Lambda Calculus Interpreter

This is a project for the course *CS350A: Principles of Programming Languages*<br>
*Requires Haskell to run*
<br>

## Usage
To start the interpreter run the code using *runhaskell* or *ghc* :
> \> runhaskell lci.hs 
<br>

## Features

The interpreter supports the following features :
+ Identifying whether the expression entered is a λ-term
+ Printing the free variables
+ substitute a λ-term replacing all free occurrences of a variable
in another λ-term
+ Applying the Beta-reduction rule and converting it to the normal form

## Example <br>
> \> "(\\x.\\y.x)" <br>
Free Variables in (\x.\y.x): []<br>
Normal form of (\x.\y.x): <br>
\x.\y.x <br>
\> "(\\x.\\y.x)(\\x.x)" <br>
Free Variables in (\x.\y.x)(\x.x): []<br>
Normal form of (\x.\y.x)(\x.x): <br>
\b.\x.x
<br>
\> "(\\x.x)a"<br>
Free Variables in (\x.x)a: ["a"] <br>
Normal form of (\x.x)a: <br>
a

## Team Members
+ Kaushik Raj V Nadar (200499)
+ Lakshmi Pravallika (200282)
