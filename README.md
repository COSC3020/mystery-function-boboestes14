[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11951599&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```
#it takes an array and checks to see if the length of the array is one, if the array is it returns the only number in the array.
if the array is bigger than one, then it calls itself recursively until it reaches the last number in the array.
then the array checks if the variable foo is bigger than the first value of the initial array.
if foo is bigger then the first value in the array, then it returns foo, else it returns the first value in the array.

#to put it simply it checks the first and last value of an array and returns the bigger variable, if the array is bigger than one.