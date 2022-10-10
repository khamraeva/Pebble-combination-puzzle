function findCombination(multipliedSum = 24, totalSum = 22) {
  const options = Array.from(Array(10).keys());
  const result = [];
  
  options.forEach(firstNumber => {
    const combination = [];
    
    options.forEach(secondNumber => {
      if (firstNumber * secondNumber === multipliedSum && !(secondNumber % 2)) {
        const fourthNumber = secondNumber/2;
        
        options.forEach(thirdNumber => {
          options.forEach(fifthNumber => {
            if (firstNumber + secondNumber + thirdNumber + fourthNumber + fifthNumber === totalSum
              && firstNumber + thirdNumber === fourthNumber + fifthNumber) {
              combination.push(firstNumber, secondNumber, thirdNumber, fourthNumber, fifthNumber)
            }
          });
        });
        
      }
    });
    combination.length && result.push(combination);
  });
  return result;
}

findCombination();
