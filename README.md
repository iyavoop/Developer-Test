# Limesharp test

Fork this repo, commit changes after each task and send us the link to your repo (don't do a Pull Request, just send us the link).
We will get back to you shortly. 
Languages accepted: Javascript or PHP. 

### Task 1: 
Make this work (repeat 3 times the contents of an array):

```javascript
repeat([1,2,3]) //[1,2,3,1,2,3,1,2,3]

Your solution:
```
function repeat(arr){

  var temp = []

  for(var i=0; i<3; i++){
      temp.push(arr);
  }    
  
  return temp;
}

###### if we type in our console your function and repeat([1,2,3]) then the result should be [1,2,3,1,2,3,1,2,3] 

### Task 2:
Make this work (no vowels, lowercase except the first letter):
```javascript
reformat("liMeSHArp DeveLoper TEST") //Lmshrp dvlpr tst

Your solution:
```
function reformat(text){

  var reformatted_text = "";
  
  reformatted_text = text.toLowerCase();
  reformatted_text = reformatted_text.charAt(0).toUpperCase() + reformatted_text.slice(1);
  
  for(var i; i<reformatted_text.length; i++){
  
    switch(reformatted_text.charAt(i)){
      case 'a':
      case 'e':
      case 'i':
      case 'o':
      case 'u':
        reformatted_text = reformatted_text.slice(0,i-1) + reformatted_text.slice(i+1)
        break;
         
    }
  }
  
  return reformatted_text;
}

###### if we type in our console your function and reformat("liMeSHArp DeveLoper TEST") then the result should be Lmshrp dvlpr tst


### Task 3 (optional, for bonus points):
Make this work (without using any built in functions, only a `for` loop, return the next binary number in a string or as an array)
```javascript
next_binary_number([1,0]) // [1,1]

// possible test cases:
// [1,0] => [1,1]
// [1,1] => [1,0,0]
// [1,1,0] => [1,1,1]
// .......
// [1,0,0,0,0,0,0,0,0,1] => [1,0,0,0,0,0,0,0,1,0]
```
Your solution:

###### if we type in our console your function and next_binary_number([1,0,0,0,0,0,0,0,0,1]) then the result should look like 1,0,0,0,0,0,0,0,1,0 (or as an array).

###### If you get invited to the first interview read the What to expect.md file.
