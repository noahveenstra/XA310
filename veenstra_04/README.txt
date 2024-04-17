Explain how BOTH algorithms work below, using your own language 
and / or pseudocode as needed...

---

FibonacciRecursive algorithm:
Define a function fibonacciRecursive that takes an integer n as an argument.
If n is less than or equal to 0, return an empty list.
If n is equal to 1, return a list containing a single element 0.
If n is equal to 2, return a list containing two elements: 0 and 1.
If n is greater than 2, do the following:
    Call the fibonacciRecursive function with n - 1 as an argument and assign the returned list to a variable sequence.
    Append the sum of the last two elements of sequence to sequence.
    Return sequence.
Outside the function, prompt the user to enter a number and convert it to an integer. Assign this integer to a variable num.
Call the fibonacciRecursive function with num as an argument and print the returned list.

Pizza algorithm:
Start the function randomPizza.
Initialize an empty string premiumTopping.
Generate a random number between 0 and 1. If this number is greater than 0.5, assign a random premium topping from the pizzaIngredients["premium"] array to premiumTopping.
Log to the console a string "Random Pizza: ", followed by a random selection of cheese, crust, meat, premium topping (if any), sauce, and vegetables. Each ingredient is randomly selected from their respective arrays in the pizzaIngredients object by generating a random index.
End the function.