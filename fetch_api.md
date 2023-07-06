let P = fetch("https://goweather.herokuapp.com/weather/ny")

P.then((value) => {

  console.log(value.status)
  
  console.log(value.ok)
  
  console.log(value.text)
  
  console.log(value.headers)
  
  return value.json()
  
}).then((value2) => {

  console.log(value2)
  
})

Output:

200 

true 

function text()

Headers { "content-length" → "240", "content-type" → "application/json" }
​

<prototype>: HeadersPrototype { append: append(), delete: delete(), get: get(), … }

Object { temperature: "+22 °C", wind: "7 km/h", description: "Partly cloudy", forecast: (3) […] }


​


