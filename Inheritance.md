class Animal {

  constructor(name, color, found)
  {
    this.name = name;
    
    this.color = color;
    
    this.found = found;
    
  }

  run() {
  
    console.log(this.name + " is running.");
    
  }

  barking() {
  
    console.log(this.name + " is of color " + this.color + " and is barking.");
    
  }
}

class Habitat extends Animal {

  shelter() {
  
    console.log(this.name + " is of color " + this.color + " and is found at " + this.found + ".");
    
  }
  
}

let Flora = new Habitat("Tiger", "yellow", "den");

let Flora2=new Animal("dog","black")

Flora.run();

Flora.shelter();

Flora2.barking();

Output:

Tiger is running.

Tiger is of color yellow and is found at den. 

dog is of color black and is barking.
