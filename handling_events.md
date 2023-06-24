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
