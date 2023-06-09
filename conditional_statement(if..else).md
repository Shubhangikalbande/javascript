if...esle statement

let age = process.argv[2]; // Read the age from command-line argument
console.log("User entered: " + age);

if (age > 0) {
  console.log("this is valid");

}
else {
  console.log("this is inavlid");
}

node filename.js 25 //Give 25 as input
 
Output: this is valid

node filename.js -25 //Give -25 as input

Output: this is invalid


