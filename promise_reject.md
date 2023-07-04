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

    //resolve("value 3")
    reject (new Error("error"))
  }, 2100)

})

let promise_all = Promise.reject([p1, p2, p3])

promise_all.then((value) => {

  console.log(value)

})

OutPut:

Uncaught (in promise) 
Array(3) [ Promise { "pending" }, Promise { "pending" }, Promise { "pending" } ]



Uncaught (in promise) Error: error
    p3 https://promiseapi--shubhangikalban.repl.co/script.js:24
    setTimeout handler*p3< https://promiseapi--shubhangikalban.repl.co/script.js:21
    <anonymous> https://promiseapi--shubhangikalban.repl.co/script.js:19

Uncaught (in promise) Error: error
    p1 https://promiseapi--shubhangikalban.repl.co/script.js:6
    setTimeout handler*p1< https://promiseapi--shubhangikalban.repl.co/script.js:3
    <anonymous> https://promiseapi--shubhangikalban.repl.co/script.js:1


