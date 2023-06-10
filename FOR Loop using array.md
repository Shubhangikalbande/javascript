let marks = {
  harry: 34,
  rohan: 98,
  akash: 35,
  monika: 5
};


for (let i = 0; i < Object.keys(marks).length; i++)
{
  
  let key = Object.keys(marks)[i];
  
  console.log("Marks of " + key + " are " + marks[key]);
}

Output:

Marks of harry are 34

Marks of rohan are 98

Marks of akash are 35

Marks of monika are 5
