class Employee{
   
  Login(){

     console.log("employee has logged in")

   }

  Logout(){

     console.log("employee has logged out")
      
    }

  leavesequest(leaves){

      console.log(`your leaves of ${leaves}   days has been approved-Auto approved`)

    }
}

class Programmer extends Employee{


  sodexo(y)

  {
    console.log(`employee has request ${y} passes`)

  }

   leavesequest(leaves)
  {

    super.leavesequest(3)

  console.log("one extra given")
  }
  
  
}
let a= new Programmer

a.Login()

a.leavesequest(4)

a.sodexo(2)

a.Logout()

Output:

employee has logged in 

your leaves of 3   days has been approved-Auto approved 

one extra given 

employee has request 2 passes 

employee has logged out
