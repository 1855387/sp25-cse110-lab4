2.1 At line 12, 3 will be printed. i is declared using var meaning it is not constrained to block scope and can be printed after and outside of the block it was declared in as long as it is within the function, in this case, after iteration i is 3.
2.2 At line 13, the last caculated discountedPrice would be printed. Again, since var was used, this variable can be accessed anywhere within the scope of the function after it is defined. It's the last calculated discountedPrice as it keeps getting redefined each iteratigve loop. In the final case it is defined as 300 * 1-0.5 giving us 150.
2.3 Again var allows finalPrice to be printed anywhere within functions scope after being defined (let wouldn't lead to issues either in this case). At each iteration finalPrice gets redefined and since the print is after the looping it will print the last calculated finalPrice. In this case, it would be 150 as there is no rounding to be done. 150*100 = 15000 / 100 = 150.
2.4 This function returns an array with the i-th index of the array representing the rounded dicounted price of the i-th index price in the original array. So in our example, discounted looks like [50,100,150].
2.5 An error will occur because let means that i is only defined within the scope of the block, not the function, so calls outside the block will register i to be undefined.
2.6 The same logic in 2.5 applies here as well. Using let makes the variable only be accessable within the scope of its block, the print statement is outside of the scope so it will register as undefined.
2.7 150 is printed at line 14. There is no error because the block that finalPrice is defined within is the scope of the function, so calls outside of the loop where it is being redefined can still access the variable. It is able to retrieve this last computed final value of 150 and print it.
2.8 This function still returns the same thing as 2.4. There is no functional difference other than the ability to print certain variables due to using let instead of var.
2.9 Again, the same issue occurs and the reasoning follows 2.5. "An error will occur because let means that i is only defined within the scope of the block, not the function, so calls outside the block will register i to be undefined."
2.10 3 will be printed. length is a constant variable set to the length of the prices array. In this case that value is 3, nothing else cahnges with this varaible so 3 is printed.
2.11 This function returns the same value as outlined in 2.4. The only distinction is that no rounding occurs before pushing the prices in our current implementation, but this has no effect on the output produced by our function with the test case provided.
2.12A student.name
2.12B student['Grad Year']
2.12C student.greeting()
2.12D student['Favorite Teacher'].name
2.12E student.courseLoad[0]
2.13A 32, converts 2 to a string and concatenates the two strings
2.13B 1, '3' converted to number and performs subtration 3-2=1
2.13C 3, null converted to 0 when used with number so 3 is produced
2.13D 3null, + with a string makes null become a string and the two get concatenated
2.13E 4 true + 3, true becomes 1 and added to make 4
2.13F 0 false and null both converted to 0, yielding 0
2.13G 3undefined, '3' + undefined made undefined a string and concatenated the two
2.13H NaN, - converts '3' to 3 and undefined to NaN, 3-NaN yields NaN

2.14A true, 2 converted to a number and it is greater than 1
2.14B false, goes by character order in string, '2' > '1' (the 1 in '12') hence false
2.14C true, loose equality '2' goes to 2 and they're equivalent
2.14D false, 2 is a number '2' is a string, checks tyopes and types are not the same, returns false
2.14E false, true becomes 1, 1 != 2, false
2.14F true, Boolean(2) just is true, true === true both in type and value

2.15 == allows for type coercion to occur in which values are attempted to be converted to comparable types if they are not comparable and then be compared whereas === checks that the value AND the type are equivalent.

2.16 code within the part2-question16.js file

2.17 The result is [ 2, 4, 6 ]. the doSomething function doubles the value of the parameter passed to it and returns that value. In modify array, it is iterating through each of the indices and doubling that value and pushing it into a new array to be returned to the user. So the returned value when passing in the specificed parameters yield the array [ 2, 4, 6 ] from [1,2,3]

2.18 code within the part2-question18.js file

2.19 1 4 3 2. It prints the non time out logs first so 1 and 4 anfd then 3 next cause it had a timeout of 0 and finally 2 since it had a timeout of 1 second.