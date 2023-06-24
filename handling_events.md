let x=function(e) {


  alert("HI! 1")
  
}
 let y=function(e) {

  alert("HI! 2")
}

container.addEventListener('click',x)

container.addEventListener('click',y)

let a= prompt("whats ur favour number")

if( a=="2")

{

  container.removeEventListener('click',x)
  
}

Output: 

On cliicking the button ,user will be able to see Hi1 & HI2 .
On click 2,user will se Hi2 only
