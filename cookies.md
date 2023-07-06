console.log(document.cookie)

document.cookie = "name=shu345678"

document.cookie = "name2=shu34567891011"

document.cookie = "name2=shu"

let key= prompt("whats ur key")

let value= prompt("whats ur value")

document.cookie=`${encodeURIComponent(key)}=${encodeURIComponent(value)}`

console.log(document.cookie)


Output:

name=shu345678; {$key}={$value}; 567=789; @45=&89; 6788#=6789:898; name2=shu 
name=shu345678; {$key}={$value}; 567=789; @45=&89; 6788#=6789:898; name2=shu; 78%3F%3F%3B'999=%3E0oo'*6666
