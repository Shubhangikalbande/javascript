const array = [
  "Initializing hack tool....",
  "Connecting to Chetan's gmail..",
  "Connecting to Server 1..",
  "Connection failed, retrying..",
  "Connecting to Server 2..",
  "Connected successfully...",
  "csawai @gmail ID detected..",
  "Trying Brute Force..",
  "200k passwords tried..",
  "Match not found..",
  "Trying again... Please wait",
  "Match found..",
  "Hacked successfully.."
];

const sleep = async (seconds) =>
{
  return new Promise((resolve) =>
  {
    setTimeout(() => {
    
      resolve(true);
      
    }, seconds * 1000);
    
  });
  
};

const hack = async (message) => 
{
  await sleep(2);
  
  console.log(message);
  
  text.innerHTML = text.innerHTML + message + "<br>"

};

(async () => {

  for (let i = 0; i < array.length; i++)
  {
    await hack(array[i]);
  }
})();
