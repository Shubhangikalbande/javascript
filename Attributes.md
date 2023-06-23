let first = document.getElementById("first");

let a = first.getAttribute("class")

console.log(a)

console.log(first.hasAttribute("class"))

console.log(first.hasAttribute("style"))

first.setAttribute("class", "shubhangi kalbande")

first.removeAttribute("class")


Output:

container 

true 

false 

NamedNodeMap [ id="first" ]


​
