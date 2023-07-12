class RailwayForm {

  submit() {
  
    alert(this.name  +  " :your form has been submitted & train no is :"  + this.number )
    
  }
  
  cancel() {
  
    alert(this.name  + "  :your form has been cancelled & train no is :"  + this.number)
  }
  
  fill(givenname, trainno) {

    this.name = givenname
    
    this.number = trainno
  }
}
let ShubhangiForm = new RailwayForm()

ShubhangiForm.fill("shubhangi", 12345)

let AgastyaForm1 = new RailwayForm()

let AgastyaForm2 = new RailwayForm()

AgastyaForm1.fill("Agastya", 22222)

AgastyaForm2.fill("Agastya", 44444)

ShubhangiForm.submit()

AgastyaForm2.cancel()

AgastyaForm1.submit()

Output:

shubhangi :your form has been submitted & train no is :12345 

Agastya  :your form has been cancelled & train no is :44444 

Agastya :your form has been submitted & train no is :22222 

​
