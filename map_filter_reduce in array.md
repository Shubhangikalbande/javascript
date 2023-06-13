//map is used to create new array

let arr = [34, 78, 92];

console.log(arr);

let a = arr.map((value ,index ,array) =>
  {
  
  console.log(value, index,array);
    
  return value + 2;
    
});

console.log(a, arr)


//filter

let arr2 =[ 2, 67, 34,9,-45,90]

let  a2=arr2.filter((value)=>{
  
return value>10
  
})

console.log (a2,arr2) 

// Reduce

let arr3=[1 ,2, 1, 3, 4, 2, 1 ]

 let newarr3=arr3.reduce((h1,h2)=>{

  return h1+h2
   
 } )

console.log(newarr3)

Output:

[ 34, 78, 92 ]

34 0 [ 34, 78, 92 ]

78 1 [ 34, 78, 92 ]

92 2 [ 34, 78, 92 ]

[ 36, 80, 94 ] [ 34, 78, 92 ]

[ 67, 34, 90 ] [ 2, 67, 34, 9, -45, 90 ]

14
