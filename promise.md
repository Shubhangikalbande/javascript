let promise = new Promise(function(resolve, reject)

{
  alert("hello four")
  
  resolve(6)
  
})

console.log("hello one")


setInterval(function() {

  console.log(" hello two")
  

}, 1000)


console.log("hello three")

console.log(promise)

Output:

hello one 

hello three 

Promise { <state>: "fulfilled", <value>: 6 }

 hello two  

​

