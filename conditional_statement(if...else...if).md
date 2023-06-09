let age = process.argv[2]; // Read the age from command-line argument


console.log("User entered: " + age);
if (age < 0) 
{
  console.log("this is invalid");

}

else if (age < 9)
{
  console.log(" u r a kid")
}

else if (age < 18 && age > 9) {
  console.log(" u still cant drive")
}

else {
  console.log(" u can drive");
}
