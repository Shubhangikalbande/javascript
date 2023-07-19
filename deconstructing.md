let arr = [2, 4, 6, 8,10,155,199]

let [a, b, c, d,...rest] = arr

console.log(a, b, c, d,...rest)

let [e, , f,...rest1] = arr

console.log(e,f,rest1)

let {z,x}={z:1,x:2}

  console.log(z,x)

let arr3=[ 2,4,7]

let obj1 ={...arr3}

console.log(obj1)

function sum( v1, v2, v3){

   return v1+v2+v3
   
}

console.log (sum(...arr3))

Output:

2 4 6 8 10 155 199 

2 6 
Array(4) [ 8, 10, 155, 199 ]
​
0: 8
​
1: 10
​
2: 155
​
3: 199

​
length: 4
​

1 2 

Object { 0: 2, 1: 4, 2: 7 }

13
