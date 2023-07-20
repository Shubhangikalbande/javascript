let a = (text) => {

  return new Promise((resolve, reject) => {
  

    setTimeout(() => {
    

      resolve(text)
      

    }, 3000)
    

  })

}
(async () => {

  let text = await a("hello")

  console.log(text)

  text = await a("world")

  console.log(text)


})()

Output:

//after 3 seconds 

Hello

//after 3 seconds

world
