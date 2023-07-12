class RailwayForm {

  constructor(givenname, trainno, address) {
  
    console.log("constructor called...." + " " + givenname + " " + trainno);
    
    this.name = givenname;
    
    this.number = trainno;
    
    this.address = address;
  }

  preview() {
  
    console.log(this.name + " your train no is: " + this.number + " and your address is: " + this.address);
    
  }

  

  submit() {
  
    console.log(this.name + ", your train no is: " + this.number  + " and your address is: " + this.address + " is confirmed.");
    
     
  }
  cancel() {
    console.log(this.name + ", your address is " + this.address + " your train number is..");
    
    this.number=0
    
  }
}

let ShubhangiForm = new RailwayForm("shubhangi", 785634, " wakad pune 411057");

ShubhangiForm.preview();

ShubhangiForm.submit();

ShubhangiForm.cancel();

ShubhangiForm.preview();

Output:

constructor called.... shubhangi 785634 

shubhangi your train no is: 785634 and your address is:  wakad pune 411057 

shubhangi, your train no is: 785634 and your address is:  wakad pune 411057 is confirmed. 

shubhangi, your address is  wakad pune 411057 your train number is.. 

shubhangi your train no is: 0 and your address is:  wakad pune 411057
