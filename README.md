# udacity
lesson 13 front end development
WHILE LOOPS

Directions:
Write a while loop that:

1. Loop through the numbers 1 to 20
If the number is divisible by 3, print "Julia"
If the number is divisible by 5, print "James"
If the number is divisible by 3 and 5, print "JuliaJames"
If the number is not divisible by 3 or 5, print the number

SOLUTION 

/*
 * Programming Quiz: JuliaJames (4-1)
 */

var x = 1;
while (x <= 20) {
    if (x % 3 === 0 && x % 5 === 0) {
        console.log ("JuliaJames");
    }
    else if (x % 3 === 0 ) { console.log("Julia");} 
    else if (x % 5===0) { console.log("James");}
    else {
        console.log(x);
    }
    x=x+1;
    
                
                
    // print Julia, James, or JuliaJames
    // increment x
}

2.
99 bottles of juice on the wall! 99 bottles of juice! Take one down, pass it around... 98 bottles of juice on the wall!
98 bottles of juice on the wall! 98 bottles of juice! Take one down, pass it around... 97 bottles of juice on the wall!
...
2 bottles of juice on the wall! 2 bottles of juice! Take one down, pass it around... 1 bottle of juice on the wall!
1 bottle of juice on the wall! 1 bottle of juice! Take one down, pass it around... 0 bottles of juice on the wall!

SOLUTION
/*
 * Programming Quiz: 99 Bottles of Juice (4-2)
 *
 * Use the following `while` loop to write out the song "99 bottles of juice".
 * Log the your lyrics to the console.
 *
 * Note
 *   - Each line of the lyrics needs to be logged to the same line.
 *   - The pluralization of the word "bottle" changes from "2 bottles" to "1 bottle" to "0 bottles".
 */

var num = 99;

while (num >= 1){
    if (num > 2){
    console.log(num +" bottles of juice on the wall! " + num +" bottles of juice! Take one down, pass it around... "+(num -1) + " bottles of juice on the wall!");
    }else if(num === 2) {
        console.log(num +" bottles of juice on the wall! "+num +" bottles of juice! Take one down, pass it around... "+(num -1) + " bottle of juice on the wall!");
    }else {
        console.log(num +" bottle of juice on the wall! "+num +" bottle of juice! Take one down, pass it around... "+(num -1) + " bottles of juice on the wall!");
    }
    num = num - 1;
}

    // check value of num
    // print lyrics using num
    // don't forget to check pluralization on the last line!
    // decrement num

3. T-60 seconds
T-59 seconds
T-58 seconds
...
T-51 seconds
Orbiter transfers from ground to internal power
T-49 seconds
...
T-3 seconds
T-2 seconds
T-1 seconds
Solid rocket booster ignition and liftoff!

SOLUTION:- 
var seconds = 60;
while(seconds >= 0) {
	if(seconds === 50) {
		console.log("Orbiter transfers from ground to internal power")
	} else if (seconds === 31) {
		console.log("Ground launch sequencer is go for auto sequence start");
	} else if(seconds === 16) {
		console.log("Activate launch pad sound suppression system")
	} else if(seconds === 10) {
		console.log("Activate main engine hydrogen burnoff system");
	} else if(seconds === 6) {
		console.log("Main engine start");
	} else if(seconds === 0) {
		console.log("Solid rocket booster ignition and liftoff!");
	} else {
		console.log("T-" + seconds + " seconds")
	}
	
	seconds = seconds - 1;
}
	
FOR LOOP
Rewrite the following while loop as a for loop:

var x = 9;
while (x >= 1) {
  console.log("hello " + x);
  x = x - 1;
}
Solution 

// rewrite the while loop as a for loop
for (var x = 9; x >= 1 ; --x) {
    console.log("hello " + x);

}

Here is a for loop that's supposed to print the numbers 5 through 9. Fix the error!

for (x < 10; x++) {
  console.log(x);
}

solution
// fix the for loop
for (var x =5; x < 10; x++) {
    console.log(x);
}

he for loop below has an error. Fix it!

for (var k = 0 k < 200 k++) {
  console.log(k);
}
SOLUTION
// fix the for loop
for (var k = 0; k < 200; k++) {
    console.log(k);
}

Write a for loop that prints out the factorial of the number 12:

A factorial is calculated by multiplying a number by all the numbers below it. For instance, 3! or "3 factorial" is 3 * 2 * 1 = 6

3! = 3 * 2 * 1 = 6 3!=3∗2∗1=6
4! = 4 * 3 * 2 * 1 = 24 4!=4∗3∗2∗1=24
5! = 5 * 4 * 3 * 2 * 1 = 120 5!=5∗4∗3∗2∗1=120

Save your final answer in a variable called solution and print it to the console

solution :- 
// your code goes here

var solution = 1;
for(var x = 12; x > 0; x--){
    solution *=x;
    
}
console.log(solution);

Theater seats often display a row and seat number to help theatergoers find their seats. If there are 26 rows (0 to 25) and 100 seats (0 to 99) in each row, write a nested for loop to print out all of the different seat combinations in the theater.

Example output for row-seat information: output each row and seat number on a separate line

0-0
0-1
0-2
...
25-97
25-98
25-99

solution :- 
 Write a nested for loop to print out all of the different seat combinations in the theater.
 * The first row-seat combination should be 0-0 
 * The last row-seat combination will be 25-99
 * 
 * Things to note: 
 
 *  - the row and seat numbers start at 0, not 1
 *  - the highest seat number is 99, not 100
 */

// Write your code here

for (var x =0; x <= 25 ; x++) { 
    for ( var y =0; y <= 99; y++) {
        console.log(x + "-" + y);
        
    }
    
}

