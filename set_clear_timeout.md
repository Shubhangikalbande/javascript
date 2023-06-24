document.write("hello")

a=setTimeout(function()
{

  alert("Time Out")
  
}, 5000)

b=prompt ("do u want to set time ,y or n")

if( b== "n")

{

clearTimeout(a); 

}
