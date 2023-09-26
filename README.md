[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11756533&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) { // input is an array
    if(a.length == 1) return a[0];  // if the length of the array is 1, return with the first element of the array
    var foo = mystery(a.slice(1, a.length)) // creates a new array without the first element, then recursively calls that new array
    // foo will equal the last element of the original array
    if(foo > a[0]) return foo; // if the final element is greater then the first, return the final
    else return a[0]; // else return the first element
}
```
The mystery function compares the first and the last element of an array, and returns the greater    

reference - used this link to figure out what slice did - https://www.w3schools.com/jsref/jsref_slice_array.asp