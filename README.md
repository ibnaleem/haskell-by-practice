<div align="center">
    <img src="https://upload.wikimedia.org/wikipedia/en/thumb/4/4d/Logo_of_the_Haskell_programming_language.svg/2560px-Logo_of_the_Haskell_programming_language.svg.png">
</div>
    
<p align="center">Practice Haskell with challenging examples, exercises and projects</p>
    
<div align="center">

<a href="https://github.com/ibnaleem/haskell-by-practice/stargazers"><img src="https://img.shields.io/github/stars/ibnaleem/haskell-by-practice.svg?style=for-the-badge"></a>
<a href="https://github.com/ibnaleem/haskell-by-practice/blob/main/LICENSE"><img src="https://img.shields.io/github/license/ibnaleem/haskell-by-practice?style=for-the-badge"></a>
</div>

This book is inspired by [Rust By Practice](https://github.com/sunface/rust-by-practice). The best way to learn any language is by using it; learn functional programming with hands-on exercises and guidance on projects to start your functional programming journey. Theoretical knowledge and concepts will be derived from [Haskell-Simplified](https://github.com/ibnaleem/Haskell-Simplified).

## Reading online

- [Haskell By Practice](https://github.ibnaleem.io/haskell-by-practice) (*currently reading*)
- [Haskell-Simplified (theorectical concepts)](https://ibnaleem.github.io/Haskell-Simplified/)

## Structure

- Each chapter contains examples, exercises and practices

- Compilation errors and GHCi troubleshooting will be covered at the end of each chapter

- Every exercise has its own solutions, which are posted in /Solutions

- Each chapter increases difficulty

## Example Exercises

### Exercise 1:
We have defined a function named `append_char` that takes an argument `char` and appends it to a string. The following should be the result in `ghci>`:
```
ghci> appended_char 'h'
"Appended char: h"
```
Below is the function defined, but it does not compile, leading to an error. Fix the defined function so it can compile and run without errors:
```haskell
appended_char :: Char -> [Char] -- ignore this
appended_char char = "Appended char: " ++ char
```

### Exercise 2:
Use recursion to rewrite the following function:
```haskell
-- Factorial function without recursion
factorial :: Integer -> Integer
factorial n = product [1..n]
```
```haskell
-- Factorial function with recursion
factorial :: Integer -> Integer
factorial n = ?
```

## Contributing
I welcome contributions from the community and appreciate the time and effort put into making [Haskell By Practice](https://ibnaleem.github.io/haskell-by-practice) better. To contribute, please follow the guidelines and steps outlined below:

> Note: **_Your pull request will be closed if you do not specify the changes you've made._**

### Fork the Repository
Start by [forking this repository](https://github.com/ibnaleem/haskell-by-practice/fork). You can do this by clicking on the ["Fork"](https://github.com/ibnaleem/haskell-by-practice/fork) button located at the top right corner of the GitHub page. This will create a personal copy of the repository under your own GitHub account.

### Clone the Repository
Next, clone the forked repository to your local machine using the following command:
```bash
$ git clone https://github.com/yourusername/haskell-by-practice.git
```
Navigate to the cloned directory:
```bash 
$ cd haskell-by-practice
```
### Create a New Branch
Before making any changes, it's recommended to create a new branch. This ensures that your changes won't interfere with other contributions and keeps the main branch clean. Use the following command to create and switch to a new branch:
```bash
$ git checkout -b branch-name
```
### Make the Desired Changes
Now, you can proceed to make your desired changes to the project. Whether it's fixing grammer mistakes, adding new material to chapters, improving documentation, or optimizing exercises, your efforts will be instrumental in enhancing the project.

### Commit and Push Changes
Once you have made the necessary changes, commit your work using the following commands:
```bash
$ git add .
$ git commit -m "Your commit message"
```
Push the changes to your forked repository:
```bash
$ git push origin branch-name
```
### Submit a Pull Request
Head over to the [original repository](https://github.com/ibnaleem/haskell-by-practice) on GitHub and go to the ["Pull requests"](https://github.com/ibnaleem/haskell-by-practice/pulls) tab.
1. Click on the "New pull request" button.
2. Select your forked repository and the branch containing your changes.
3. Provide a clear and informative title for your pull request, and use the description box to explain the modifications you have made. **_Your pull request will be closed if you do not specify the changes you've made._**
4. Finally, click on the "Create pull request" button to submit your changes.
