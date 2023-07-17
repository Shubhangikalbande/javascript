class Complex {

  constructor(real, imaginary) {
  
    this.real = real;
    
    this.imaginary = imaginary;
    
  }
  

  add(num) {
  
    this.real = this.real + num.real;
    
    this.imaginary = this.imaginary + num.imaginary;
    
  }

  get real() {
  
    return this._real;
    
  }
  

  get imaginary() {
  
    return this._imaginary;
    
  }

  set real(newReal) {
  
    this._real = newReal;
  }
  

  set imaginary(newImaginary) {
  
    this._imaginary = newImaginary;
    
  }
  
}

let a = new Complex(2, 4);

let b = new Complex(6, 7);

 a.real=10;
 
a.imaginary=10;

a.add(b);

console.log(`${a.real}+${a.imaginary}i`);

Output:

16+17i
