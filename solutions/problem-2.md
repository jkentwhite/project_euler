# Problem 2: Even Fibonacci Numbers

Each new term in the Fibonacci sequence is generated by adding the previous two terms. By starting with 1 and 2, the first 10 terms will be:

1, 2, 3, 5, 8, 13, 21, 34, 55, 89, ...
By considering the terms in the Fibonacci sequence whose values do not exceed n, find the sum of the even-valued terms.

Solution:

```
let sum = 0, prevnum = 1, nextnum = 2;
while(nextnum <= n){

  if(nextnum%2 === 0){
    sum += nextnum;
  }

  nextnum = prevnum + nextnum;
  prevnum = nextnum - prevnum;
}

return sum;
```
