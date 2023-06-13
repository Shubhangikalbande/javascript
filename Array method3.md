let newarray=[978 ,3,90,-34,9000, -21]


let compare =(a,b)=>{

  return a-b;     //arrange in ascending order
  
}
newarray.sort(compare)

console.log(newarray)


let compare2 =(a,b)=>{

  return b-a; // arrange array in DESC order
  
}

newarray.sort(compare2)

console.log(newarray)


newarray.reverse()

console.log(newarray)

Output:

[ -34, -21, 3, 90, 978, 9000 ]

[ 9000, 978, 90, 3, -21, -34 ]

[ -34, -21, 3, 90, 978, 9000 ]
