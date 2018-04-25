# Maths
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
## 1.4 Probability of a random integer being divisible by 5:
One out of every five numbers is divisible by 5, meaning there is a 1/5 chance. 5 can be divided by numbers in the 5 timetables such as 40,45,50 which means 5 is divisible 1/5 times. Whereas 0,1,2,3, or 4 dont have the same probability to equate, or be divisible by 5.

An example is:

Range 1-100 / Total = 20/100 = 1/5
### Event occurring from a discrete, random variable:
![36476634-5e589bac-16f6-11e8-83ad-c865fdd0e82e](https://user-images.githubusercontent.com/31927590/36792478-9e3d78c2-1c92-11e8-8f8f-2de8bd9059ab.PNG)
Above is the random selection event only possible from a finite set of inputs. The selection is always made fromm a finite set which is repeated. Each time a selection is made it is from a bigger set.

## 1.5 simple shapes using co-ordinate geometry:
Here is the code i made to calculate simple shapes using co-ordinate geometry:
```C++
#include <iostream>
#include <cmath>
using namespace std;
int main() {
 int x[4], y[4];
 char next;
 int count;

 for(count=0; count<4; count++){
 cout << "Enter coordinates?";
 cin >> next;

 if(next=='Y'){
 cout << "\nEnter X" << count+1 << "=";
 cin >> x[count];

 cout << "\nEnter Y" << count+1 << "=";
 cin >> y[count];
 }else{
 cout << "\nOk, we have " << count << " coordinates";
 break;
 }
 }

 if(count==4){
 //distance between 2 points

 double term1 = pow((x[1]-x[0]),2);
 double term2 = pow((y[1]-y[0]),2);

 double d1 = sqrt(term1+term2);

 term1 = pow((x[3]-x[2]),2);
 term2 = pow((y[3]-y[2]),2);

 double d2 = sqrt(term1+term2);

 term1 = pow((x[2]-x[0]),2);
 term2 = pow((y[2]-y[0]),2);

 double d3 = sqrt(term1+term2);

 term1 = pow((x[3]-x[1]),2);
 term2 = pow((y[3]-y[1]),2);

 double d4 = sqrt(term1+term2);

 if(d1==d2 && d2==d3 && d3==d4){
 cout << "\nSquare!";
 }else if(d1==d2 && d3==d4){
 cout << "\nRectangle!";
 } else{
 cout << "\nNot a simple shaple!";
 }
 } else if(count == 3){
 double term1 = pow((x[1]-x[0]),2);
 double term2 = pow((y[1]-y[0]),2);

 double d1 = sqrt(term1+term2);

 term1 = pow((x[2]-x[0]),2);
 term2 = pow((y[2]-y[0]),2);

 double d2 = sqrt(term1+term2);

 term1 = pow((x[2]-x[1]),2);
 term2 = pow((y[2]-y[1]),2);

 double d3 = sqrt(term1+term2);

 if(d1!=0 && d2!=0 && d3!=0){
 cout << "\nTriangle!";
 }else{
 cout << "\nNot a simple shaple!";
 }

 } else {
 cout << "\nNot a simple shaple!";
 }

 return 0;
}
```
## 1.6 integral calculus to solve practical problems involving area:
### Calculus:
Calculus is the mathematical study of continuous change, this means the study of instantaneous change over tiny intervals of time.
### Integral:
In mathematics, an integral assigns numbers to functions in a way that can describe displacement, area, volume, and other concepts that arise by combining infinitesimal data.
## Determine shape parameters using appropriate vector methods:
A vector is a quantity or phenomenon that has two independent properties; magnitude direction. The term also denotes the mathematical or geometrical representation of such a quantity. To scale shapes and identify shape parameters i have created a formula that you can use to scale a shape vector method. The formula or code is below:

```
<body>

<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;"></canvas>

<br>
<button onclick="move(1)">LEFT</button>
<button onclick="move(2)">UP</button>
<button onclick="move(3)">DOWN</button>
<button onclick="move(4)">RIGHT</button>
<br>
<button onclick="move(5)">DIAGONAL RIGHT DOWN</button>
<button onclick="move(6)">DIAGONAL RIGHT UP</button>
<br>
<button onclick="move(7)">DIAGONAL LEFT DOWN</button>
<button onclick="move(8)">DIAGONAL LEFT UP</button>
<br>
<button onclick="shape()">SHAPE?</button>


<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();

var curX=parseInt(prompt("Please enter the initial X"));;
var curY=parseInt(prompt("Please enter the initial Y"));;

function move(dir){
var mag = parseInt(prompt("Please enter the magnitude"));

if(dir==1){
  //left
  ctx.moveTo(curX, curY);
  curX = curX-mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Left / Vector Magnitude: "+mag);
}else if(dir==2){
  //up
  ctx.moveTo(curX, curY);
  curY = curY-mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Up / Vector Magnitude: "+mag);
}else if(dir==3){
  //down
  ctx.moveTo(curX, curY);
  curY = curY+mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Down / Vector Magnitude: "+mag);
}else if(dir==4){
  //right
  ctx.moveTo(curX, curY);
  curX = curX+mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Right / Vector Magnitude: "+mag);
}else if(dir==5){
  //diagonal right down
  ctx.moveTo(curX, curY);
  curX = curX+mag/2;
  curY = curY+mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Right Down / Vector Magnitude: "+mag);
}else if(dir==6){
  //diagonal right up
  ctx.moveTo(curX, curY);
  curX = curX+mag/2;
  curY = curY-mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Right Up / Vector Magnitude: "+mag);
}else if(dir==7){
  //diagonal left down
  ctx.moveTo(curX, curY);
  curX = curX-mag/2;
  curY = curY+mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Left Down / Vector Magnitude: "+mag);
}else if(dir==8){
  //diagonal left up
  ctx.moveTo(curX, curY);
  curX = curX-mag/2;
  curY = curY-mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Left Up / Vector Magnitude: "+mag);
}

ctx.stroke();

}

function shape(){
  var shape = prompt("Is this a shape Y/N?");

  if(shape=='Y'){
      prompt("What shape?");
  }else {
      alert("Keep drawing!");
  }
}

</script>

</body>
</html>
```
## Determine the rate of change within an algebraic function:
The average rate of change is the average rate that one value is changing with respect to another value changing. Some well known rates of change include 'Miles per gallon' which is calculated by dividing the cost of electricity by the number of kilowats used. There is also another well know one which is 'miled per hour', this is calculated by dividing the number of miles travelled by the number of hours it takes to travel them. In general the average rate of change function is a process that calculates the amount of change in one item divided by the corresponding amount of change in another. We use this function to work out the rate of change:
![rate of change](https://user-images.githubusercontent.com/31927590/39234950-8af38742-486c-11e8-929e-0104630fd601.jpg)

