let num = [2, 3, 4, 5, 6];

// forEach loop

num.forEach((element) => {
  
  console.log(element * element);
  
});

//Array from

let num2="Shubh"

let arr=Array.from(num2)

console.log(arr)

//for..of

for (let item of num){
  
  console.log(item)
  
}

//for ..in

for (let i  in num2){
  
  console.log(i)
  
}

Out:
4
9
16
25
36

[ 'S', 'h', 'u', 'b', 'h' ]

2
3
4
5
6


0
1
2
3
4
