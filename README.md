## Welcome to my GitHub Profile! 👋 

<a href="https://leanpub.com/all-about-solidity-book#:~:text=A%20developer%20guide%20for%20smart,build%20new%20protocols%20and%20dApps.&text=Discover%20the%20secrets%20of%20the,About%20Solidity%22%20for%20a%20reason!" target="_blank"><img src="https://d2sofvawe08yqg.cloudfront.net/all-about-solidity-book/s_hero?1715538832" alt="side Gif" style="z-index: 99999999" align="right" height="auto"/></a>

[![X (formerly Twitter) URL](https://img.shields.io/twitter/url?url=https%3A%2F%2Fx.com%2FJeanCavallera&style=social&label=Follow%20Me&labelColor=1DA1F2)](https://x.com/JeanCavallera)
[![Contact Me](https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&labelColor=0A66C2&color=0A66C2&logoColor=white&label=%20)](https://www.linkedin.com/in/jeancav/)
[![Read My Articles](https://img.shields.io/static/v1?message=Medium&logo=medium&labelColor=000000&color=000000&logoColor=white&label=%20)](https://medium.com/@jeancvllr)
[![Youtube videos](https://img.shields.io/static/v1?message=YouTube&logo=youtube&labelColor=FF0000&color=FF0000&logoColor=white&label=%20)](https://www.youtube.com/playlist?list=PLFb3VvViujW7bvEh_UdPChneZsZC8tXdZ)

I am Jean (French as you might guess! 🥖🥐), a passionate web3 developer, specialised in Smart Contracts, EVM and Solidity.

I am also the 📓 Author of the [**All About Solidity Book**](https://leanpub.com/all-about-solidity-book#:~:text=A%20developer%20guide%20for%20smart,build%20new%20protocols%20and%20dApps.&text=Discover%20the%20secrets%20of%20the,About%20Solidity%22%20for%20a%20reason!)! + the 📑 Writer of the [**All About Solidity** article series](https://medium.com/me/stories/public)

- 🔭 **Currently working as:** Smart Contract Team Lead at LUKSO.
- 🌱 **Currently learning:** Defi.
- 🤝🏻 **Looking to collaborate on:** any web3 protocol or project.
- 💬 **Ask me anything about:** smart contracts and Solidity! 🫡

### 🎙️ Talks & Presentations

- [Building a POAP using the LSP8 Standard - Eth Denver 2024 Workshop.](https://www.youtube.com/watch?v=ff_IYOuQn_s&pp=ygUOamVhbiBjYXZhbGxlcmE%3D)
- [The Bytecode Episode #4 - Explaining the LSP6 Key Manager](https://www.youtube.com/watch?v=2Sm9LsCPjdE)
- [LUKSO LSP Recipes to build new protocols](https://www.youtube.com/watch?v=cx7EHlP6BZM&pp=ygUOamVhbiBjYXZhbGxlcmE%3D)
- LUKSO Standard Proposal Workshops for BuildUP #2 Hackathon - [Episode 1](https://www.youtube.com/watch?v=PrXVcRL1n98) | [Episode 2](https://www.youtube.com/watch?v=xQV2l7VSRZ0)

<br/> 

```solidity title="GitHubProfile.sol"
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import { Ownable } from "@openzeppelin/contracts/access/Ownable.sol";

contract GitHubProfile is Ownable(0xB82023c6d61C60E8715db485066542d501A91140) { // cj42.eth

    struct Github {
        string username;
        string url;
    }

    Github githubInfos;

    /// @dev Set as constant as assigned at birth (and not planning to change it!)
    string public constant FIRST_NAME = "Jean";
    string public job;

    string[] public skills;

    constructor() {
        githubInfos.username = "CJ42";
        githubInfos.url = "https://github.com/CJ42";

        job = "Smart Contract Team Lead at LUKSO";
        
        skills.push("Solidity");
        skills.push("Smart Contracts");
        skills.push("Blockchain");
        skills.push("Web Development");
        skills.push("React");
    }

    function updateJob(string memory newJob) public onlyOwner {
        job = newJob;
    }

    function addSkill(string memory newSkill) public {
        skills.push(newSkill);
    }

    function getSkills() public view returns (string[] memory) {
        return skills;
    }
}
```

<!--
**CJ42/CJ42** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:
- ⚡ Fun fact: ...
- 🤔 **I’m looking for help** with front-end web design to 
-->

## 🌟 Featured Projects

<img src="https://github-readme-stats.vercel.app/api?username=cj42&count_private=true&show_icons=true&include_all_commits=true" align="right" alt="Jean's Github Stats" height="auto"/>

- **All About Solidity**
    - [The Book](https://leanpub.com/all-about-solidity-book#:~:text=A%20developer%20guide%20for%20smart,build%20new%20protocols%20and%20dApps.&text=Discover%20the%20secrets%20of%20the,About%20Solidity%22%20for%20a%20reason!)
    - [The Article Series](https://medium.com/coinmonks/all-about-solidity-article-series-f57be7bf6746
)
    - [Repository with more in-depth explanations and code examples](https://github.com/CJ42/All-About-Solidity).
- [Blockchain Academic References](https://github.com/CJ42/Blockchain-Academic-References)
- [Bitcoin Core Alpha release](https://github.com/CJ42/original-bitcoin-core-code-explained) - Deep Dive into the C++ source code.

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=cj42&hide=TeX&layout=compact" alt="Jean's Github Stats" align="right" height="auto"/>

### 💝 LUKSO Featured

- [Twitter UP dApp](https://github.com/CJ42/twitter-up-dapp)
- [LUKSO Hardhat Template](https://github.com/CJ42/LUKSO-Hardhat-template)
- [LUKSO Forge Template](https://github.com/CJ42/lukso-forge-template)

### 👨🏻‍🍳 Ongoing projects I am cooking

- [**solidity-debugger.io**](https://solidity-debugger.io/) - curated list of Solidity errors and warnings + their explanations and how to fix them.
- [**Decentralised Relayer Contracts**](https://github.com/CJ42/contracts.any.sender) - optimised forked version of any.sender working with Solidity 0.8.x
- [**Solidity Bytes Utils**](https://github.com/CJ42/Solidity-BytesUtils) - Solidity library to manipulate bits and bytes.




