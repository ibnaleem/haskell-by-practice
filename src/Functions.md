# Functions

What makes Haskell a unique language is its requirement of functions; unlike other languages where you can declare variables and classes, Haskell forces you to use pure functions that must return a value to compile. We will explore exercises related to the I/O paradigm in Haskell in the I/O Chapter. For now, complete the following exercises.

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
```ghci> max_three 1 2 3
3
```
> Moving forward, you will not be given the boilerplate; you will write the functions in Haskell syntax yourself. The only time boilerplate will be given is when you're tasked to debug code.

## Exercise 5:
To convert a two-bit binary number (represented as \mathrm{bin_to_dec}) b_{1}b_{2} to decimal:
    \mathrm{bin_to_dec} = b_{1} ∗ 2^1 + b_{2} ∗ 2^0
Thus, 11 in binary becomes 1 × 2 + 1 = 3

Write a function `pow2` that raises 2 to its argument `x`. For example:
```ghci> pow2 5
32
```
Additionally, create another function `bin_to_dec` that takes 2 arguments `b1` `b2` and uses the formula above to calculate \mathrm{bin_to_dec}

> 💡 You will need to use `pow2` to sum up `b1` and `b2`. Remember that the formula states `b1` must multiply by 2^1, and `b2` by 2^0, then they are both summed up.