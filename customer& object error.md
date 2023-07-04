try{

  let age= prompt("Enter your age")
  
  age=Number.parseInt(age)
  
  if (age >120){
  
    throw new ReferenceError("This is hypothetical")
  }
  
}

catch(error){

  console.log(error.name)
  
  console.log(error.message)
  
  console.log(error.stack)
  
}

console.log("program still running..")

Output:

 enter input as 160
 
ReferenceError 

This is hypothetical 

program still running.. 

​

