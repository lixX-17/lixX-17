- 👋 Hi, my name is Leonardo Monteiro
- 💻 Currently pursuing a Master's in Computer Engineering at the Faculdade de Ciências
- ⚽️🥎🏐🏓 Sports are a big part of my life🎱🥊🥋🏋️‍♀️
- 📱 Here is my Linkedin: https://www.linkedin.com/in/leonardomonteiro3467/)


---------------------------------------------------------------------------------------------------------------------------------
###

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" height="40" alt="java logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/haskell/haskell-original.svg" height="40" alt="haskell logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" height="40" alt="c logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="40" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="40" alt="html5 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="40" alt="css3 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="40" alt="javascript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" height="40" alt="nodejs logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original.svg" height="40" alt="jupyter logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/anaconda/anaconda-original.svg" height="40" alt="anaconda logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" height="40" alt="vscode logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/intellij/intellij-original.svg" height="40" alt="intellij logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" height="40" alt="linux logo"  />
</div>

---------------------------------------------------------------------------------------------------------------------------------------
###

<h2 align="left">My Stats</h2>
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=lixX-17&show_icons=true&theme=tokyonight&bg_color=30,e96443,904e95&title_color=fff&text_color=fff" alt="lixX-17">
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=lixX-17&show_icons=true&theme=vision-friendly-dark&locale=en&layout=compact&langs_count=8&bg_color=30,11998e,38ef7d&title_color=fff&text_color=fff" alt="lixX-17"/>
</p>

const fetch = require("node-fetch");

const username = lixX-17; 
const githubToken = "TEU_GITHUB_TOKEN"; 

const getContributions = async () => {
    const response = await fetch(
        `https://api.github.com/users/${lixX-17}/events/public`,
        {
            headers: { Authorization: `token ${githubToken}` },
        }
    );
    const events = await response.json();
    const contributions = {};

    events
        .filter(event => event.type === "PushEvent")
        .forEach(event => {
            const repo = event.repo.name;
            contributions[repo] = contributions[repo] || 0;
            contributions[repo] += event.payload.size;
        });

    console.log("Contributions by Repository:", contributions);
};

getContributions();


---------------------------------------------------------------------------------------------------------------------------------------
###





