
# Permutations and Combinations Overview

This document provides a summary of the basic principles and formulas used in permutations and combinations, which are fundamental concepts in combinatorics. These tools are essential in various fields such as probability, statistics, and discrete mathematics.

## Introduction to Permutations and Combinations

Permutations and combinations are methods used to count the number of possible arrangements or selections of objects. The key difference between them is whether the order of the objects matters:

- **Permutations**: The order of the objects matters.
- **Combinations**: The order of the objects does not matter.

### Key Concepts

1. **Order matters; repetition allowed** (Permutations with repetition):

   - **Formula**: $n^r$
   - **Example**: Creating a password of 3 letters, using 26 different letters (with repetition allowed):
     $26^3 = 17,576\text{ possible passwords}$

2. **Order matters; repetition not allowed** (Permutations without repetition):

   - **Formula**: $P(n, r) = \frac{n!}{(n-r)!}$
   - **Example**: Assigning 3 distinct prizes to 5 people:
     ${P}(5, 3) = \frac{5!}{(5-3)!} =\frac{5!}{2!} = 5\times4\times3= 60\text{ ways}$

3. **Order doesn't matter; repetition not allowed** (Combinations):

   - **Formula**: $C(n, k) = \frac{n!}{k!(n-k)!} = \binom{n}{k}$
   - **Example**: Selecting 3 people from a group of 10:
     $\binom{10}{3} =  \frac{10!}{3!(10-3)!} = \frac{10!}{3!\times7!} =\frac{10\times9\times8}{3\times2\times1} =120\text{ combinations}$

4. **Order doesn't matter; repetition allowed** (Combinations with repetition):

   - **Formula**: ${C}(n+k-1,k) = \frac{(n+k-1)!}{k!(n-1)!} =\binom{n + k - 1}{k}$
   - **Example**: Ordering 8 tacos from 3 different types:
     $\binom{3+8 - 1}{8} = \binom{10}{8} = \frac{10!}{8!(10-8)!}= \frac{10\times9}{2\times1}=45\text{ ways}$

### Permutations of a Multiset

When dealing with permutations of a multiset (where some elements are repeated), the formula adjusts to account for the repetitions:

- **Formula**: $P(n; r_1, r_2, \ldots, r_k) = \frac{n!}{r_1! r_2! \ldots r_k!}$
- **Example**: Anagramming the word "BALLOON" (7 letters, with repetitions):
  $\frac{7!}{1!\times1!\times2!\times2!\times1!} = 1260\text{ possible anagrams}$

## Conclusion

This guide summarizes the foundational formulas and concepts related to permutations and combinations. Understanding when and how to apply these principles is crucial in combinatorics and related mathematical fields. For practical applications, ensure that you correctly identify whether the order of selection matters and whether repetition of elements is allowed.
