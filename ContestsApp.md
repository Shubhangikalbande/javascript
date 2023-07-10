let url = "https://kontests.net/api/v1/all";
let response = fetch(url);

response.then((v) => {
  return v.json();
}).then((contests) => {
  console.log(contests);

  let ihtml = "";
  let cardcontainer = document.getElementById("cardcontainer");

  for (let item in contests) {
    let contest = contests[item];
    let imageUrl = getContestImageUrl(contest); // Call a function to determine the image URL

    ihtml += `
      <div class="card" style="width: 23rem;">
        <img src="${imageUrl}" class="rounded float-start" alt="Contest Image">
        <div class="card-body">
          <h5 class="card-title">${contest.name}</h5>
          <p class="card-text">Take Challenge</p>
          <p>Starts at: ${contest.start_time}</p>
          <p>Ends at: ${contest.end_time}</p>
          <a href="${contest.url}" class="btn btn-primary">Visit Contest</a>
        </div>
      </div>
    `;
  }

  cardcontainer.innerHTML = ihtml;
});

function getContestImageUrl(contest) {
 
  if (contest.name === "ProjectEuler+") 
  {
    return "https://media.istockphoto.com/id/537331500/photo/programming-code-abstract-technology-background-of-software-deve.webp?b=1&s=170667a&w=0&k=20&c=iQE4in2blXsYoRYjoX7F8e4AFF6kOaE-TZiVNMPQ5kI="; 
  }
  else if (contest.name === "1v1 Games by CodeChef")
  {
    return "https://media.istockphoto.com/id/1356364268/photo/close-up-focus-on-persons-hands-typing-on-the-desktop-computer-keyboard-screens-show-coding.webp?b=1&s=170667a&w=0&k=20&c=DriezQW30CaJxGzEvW_l0Z5vpIrIYqUx7-K1ah2gTx0=";
  } 
  else if (contest.name === "Rootstock: Bitcoin Scaling Hackathon")
  {
    return "https://media.istockphoto.com/id/1413837275/photo/abstract-it-design-background-with-a-tilted-triangular-grid-surface-and-python-computer.webp?b=1&s=170667a&w=0&k=20&c=niNjthAGYXZ9zF8a5d9klfKftbd4Ih_F0jWKP4N3DNM="; 
  }

  return "default.jpg";
}
