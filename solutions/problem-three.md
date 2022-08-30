# Problem 3: Largest prime factor

The prime factors of 13195 are 5, 7, 13 and 29.

What is the largest prime factor of the given number?

Solution:

```let max = 1, prime = 2;

while(prime <= number){
    if(number%prime === 0){
        max = prime;
        number = number/prime;
    } else prime++;
}
return max;
```
