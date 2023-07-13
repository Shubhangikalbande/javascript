class Employee{

  constructor(givenname){

    this.name=givenname
    console.log(`${this.name} ,this the new constructor `)
  }
  
  login()
  {
    console.log(" employe has logged in")
    
  }
  leavesrequest(leaves)
  {
    console.log(`${leaves} has been requested by ${this.name}`)
  }  
}

class programmer extends Employee{
  // constructor{(...argu) 
  //supr(..argu)}--- this has been added by javascript automatically
/*constructor(givenname){
 super(givenname)
    this.name=givenname
    console.log(`${this.name} ,this the new constructor no 2 `)  if th eprogrammer wants to hav constructor for extened class then he needs  to begin constuctor follwed by super passing argument in both follwed by this. */
  }
  leavesrequest(leaves){
    super.leavesrequest(2)
    console.log(` ${leaves} days has been approved...requested by ${this.name}`)
  }
  
}

let a= new programmer("shubhangi")
a.leavesrequest(5)


Output:

shubhangi ,this the new constructor 

shubhangi ,this the new constructor no 2 

2 has been requested by shubhangi 

 5 days has been approved...requested by shubhangi
