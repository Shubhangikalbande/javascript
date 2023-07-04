let p1= new Promise((resolve,reject)=>{

setTimeout(()=>{
  
  console.log(" hey ,promise is not resolved")
  
  resolve(1)

},2000)
  
})

p1.then((value)=>{


  setTimeout(()=>{
  
    
console.log("congo,promised resolved")
  
    
  }, 2000)

  
})

p1.then((value)=>{

  

  console.log("hurray!!")
  
  return new Promise((resolve,reject)=>{
  
     setTimeout(()=>{
     
       console.log(" promises r meant to be broken ")
       
       resolve(4)
       
     },5000)

  })

  
  
}).then ((value)=>{

  console.log(value)
})

Output:

  hey ,promise is not resolved 
  
hurray!! 

congo,promised resolved 

 promises r meant to be broken 
 
4
