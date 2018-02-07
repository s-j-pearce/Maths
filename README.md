# Maths

## Table of contents:
 1.0 Introduction:

 1.1 How to calculate the greatest common divisor and the least common multiple:

 1.2 Arithmetic and geometric progressions:

 1.3 expectation of an event occurring from a discrete, random variable:

 1.4 simple shapes using co-ordinate geometry:

 1.5 integral calculus to solve practical problems involving area:

 1.6 coordinate system used in programming a simple output device:

## 1.0 Introduction:
Within this document, I will be looking at the methodologies and ideaolagies of some mathematical equations and terms.
## 1.1 How to calculate the greatest common divisor and the least common multiple:
### Greatest common divisor:
GCD or the greatest common divisor is the largest number that divides the given numbers. In order to calculate the greatest common divisor you must first find out all of the divisors for the given numbers. Once you have all the divisors, you will compare the two sets and find the largest divisor that is shared between the two groups.
#### GCD Example:
Find the GCD of 45 and 54.

Step 1: Find the divisiors of given numbers:

The divisiors of 45 are : 1, 3, 5, 9, 15, 45

The divisiors of 54 are : 1, 2, 3, 6, 9, 18, 27, 54

Step 2: Find the greatest number that these two lists share in common. In this example the GCD is 9.
### Least common multiple:
LCM stands for Lowest Common Multiple. LCM is the smallest number that is a multiple of both a and b.
#### LCM Example:
Find the LCM of 6 and 8.

The multiples of 6 are : 6, 12, 18, 24, 30, . . .

The multiples of 8 are : 8, 16, 24, 32, 40, . . .

So, the Lowest Common Multiple is 24.
## 1.2 Arithmetic and geometric progressions:
Here is a code for an algorithm to calculate Arithmetic and Geometric Progression:
```C++
#include <iostream> /*Libary*/
#include <time.h>


using namespace std;

int main () {
  
int input;

cout << "Enter a number" << "\n";

cin >> input;

int geometric = input + input;

int geometric2 = geometric + input;

int geometric3 = geometric2 + input;

cout << "Geometric Number: " "\n";
cout << geometric << "\n";
cout << geometric2 << "\n";
cout << geometric3 << "\n";
}
```
## 1.3 Conditional probability:
Conditional probability is when the probability of one event all depends on a possible previous event. The easiest way to understand this theory is to visualise it in a tree diagram. Below is an example of a tree diagram:
![probability-marbles-tree2](https://user-images.githubusercontent.com/31927590/35920684-6b1ac004-0c10-11e8-8878-93d21060177d.gif)

The example above is of a bag full of marbles, there are 2 blue marbles and 3 red marbles. we want to find out what the probability is that we will pull out 2 blue marbles.
![probability-marbles-tree3](https://user-images.githubusercontent.com/31927590/35920698-770cb4bc-0c10-11e8-815c-8c8026e9e518.gif)

The example above shows the process to find out the probability of pulling out 2 blue marbles. As you can see in the first branch, there is a 2/5 chance of pulling out a Blue marble, and a 3/5 chance for Red. We can go one step further and see what happens when we pick a second marble. If a blue marble was selected first there is now a 1/4 chance of getting a blue marble and a 3/4 chance of getting a red marble. If a red marble was selected first there is now a 2/4 chance of getting a blue marble and a 2/4 chance of getting a red marble.

We can now answer the question of what is the probability of pulling out 2 blue marbles. The Answer is 2/5 chance followed by 1/4 chance:

That translates to: 2/5 * 1/4 = 2/20 = 1/10

That means that the chance of pulling out two blue marbles is 1/10.
## 1.4 expectation of an event occurring from a discrete, random variable:

## 1.5 simple shapes using co-ordinate geometry:

## 1.6 integral calculus to solve practical problems involving area:

## 1.7 coordinate system used in programming a simple output device:
