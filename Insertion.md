let a = document.getElementsByTagName('div')[0]

//a.innerHTML = a.innerHTML + "<h> HELLO WORLD !</h>"


let div = document.createElement('div');

div.innerHTML = '<h> <b>HELLO WORLD!! </b></h>';

a.append(div);//will reflect in the last

a.prepend(div);//will reflect at the start

a.before(div);// quite similar to prepend but before div starts

a.after(div); //will reflect in th end but ou tof div

a.replaceWith(div)
