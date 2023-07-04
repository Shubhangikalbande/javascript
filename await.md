async function pro() {

  let puneweather = new Promise((resolve, reject) => {

    setTimeout(() => {
      resolve("pune weather is 26 deg")
    }, 2000)
  })

  let mumbaiweather = new Promise((resolve, reject) => {

    setTimeout(() => {
      resolve("mumbai weather is 30 deg")
    }, 4000)
  })

  //puneweather.then(alert)
  //mumbaiweather.then(alert)
  
  console.log(" fetching pune's weather,please wait..")
  
  let punew = await puneweather
  
  console.log(" pune's weather is fetched", punew)
  
  console.log(" fetching mumbai's weather,please wait...")
  
  let mumbaiw = await mumbaiweather
  
  console.log(" mumbai's weather is fetched", mumbaiw)
  
  return [punew, mumbaiw]
}

console.log("tell me today's weather")

let a = pro()

a.then((value) => {

  console.log(a)
})


output:


tell me today's weather 

 fetching pune's weather,please wait.. 

 pune's weather is fetched pune weather is 26 deg 
 
 fetching mumbai's weather,please wait... 
 
 mumbai's weather is fetched mumbai weather is 30 deg 
 
Promise { <state>: "fulfilled", <value>: (2) […] }
​
"
​
<value>: Array [ "pune weather is 26 deg", "mumbai weather is 30 deg" ]
​


​

