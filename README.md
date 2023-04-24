# Exercies-JS

Sum Factorial de un Array.

function sumFactorial(arr){
  let nuevoArray = arr.map(num => {
    return factorial(num)
  })
  function factorial(num) {
    if (num === 0 || num === 1)
      return 1;
    for (var i = num - 1; i >= 1; i--) {
      num *= i;
    }
    return num;
  }
  let total = nuevoArray.reduce((accumulator, currentValue) => accumulator + currentValue);
  return total;
}
