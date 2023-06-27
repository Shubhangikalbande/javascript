function loadscript(src ,callback){

  var script =document.createElement("script");
  
  script.src=src;
  
  document.body.appendChild(script);
  
  script.onload=function (){
  
   console.log("loaded script with src :" +src)
   
      callback(src);
  }
  
}

function hello(src)

{

  alert("hello" + src);
  
}

function Goodmorning()

{

  alert("Goodmorning");
  
}

loadscript("https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js" , hello)
