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
if the array is bigger than one, then it calls itself recursively until it reaches the last number in the array, where it sets the variable foo equal to it. then the array checks if the variable foo is bigger than the next number in the array. it does this until it gets the biggest number in the array, and then returns that.

# to put it simply it checks the all the elements in the array and returns the biggest one.