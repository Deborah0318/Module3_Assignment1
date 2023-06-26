# Module3_Assignment1
// Function to sort numbers in increasing order
function displayNumbersInIncreasingOrder(numbers) {
  // Sort the numbers in ascending order
  numbers.sort(function(a, b) {
    return a - b;
  });

  // Display the sorted numbers
  console.log("Numbers in increasing order:");
  numbers.forEach(function(number) {
    console.log(number);
  });
}

// Function to prompt the user for input and invoke displayNumbersInIncreasingOrder
function promptAndDisplayNumbers() {
  // Prompt the user for input
  var input = prompt("Enter a set of numbers separated by commas:");

  // Split the input string into an array of numbers
  var numbers = input.split(",").map(function(number) {
    return Number(number.trim());
  });

  // Invoke the displayNumbersInIncreasingOrder function
  displayNumbersInIncreasingOrder(numbers);
}

// Call the promptAndDisplayNumbers function to start the program
promptAndDisplayNumbers();
