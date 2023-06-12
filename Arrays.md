let class_12marks=[
  21 ,67, false ,90,65, "TBA"
]

console.log(class_12marks)

console.log(class_12marks[0])

console.log(class_12marks[1])

console.log(class_12marks[2])

console.log(class_12marks[3])

console.log(class_12marks[4])

console.log(class_12marks[5])

class_12marks[6]=35

console.log(class_12marks[6])

console.log(class_12marks.length) 

Output:
[ 21, 67, false, 90, 65, 'TBA' ]
21
67
false
90
65
TBA
35
7

// write program to print elements in the above array using FOR Loop

for( let i=0;i< class_12marks.length;i++)
  {
    
    console.log(class_12marks[i])
  }
