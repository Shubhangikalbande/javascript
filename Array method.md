//Splice and slice

let num=[ 1,5,89,54,-89,-1]

num.splice( 1,3,1022,3022,4022)

console.log(num)

let deletedvalues=num.splice( 1,3,1022,3022,4022)

console.log(deletedvalues)

let newnum=num.slice(5)

console.log(newnum)

let newnewnum=num.slice(3,5)

console.log(newnewnum)

Output:

[ 1, 1022, 3022, 4022, -89, -1 ]

[ 1022, 3022, 4022 ]

[ -1 ]

[ 4022, -89 ]
