1. Prime number generation

A prime Number is a whole number greater than 1, which is only divisible by 1 and itself. First few prime numbers are : 2 3 5 7 11 13 17 19 23 …..

Some interesting fact about Prime numbers

1.>  2 is the only even Prime number.                                                                                                   
2.>  every prime number can represented in form of 6n+1 or 6n-1, where n is natural number.                                             
3.>  2, 3 are only two consecutive natural numbers which are prime too.
4.>  Goldbach Conjecture: Every even integer greater than 2 can be expressed as the sum of two primes.
5.>  GCD of a natural number with Prime is always one.
6.>  Wilson Theorem : Wilson’s theorem states that a natural number p > 1 is a prime number if and only if
            (p - 1) ! ≡  -1   mod p 
            OR  (p - 1) ! ≡  (p-1) mod p
7.>  Fermat’s Little Theorem: If n is a prime number, then for every a, 1 <= a < n,
             an-1 ≡ 1 (mod n)
             OR 
             an-1 % n = 1 
8.>  Prime Number Theorem : The probability that a given, randomly chosen number n is prime is inversely proportional to its number of          digits, or to the logarithm of n.
9.>  Lemoine’s Conjecture : Any odd integer greater than 5 can be expressed as a sum of an odd prime (all primes other than 2 are odd) and      an even semiprime. A semiprime number is a product of two prime numbers. This is called Lemoine’s conjecture.

How we check whether a number is Prime or not?

1.> Naive solution.
          A naive solution is to iterate through all numbers from 2 to n-1 and for every number check if it divides n. If we find any                 number that divides, we return false.
          
          bool isprime(int n){
               if(n<1){
                  return false;
                  }
               else{
                   for(i=2;i<n;i++){
                       if(n%i==0){
                           return false;}
                           }
                           return true;
                           }
                           
                           
                           
                           
    Time complexity : O(n)
