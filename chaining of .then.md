let promise = new Promise((resolve, reject) => {


  setTimeout(() => {

    console.log(" promise will b resolved after 2 sec")
    
    resolve(56)
    
  }, 2000)

})

promise.then((value) => {

  console.log(value)
  
  let p2 = new Promise((resolve, reject) => {
  
    setTimeout(() => {

      resolve("promise 2")
      
    }, 4000)
    
  })
  
  return p2
  

}).then((value) => {

  console.log("we r done")
  
  return 2

}).then((value) => {

  setTimeout(() => {
  
    console.log("we are pakka done")
    
  }, 2000)

})


Output:

promise will b resolved after 2 sec 

56 

we r done 

we are pakka done
