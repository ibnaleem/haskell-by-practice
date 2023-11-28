# Functions

What makes Haskell a unique language is its requirement of functions; unlike other languages where you can declare variables and classes, Haskell forces you to use pure functions that must return a value to compile. We will explore exercises related to the I/O paradigm in Haskell in the I/O Chapter. For now, complete the following exercises.

> We have simplified exercises by creating template files. Click here to use a template file to follow along with this exercise. *Learn More*

## Exercise 1:
Write a function that adds two to its argument.
```haskell
add_two :: Int -> Int
add_two x = ?
```

## Exercise 2:
Complete this function that should return the double of its argument:
```haskell
double_me :: Int -> Int
double_me x = ?
```
> There are **2** solutions to this exercise.

## Exercise 3:
Write a function `add_squares` that takes 2 arguments `x` and `y`, squares them, then adds them together.

```haskell
add_squares :: Int -> Int -> Int
add_squares x y = ?
```

## Exercise 4:
Write a function `max_three` that takes 3 arguments `x`, `y` and `z`; the purpose of this function is to find the maximum value between 3 arguments. For example:
```
ghci> max_three 1 2 3
3
```
> Moving forward, you will not be given the boilerplate; you will write the functions in Haskell syntax yourself. The only time boilerplate will be given is when you're tasked to debug code.

## Exercise 5:
Write a function `pow3` with one argument `x` that returns 3 to the power `x`

## Exercise 6:
Write a function `all_equal` with three arguments `x`, `y` and
`z` that returns `True` if `x` is equal to `y` and `y` is equal to `z`.
> ❌  You are not allowed to use `if` expressions.

## Exercise 7:
Write a function `minplus` with four arguments `a`, `b`, `c` and `d` that computes the sum of the minimums between a, b and c, d. For example, `minplus` should compute the sum of 1 and 3 since 1 and 3 are the minimum from the given arguments 1,2,3,4.
```
ghci> minplus 1 2 3 4
4
```

## Exercise 8:
Write a function minFour with four arguments `a`, `b`, `c` and `d` that returns the minimum of its four arguments. Examples:
```
ghci> minFour 1 2 3 4
1
ghci> minFour 33 66 99 100
33
```

## Exercise 9:
To convert a two-bit binary number (represented as \\( \mathrm{bin} \\)) to decimal:

\\[ \mathrm{bin\} = b_{1} \cdot 2^1 + b_{2} \cdot 2^0 \\]

Thus, 11 in binary becomes 1 × 2 + 1 = 3

Write a function `pow2` that raises 2 to its argument `x`. For example:
```
ghci> pow2 5
32
```
Additionally, create another function `bin_to_dec` that takes 2 arguments `b1` `b2` and uses the formula above to calculate \\( \mathrm{bin} \\)

> 💡 You will need to use `pow2` to sum up `b1` and `b2`. Remember that the formula states `b1` must multiply by 2¹, and `b2` by 2⁰, then they are both summed up.

## Exercise 9.5:
Modify `bin_to_dec` function such that it can convert 4 bit binary numbers.

## Exercise 10:
Write a function `quad` that computes the quadratic formula on 3 of its arguments `a`, `b` and `c`.

\\[ x = \frac{{-b + \sqrt{b^2 - 4ac}}}{{2a}} \\]

Examples:
```
ghci> quad 1 16 0
0
ghci> quad 1 -2 1
1.0
```
For your convinience, we have changed \\( \pm \\) to \\( + \\) in \\( -b \pm \sqrt{b^2 - 4ac} \\)