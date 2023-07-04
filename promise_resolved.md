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
  }, 2100)

})

let promise_all = Promise.resolve([p1, p2, p3])

promise_all.then((value) => {

  console.log(value)

})

Output:

Array(3) [ Promise { "pending" }, Promise { "pending" }, Promise { "pending" } ]

Uncaught (in promise) Error: error
   
    setTimeout handler*p1< https://promiseapi--shubhangikalban.repl.co/script.js:3
    
