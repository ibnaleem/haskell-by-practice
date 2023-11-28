# Ifs and Lets
Programs will require conditions, or else they will run into errors or not produce the result we are aiming for. This section covers exercises related to `if` and `let` expressions in Haskell.

> We have simplified exercises by creating template files. Click here to use a template file to follow along with this exercise. *Learn More*

## Exercise 1: If Expressions
Write a function `gt10` that takes an argument `x` that returns `"yes"` if `x` is greater than 10, otherwise it returns `"no"`
```
ghci> gt10 9
"no"
ghci> 11
"yes" 
```

## Exercise 2: If Expressions
What is wrong with the following code?:
```haskell
gt10 x = if x > 10 then 1 else "no"
```
```
<interactive>:3:25: error:
    • Could not deduce (Num String) arising from the literal ‘1’
      from the context: (Ord a, Num a)
        bound by the inferred type of gt10 :: (Ord a, Num a) => a -> String
        at <interactive>:3:1-35
    • In the expression: 1
      In the expression: if x > 10 then 1 else "no"
      In an equation for ‘gt10’: gt10 x = if x > 10 then 1 else "no"
```

## Exercise 3: If Expressions
Write a function `computeExpression` that takes two arguments `a` and `b`, and returns `(a + 12)` if \\( a > 10 \) and \\( b < 20 \), otherwise it returns the minimum of `a` and `b`.
```
ghci> computeExpression 12 2
24
ghci> computeExpression 12 20
12
ghci> computeExpression 12 12
12
ghci> computeExpression 14 19
26
```

## Exercise 4: If Expressions
Create a function `mixedOperation` that takes two arguments, `a` and `b`. If \\( a \neq b \), the function should return \\( a \) if \\( a = 1 \) and \\( b \) otherwise. If \\( a = b \), the function should return 0.
```
ghci> mixedOperation 10 10
0
ghci> mixedOperation 10 12
12
ghci> mixedOperation 1 12
1
```

## Exercise 5: If Expressions
What will the following expressions evaluate?
```haskell
if (1 == 1 && 2 /= 3 && 3 < 4) then 1 else 0

if 1 > 0 then (if 1+1 /= 2 then 4 else 2) else 1

if (if True then False else True) then "Which" else "One?"
```
> 💡 Try to break down the expressions by precedence to solve this exercise.

## Exercise 6: Let Expressions
Take the following expression and convert it into a `let` expression:
```haskell
(x * x - 4) + sqrt (x * x - 4)
let s = ?
```

## Exercise 7: Let Expressions
Write a `let` expression that take bindings `a` and `b` and sum them up

## Exercise 8: Let Expressions
The following expression throws an error:
```haskell
func x = let a = x * x; a = a + 1 in a
```
```
```
<interactive>:4:5: error:
    Conflicting definitions for ‘a’
    Bound at: <interactive>:4:5
              <interactive>:4:16
```
Fix the `let` such that no errors persist.
```
ghci> func 5
26
```

## Exercise 9: Let Expressions
Bindings `a` and `b` are set to 1 and 2 (in that order) and calling the max function on them will return 2.
```ghci> max a b
2
```
Write `let` expressions (in GHCi) and call the max function on them like shown above.