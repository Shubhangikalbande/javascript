class Animal {

  constructor(givenname) {
  
    this.name = Animal.capitalize(givenname)}

  walk() {
  
    console.log("Animal ," + this.name  + " is walking.");
  }
  
  static capitalize(word){
    
return word.charAt(0).toUpperCase() + word.slice(1, word.length);
  }
  
}

let s = new Animal("dianosauras");

s.walk();

Output:

Animal ,Dianosauras is walking.


//Static method is used to implement a function that belongs to a class as a whole and not to any particular object.
