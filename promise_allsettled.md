let p1 = new Promise((resolve, reject) => {

  setTimeout(() => {

    //resolve("value 1")
    
    reject(new Error("error"))
    
  }, 2500)

})

let p2 = new Promise((resolve, reject) => {

  setTimeout(() => {

    resolve("value 2")
    // reject (new Error("error"))
  }, 400)

})

let p3 = new Promise((resolve, reject) => {

  setTimeout(() => {

    resolve("value 3")
    
    //reject (new Error("error"))
  }, 100)

})


let promise_all = Promise.allSettled([p1, p2, p3])


promise_all.then((value) => {

  console.log(value)

})

Output:

Array(3) [ {…}, {…}, {…} ]

0: Object { status: "rejected", reason: Error }

​
1: Object { status: "fulfilled", value: "value 2" }

​
2: Object { status: "fulfilled", value: "value 3" }

​
length: 3

​
<prototype>: Array []


​
