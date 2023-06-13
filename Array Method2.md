let n=[771 ,3, 5,-8,90]

let b=n.toString()

console.log(b ,typeof b)

let c=n.join("*")

console.log(c)

let d=n.pop()

console.log(d ,n)

let e=n.push(100)

console.log( e,n)

let f=n.shift()

console.log(f ,n)

let g=n.unshift(-2)
console.log(g ,n)

delete n[0]
console.log(n,n.length)

let n2=[34, 78,9,0]

let n3=[9 ,0 ,45, 89,76]

let newarray=n.concat( n2,n3)

console.log(newarray)

let num=newarray.sort()

console.log(num)

Output:

771,3,5,-8,90 string

771*3*5*-8*90

90 [ 771, 3, 5, -8 ]

5 [ 771, 3, 5, -8, 100 ]

771 [ 3, 5, -8, 100 ]

5 [ -2, 3, 5, -8, 100 ]

[ <1 empty item>, 3, 5, -8, 100 ] 5

[ <1 empty item>, 3, 5, -8, 100, 34, 78, 9, 0, 9, 0, 45, 89, 76 ]

[ -8, 0, 0, 100, 3, 34, 45, 5, 76, 78, 89, 9, 9, <1 empty item> ]
