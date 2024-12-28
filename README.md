# codewars

Create a function that returns the sum of the two lowest positive numbers given an array of minimum 4 positive integers. No floats or non-positive integers will be passed.

For example, when an array is passed like [19, 5, 42, 2, 77], the output should be 7.

function sumTwoSmallestNumbers(numbers) {  
  //Code here
  let orderedNumbers = numbers.sort((a, b)=> a - b)
  
  for(var i = 0; i < orderedNumbers.length; i++) {
    let sum = 0;
    if(i === 0) {
      sum = sum + orderedNumbers[0]
    }
    if(i=== 1){
      sum = sum + orderedNumbers[1]
    }
    return sum
