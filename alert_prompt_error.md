let runagain=true


const candrive=(a)=>{

  return a>=18?true:false

}

while (runagain){

let a=prompt("enter age")

a=Number.parseInt(a)


  if (a<=0)
  {
    
    console.log("you hav entered wrong age")
    break;
  
  }
  
if (candrive(a))
{
  alert( "  yes you can drive")

}
   
else{
  alert(" you can't drive" )
}

runagain=confirm("you want to play again")
}
