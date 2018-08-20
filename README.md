# Limesharp test

Fork this repo, commit changes after each task and send us the link to your repo (don't do a Pull Request, just send us the link).
We will get back to you shortly. 
Languages accepted: Javascript or PHP. 

### Task 1: 

```javascript
//repeat([1,2,3]) //[1,2,3,1,2,3,1,2,3]

//Your solution:

function repeat(arr){

  var temp = []

  for(var i=0; i<3; i++){
      temp.push(...arr);
  }    
  
  return temp;
}
```

### Task 2:

```javascript

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
```



### Task 3 (optional, for bonus points):

```javascript

function next_binary_number(arr){

  var temp = [];
  var decimal_number = 0;
  
  for(var i=0; i<arr.length-1; i++){
      
      decimal_number += (2 ** (arr.length-1-i)) * arr[i];
  
  }
  
  decimal_number++;
      
  quotient = decimal_number;
  
  
  while(quotient > 0){
     
      remainder = decimal_number % 2;
      
      temp.push(remainder) 
      
      quotient = decimal_number / 2;
  
  }

  return temp;

}


```



