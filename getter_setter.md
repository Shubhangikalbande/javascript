class Animal {

  constructor(name) {

    this._name = name
  }

  fly() {

    console.log(this.name + ",animal is flying")
    
  }
  
  get name (){
  
     return this._name
     
  }
  set name (newName){
  
      this._name=newName
  }
}

let a = new Animal("Kite")

a.fly()

a.name="Bruno"

console.log(a.name)

output:

Kite,animal is flying 

Bruno
