
//There are 7 types of primitive datatypes (N N S S B B U)

let a=null
let b=567
let c=true
let d=BigInt("678")
let e="shu"
let f=Symbol
let g=undefined
console.log(a,b,c,d,e,f,g)

output:
~/jssample$ node primitive.js
null 567 true 678n shu [Function: Symbol] undefined

//Objects  

const item = {
  "shu": true,
  "kal": false,
  "aggu": undefined
}

console.log(item.aggu)

 Output
 ~/jssample$ node primitive.js
undefined
 
