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
	
