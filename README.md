# Exericios-Eloquent-Javascript

## Looping a triangle
Write a loop that makes seven calls to console.log to output the following triangle:

\#

\##

\###

\####

\#####

\######

#######

```javascript
let count = 0;
let hashtag = "#";

while(count < 7){
  console.log(hashtag);
  hashtag += "#";
  count += 1;
}
```

## FizzBuzz

Write a program that uses console.log to print all the numbers from 1 to 100, with two exceptions. For numbers divisible by 3, print "Fizz" instead of the number, and for numbers divisible by 5 (and not 3), print "Buzz" instead.

When you have that working, modify your program to print "FizzBuzz" for numbers that are divisible by both 3 and 5 (and still print "Fizz" or "Buzz" for numbers divisible by only one of those).

(This is actually an interview question that has been claimed to weed out a significant percentage of programmer candidates. So if you solved it, your labor market value just went up.)

```Javascript
count = 0;

while (count <= 100){
  if ((count % 3 === 0) && (count % 5 === 0)){ 
  	console.log("FizzFuzz");
    count += 1;
    continue;
  }
  if (count % 3 === 0){
    console.log("Fizz")
    count += 1;
    continue;
  }
  if (count % 5 === 0){
    console.log("fuzz")
    count += 1;
    continue;
  }
  console.log(count);
  count += 1;
}
```



## Chessboard







```Javascript
// Versão simplificada somente com alteração na altura do tabueiro
let size = prompt("quantas linhas voce quer no tabuleiro?");
let count = 0;
let tabuleiro = " # # # #\n";
while(count <= size){
  if (count % 2 === 0){
    tabuleiro += "# # # # \n";
  }
  if (count % 2 !== 0){
    tabuleiro += " # # # #\n";
  }
  count += 1;	 
}

console.log(tabuleiro);
```


## MINIMUM

The previous chapter introduced the standard function Math.min that returns its smallest argument. We can build something like that now. Write a function min that takes two arguments and returns their minimum.

```javascript
const f = function(a,b){
  if (a<b){
  	return console.log(a);
  }else{
  	return console.log(b);
  }
}  
```

## Recursion

We’ve seen that % (the remainder operator) can be used to test whether a number is even or odd by using % 2 to see whether it’s divisible by two. Here’s another way to define whether a positive whole number is even or odd:

Zero is even.

One is odd.

For any other number N, its evenness is the same as N - 2.

Define a recursive function isEven corresponding to this description. The function should accept a single parameter (a positive, whole number) and return a Boolean.

Test it on 50 and 75. See how it behaves on -1. Why? Can you think of a way to fix this?

```javascript
function isEven (a){
	if (a % 2 === 0) {
    	return true;
    }else{
    	return false;
    }
}
```

