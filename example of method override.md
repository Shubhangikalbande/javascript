class Human {

  constructor(name, favfood) {
  
    this.name = name;
    
    this.favfood = favfood;
  }
  

  walk() {
  
    console.log(this.name + " is walking fast & " + this.favfood + " is his fav food");
    
  }
  
}

class Student extends Human {

  constructor(name, favfood) {
  
    super(name, favfood); // Call the parent class constructor using super()
    
  }

  walk() {
  
    console.log(this.name + " is running & " + this.favfood + " is his fav food");
    
  }
  
}

let b= new Human("Chetan","vada pav")

b.walk()

let a = new Student("Aggu", "pizza"); // Provide both name and favorite food as arguments

a.walk();

Output:

Chetan is walking fast & vada pav is his fav food 

Aggu is running & pizza is his fav food
