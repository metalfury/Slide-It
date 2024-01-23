# <a name="_toc106213983"></a><a name="_toc106214119"></a><a name="_toc106214171"></a>**TABLE OF CONTENTS**
[**TABLE OF CONTENTS**](#_toc106213983)**

[**ABSTRACT**](#_toc106213985)

[SLIDE IT! DRIFT-BASED MOBILE GAME AND WEBSITE PROJECT](#_toc106213986)

[**INTRODUCTION**](#_toc106213987)

[1. INTRODUCTION](#_toc106213988)

[1.1 PROBLEM STATEMENT](#_toc106213989)

[1.2 MOTIVATION](#_toc106213990)

[**LITERATURE REVIEW**](#_toc106213991)

[2. LITERATURE REVIEW](#_toc106213992)

[**METHOD**](#_toc106213993)

[3. METHOD](#_toc106213994)

[3.1 METHODS USED IN THE DEVELOPMENT OF THE GAME](#_toc106213995)

[3.2 METHODS USED IN THE DEVELOPMENT OF THE WEBSITE](#_toc106213996)

[**RESULTS AND DISCUSSION**](#_toc106213997)

[4. RESULTS AND DISCUSSION](#_toc106213998)

[**REFERENCES**](#_toc106213999)

# **PROJECT MEMBERS**
**Ömer Faruk Can DOĞRUSOY**
**Hüseyin KARAOĞLAN**
**Mert Ömer ŞENER**

# **ABSTRACT**
## <a name="_toc106213986"></a><a name="_toc106214122"></a><a name="_toc106214174"></a>**SLIDE IT! DRIFT-BASED MOBILE GAME AND WEBSITE PROJECT**
The fundamental motivation behind the creation of the Slide It! project is to fill a gap in the mobile gaming market and to establish an ecosystem where both users and developers benefit.

In the Slide It! project, a mobile game has been designed and implemented where users earn points by drifting & exchange with cryptocurrency, and a website has been prepared for information and user transactions.

Unity game engine was used in the development of the Slide It! game. The website was developed using the JavaScript language, with the addition of the ReactJS library. Google Firebase Realtime Database was utilized as a common database for both systems.

As a result, we have a working game with an in-game point earning algorithm and a website with completed front-end development and ongoing back-end development. Both systems are partially integrated with each other.

Developing such a large project requires more time and a slightly larger team. However, the results achieved in a short period are satisfactory.

# <a name="_toc106213987"></a><a name="_toc106214123"></a><a name="_toc106214175"></a>**INTRODUCTION**
## <a name="_toc106213988"></a><a name="_toc106214124"></a><a name="_toc106214176"></a>**1. INTRODUCTION**
The widespread use of smartphones around the world has significantly facilitated companies' access to end-users. Especially with the prevalence of mobile ads and evolving social platforms, almost everyone is now seen as a potential gamer by companies.

With the existence of a substantial audience called Non-Gamers today, the curiosity of this audience in Hyper Casual games on smartphones has led game studios to focus on the mobile market. Considering the active presence of 4.5 billion smartphones globally, the size of the market can be measured.

Devices with advanced features can provide ideal opportunities for outdoor gaming. As observed, computer and console games are relatively expensive, even criticized for price increases in the United States and European countries. Consequently, many gamers prefer more affordable and even free mobile games. Moreover, as the number of game enthusiasts choosing mobile games increases, almost every game available on computers and game consoles is also released in the mobile game environment. This has been one of the factors reducing game prices. Looking at smartphones, it can be observed that many things are consolidated into a single device with the development of technology. Additionally, this technology comes at a lower cost. <sup>[\[1\]](#k1)</sup>

Our game, Slide It!, is designed to create an ecosystem that allows users to earn money while playing, and the earned money can be used either with their own cryptocurrency on real stock exchanges or for in-game purchases in the game market.

Unity game engine was used to develop the game. Unity is a cross-platform game engine developed by Unity Technologies, primarily used for developing video games and simulations for computers, consoles, and mobile devices.

In the development of the website, JavaScript and the React library were employed.

Firebase Realtime Database was used as a shared database for both systems.

Unity game engine has been adopted and used not only in the video game industry but also in various other industries such as the film sector, automotive sector, architecture, engineering, and construction. Unity is a versatile game engine that supports 2D and 3D graphics, drag-and-drop functionality, and script writing with C#. It is compatible with various platforms such as PC, Mac, Web, iOS, Android, Windows Phone, Playstation, Xbox, thanks to its capability to compile a game developed with Unity for different platforms with a single click without the need for any infrastructure changes. <sup>[\[2\]](#k2)</sup>

Firebase Realtime Database is a cloud-based NoSQL (Not Only SQL) database system. It allows management with JSON parameters without the need for any SQL queries. In addition to data storage, it enables real-time tracking of data changes with its asynchronous operation. The structure of Firebase Realtime can be generally thought of as a cloud-based JSON tree structure.

JavaScript, designed by Brendan Eich in 1995 for Netscape, is a weakly typed and dynamically written programming language. Although its initial purpose was to make websites interactive, today, it can run not only in browsers but also on servers with JavaScript runtimes like NodeJs and Deno. This enables writing both the front-end user interface and back-end server of a website in the same language. With the transition from Web1.0 to Web2.0, front-end libraries such as ReactJs and Angular started to be used. <sup>[\[3\]](#k3)</sup> <sup>[\[4\]](#k4)</sup> <sup>[\[5\]](#k5)</sup>

React is a component-based library developed by Meta (Facebook). It uses a language called JSX, a combination of JavaScript and HTML. JSX code is converted to HTML and JavaScript by React. React components are combined with a tree structure to create user interfaces. Components manage their internal states and can communicate with other components through props and callback functions. Props transfer information from parent components to child components, while callback functions enable information transfer from child components to parent components. Any change in the internal state of a component leads to its re-rendering as well as the re-rendering of its child elements. <sup>[\[6\]](#k6)</sup>

Since coins will be active in the game, we can also mention the structure of the coin. The purpose of the coin is to offer an alternative using a decentralized peer-to-peer transaction system, contrasting with the centralized transaction system dependent on major financial institutions. The ledger where transactions are added is shared with users, allowing the security of transactions to be confirmed. Since Bitcoin uses the proof-of-work mechanism, blocks are "mined," and those who mine the blocks are called "miners." At the core of the proof-of-work mechanism is relying on the computer that has spent the most computing power. 

Combining all these technological components, the Slide It! ecosystem, where you play to earn, has been created.

## <a name="_toc106213989"></a><a name="_toc106214125"></a><a name="_toc106214177"></a>**1.1 PROBLEM STATEMENT**
Play to Earn translates to "kazanmak için oyna" in Turkish and signifies a new video game ecosystem. In traditional video games, the goal of game studios has been to maximize profits from players. This has led to the introduction of the Pay-to-Win system in multiplayer online games, where players contributing financially to the game are rewarded with in-game advantages. Play-to-Earn games, on the other hand, involve players in the economy of the game, allowing them to earn money while playing.

The Play-to-Earn system is currently used in many NFT and metaverse games. Users accumulate tokens and NFTs that can be converted into real money as they play the game. The Slide It! project is designed with the goal of creating a structure where both the developers and players can earn. <sup>[\[7\]](#k7)</sup>

## <a name="_toc106213990"></a><a name="_toc106214126"></a><a name="_toc106214178"></a>**1.2 MOTIVATION**
Play-to-earn games reward participants with digital cash or tokens without value. In recent years, these blockchain-supported games, also known as P2E, have become mainstream and an essential component of almost every metaverse.

Typically, each platform has its own cryptocurrency format to pay online players for their time commitment. Earning real-world currency while having fun is a significant plus for players. In traditional games, there is no incentive to play other than pure entertainment. The relationship is one-way: you pay to play the game, and unless you are a professional esports player or a streamer with a large following, you can never earn money from your game time.

In contrast, blockchain games offer players the opportunity to earn real money. Simply put, play-to-earn games are video games where players can receive rewards in real-world value. While people have been making money by playing video games for years through practices like "gold farming" and unofficial marketplaces for in-game items, the emergence of blockchain technology and NFTs has literally transformed the gaming industry.

NFTs, or non-fungible tokens, are cryptographically unique tokens that can be used to prove ownership of content such as images or music. In blockchain games, they enable users to own in-game items like virtual clothing or pieces of land. Non-fungible tokens or NFTs are digitally unique assets whose uniqueness is proven by cryptography. They can be used to represent both tangible and intangible items. The game's mobility, superior selection of appropriate technologies, and a play-to-earn and blockchain approach make it a current, innovative, and potentially marketable project.

# <a name="_toc106213991"></a><a name="_toc106214127"></a><a name="_toc106214179"></a>**LITERATURE REVIEW**
## <a name="_toc106213992"></a><a name="_toc106214128"></a><a name="_toc106214180"></a>**2. LITERATURE REVIEW**
The Slide It project has been created by taking examples from the works of competitors in the industry. It significantly resembles other projects currently in the sector, which does not provide diversity for users. For instance, these projects do not provide mobile support, and users can only play their games on the projects' websites. This is not a suitable process for the modern world, given the significantly increasing use of mobile devices.

To discuss these projects, we need to look at projects that have made a mark in the industry and achieved sustainability. For example, looking at the Axie Infinity project and its coin, AXS, Axie Infinity is a game inspired by Pokémon, where individuals can earn tokens by contributing to the ecosystem and showcasing their gaming skills.

Players can battle for their pets, collect items, upgrade them, and establish a land-based kingdom. All game data and Axie genetic data are easily accessible to third parties, allowing community developers to create their tools and experiences in the Axie Infinity universe. Axie Infinity is a blockchain-based trading and battling game partially owned and operated by players.

Inspired by popular games like Pokémon and Tamagotchi, Axie Infinity allows players to collect, breed, upgrade, battle, and trade token-based creatures known as Axies. Axies can take various forms, and there are over 500 different body parts, including aquatic, beast, bird, bug, plant, and reptile sections.

Despite being in early access at the moment, Axie is ranked as the number one Ethereum game by daily, weekly, and monthly active users. Axie has earned over 6,400 ETH (2 million+ USD) to date. Besides being a fun game, Axie has taken on the features of a social network and business platform due to its strong community and rapid success. The fundamental difference between Axie and a regular game is the use of blockchain economic design to reward players for their contributions to the ecosystem.

This new game model is called "play-to-earn." Axie has attracted thousands of players from developing countries seeking a new income stream during the Covid pandemic. Many of these players, previously unfamiliar with blockchain technology, include not only fathers, aunts, and even grandparents.

The winning side can upgrade an Axie's statistics or improve body parts by earning more experience points. Axies can be combined to produce new and unique offspring that can be used or sold on the Axie market.

The Axie Infinity ecosystem also has its unique governance tokens called Axie Infinity Shards (AXS). These are used to participate in key governance votes and give owners a say in how funds in the Axie Community treasury will be spent.[<sup>\[8\]</sup>](#k8)

It is also possible to provide examples of unsuccessful project cases in the play-to-earn style. For instance, Smooth Love Potion (SLP) is an ERC-20 based utility token used in the Axie Infinity (AXS) ecosystem.

Axie Infinity (AXS) is currently one of the most popular metaverse NFT games. Designed in the play-to-earn model, the game is created by drawing inspiration from popular games like Pokémon and Tamagotchi.

Launched by Sky Mavis in 2018, Axie Infinity is a game where we collect and develop cute digital creatures called Axies, making them fight each other.

Each Axie is also an ERC-721-based NFT. Players can collect Smooth Love Potion (SLP) tokens by battling with their Axies and completing tasks, which they can then convert into fiat currency.

In fact, Smooth Love Potion (SLP) is one of the two tokens in the Axie Infinity game. The governance token of the game is the AXS token. The SLP token serves as a utility token used in the game.

Smooth Love Potion (SLP) is the cryptocurrency used to enhance characters called Axies in the Axie Infinity (AXS) game. In this respect, SLP tokens are similar to experience points in many games. SLP tokens can be earned by playing the Axie Infinity game. Users can also choose to sell their SLP tokens for fiat currency on cryptocurrency exchanges.

In the game, Axies can be upgraded seven times. Development costs start at 100 SLP tokens and increase each time: the second development requires 200 SLP, the third development 300 SLP, the fourth development 500 SLP, the fifth development 800 SLP, the sixth development 1,300 SLP, and the seventh development 2,100 SLP.<sup>[[9\]</sup>](#k9)

The Slide It project has been developed by examining the advantages and disadvantages of competitors in the industry and aims to provide concrete answers to questions users might have by observing the playing styles of their competitors. The project does not approach this merely as a gaming logic but also as an evaluation of shortcomings to keep the coin value high in line with the logic of winning projects.


# <a name="_toc106213993"></a><a name="_toc106214129"></a><a name="_toc106214181"></a>**METHOD**
## <a name="_toc106213994"></a><a name="_toc106214130"></a><a name="_toc106214182"></a>**3. METHOD**
The Slide It! project involves multiple systems. During the phase of determining both the website and the technologies for the game, an extensive market research and evaluation of options stage was conducted.

## <a name="_toc106213995"></a><a name="_toc106214131"></a><a name="_toc106214183"></a>**3.1 METHODS USED IN GAME DEVELOPMENT**
The Unity game engine was chosen as the game engine and development environment for developing the game. The reason for selecting this game engine is its user-friendly development interface, easy integration of plugins and services, easy access for developers to extensions called assets through the Unity Asset Store, and its compatibility with the C# language. Additionally, the community support is greater compared to other game development environments.

![Unity Interface](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.001.png)
*Screenshot 1: Unity Interface*

![Visual Studio Interface](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.002.png)
*Screenshot 2: Visual Studio 2022 Interface*

Every script in the game, including the core drift mechanics, was written using Visual Studio 2022, which integrates seamlessly with Unity.

# Assets

The "ACC (Arcade Car Controller)" asset was purchased from the Asset Store and integrated into the game for the core drift mechanics. Additionally, the main menu template from the same asset was used for the main menu.

![ACC Asset](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.003.png)

*Screenshot 3: Unity Asset Store ACC Asset*
---
The Modern UI Pack Asset was used for some interface elements (input field, modal window, button). This asset was acquired for free.

The "STYLIZED: Complete Drift Cars" asset was purchased for the cars that will be used and sold in the game. This asset includes 17 car models, and the models were added to the game using the "Add car to game" panel of the ACC asset.
---
![Car Asset](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.005.png)

*Screenshot 4: Asset Store Car Asset*
---
![Car Adding Panel](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.004.png)

*Screenshot 5: Car Adding Panel*
---
![Importing Asset](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.006.png)

*Screenshot 6: Asset Import Screen*
---
![Login Screen Hierarchy](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.007.png)

*Screenshot 7: Login Screen Hierarchy*
---
![Login Screen](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.008.jpeg)

*Screenshot 8: Login Screen*
---
![Main Screen Hierarchy](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.009.png)

*Screenshot 9: Main Screen Hierarchy*
---
![Main Screen](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.010.jpeg)

*Screenshot 10: Main Screen*
---
Due to time constraints, a custom map was not added to the game, and existing maps in the ACC asset were used.

![Select Map Screen](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.011.jpeg)

*Screenshot 11: Map Selection Screen*
---
![Select Car Screen](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.012.png)

*Screenshot 12: Car Selection Screen*
---
![Gameplay Screenshot](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.013.png)

*Screenshot 13: Gameplay Screenshot*
---
Game data (username, user's money, score, etc.) is currently stored in a local database provided by Unity called PlayerPrefs. The desired future step is to integrate the Firebase Realtime Database into the game to retrieve data from the user who registered through our website and write the game data to the database.

![Database Connection Method](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.014.png)

*Screenshot 14: Method for Database Connection*
---
![Fetching User Data](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.015.png)

*Screenshot 15: Fetching User Data from Database & User Authentication*
---
![Fetching Money Data](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.016.png)

*Screenshot 16: Fetching Money Data from Database*
---
![Writing Username to Game](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.017.png)

*Screenshot 17: Writing Username to Game*
---
![PlayerPrefs Methods](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.018.png)

*Screenshot 18: PlayerPrefs Methods*
---
## <a name="_toc106213996"></a><a name="_toc106214132"></a><a name="_toc106214200"></a>**3.2 METHODS USED IN THE DEVELOPMENT OF THE WEBSITE**
To develop the website, a template named "NetStorm -NFT Marketplace" was purchased from ThemeForest, prepared with ReactJs. The template proved challenging initially due to unclear descriptions and documentation, but the development process became smoother over time.

![Template Preview](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.019.png)

*Screenshot 19: Template Preview on the Store*
---
The template employs an inheritance logic, requiring locating the file of the inherited section to make changes, followed by observing the desired page for modifications. Additionally, there is a local database within the template for storing certain data, leading to the necessity of tracking a separate database. Understanding the template's core logic took some time, but eventually, a presentation-ready web page emerged.

The entire project was uploaded to GitHub as private, and development work was done in Visual Studio Code.

Basic JavaScript and CSS codes were used in the development of the web page.

![GitHub Repository](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.020.png)

*Screenshot 20: GitHub Repository of the Web Page*
---
![Home Page](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.021.png)

*Screenshot 21: Web Page - Home Page*
---
![News Page](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.022.png)

*Screenshot 22: Web Page - News Page*
---
![Front-End Development of the Home Page](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.023.png)

*Screenshot 23: Front-End Development of the Home Page*
---
![Wallet Integration Method](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.024.png)

*Screenshot 24: Wallet Integration Method*
---
Another template named "Vision UI Dashboard" was used for users to perform transactions and register. This template is also written in ReactJs and integrated with Firebase Realtime Database.

![Template Preview](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.025.png)
*Screenshot 25: Template Preview*
---
The homepage of this template is currently static.

![Static Interface](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.026.png)

*Screenshot 26: Static Interface*
---
The Firebase Realtime Database method is present in the user registration section. Through this method, user information, along with a unique key, is written to the database via a form.

![User Registration](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.027.png)

*Screenshot 27: User Registration Screen and Form*
---
![Firebase Configuration File](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.028.png)

*Screenshot 28: Firebase Configuration File*
---
![Importing Firebase into the Project](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.029.png)

*Screenshot 29: Importing Firebase into the Project and Defining Input Components*
---
![Defining Components](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.030.png)

*Screenshot 30: Defining Components for Inputs and Button*
---
![Component Definitions](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.031.png)

*Screenshot 31: Method for Database Registration*
---
![Firebase Realtime Database Interface](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.ab673a4a-99af-4915-9591-61bf4090cf5b.032.png)

*Screenshot 32: Firebase Realtime Database Interface*
---
## <a name="_toc106213997"></a><a name="_toc106214133"></a><a name="_toc106214216"></a>**RESULTS AND DISCUSSION**
### <a name="_toc106213998"></a><a name="_toc106214134"></a><a name="_toc106214217"></a>**4. RESULTS AND DISCUSSION**
As a result of the conducted work, the front-end development of the Slide It! project's website is complete.

The back-end development includes completed methods for user registration and data writing, while methods for retrieving user data are still in progress. Additionally, some modules envisaged to be added to the website (e.g., swap feature, display of game data) are currently unfinished.

Slide Coin has been minted in the Avalanche network, totaling 1 billion coins.

The game part of the Slide It! project is playable. Users can log into the game with their registered accounts, but user data (money amount, score) from the database is not displayed in the game. Currently, the game data is stored in the local database provided by the Unity game engine, called PlayerPrefs. The desired state is to write this data to the Firebase Realtime Database. Methods for reading data from the database have been written, and once some errors are resolved, they are ready to be replaced with local database methods.

The game, however, can be played smoothly. Users can earn in-game currency by drifting, purchase cars and maps with their money. However, currently, in-game currency cannot be exchanged for Slide Coin. Additionally, the Marketplace section is currently not functioning. Although the inventory section does not appear in a single area, users can view the assets (maps, cars) they own on the car selection and map selection screens.

The development of the game will continue in the future. If necessary, the website infrastructure can be further strengthened, and development can continue with a larger team.

# <a name="_resources"></a><a name="_toc106213999"></a><a name="_toc106214135"></a><a name="_toc106214218"></a>**RESOURCES**

<a name="k1"></a><sup>[1]</sup>Erdem, Feyza. “Why Are Mobile Games on the Rise?” Technotoday, October 19, 2021. [Source](https://technotoday.com.tr/mobil-oyunlar-neden-bu-kadar-yukseliste/). [Accessed June 14, 2022]

<a name="k2"></a><sup>[2]</sup>Unity (Game Engine). Wikipedia. Wikimedia Foundation, April 5, 2022. [Source](https://en.wikipedia.org/wiki/Unity_(game_engine)). [Accessed June 14, 2022]

<a name="k3"></a><sup>[3]</sup>JavaScript history. (n.d.). [Source](https://www.w3schools.com/js/js_history.asp). [Accessed June 14, 2022]

<a name="k4"></a><sup>[4]</sup>Delaney, J. (2019, June 20). *The weird history of JavaScript*. DEV Community. [Source](https://dev.to/codediodeio/the-weird-history-of-javascript-2bnb). [Accessed June 14, 2022]

<a name="k5"></a><sup>[5]</sup>Node.js. (n.d.). *About*. Node.js. [Source](https://nodejs.org/en/about/). [Accessed June 14, 2022]

<a name="k6"></a><sup>[6]</sup>Orcuntuna. (n.d.). *Orcuntuna/React-TURKCE-Kaynak: React.js öğrenmek için kullanabileceğiniz ücretsiz Türkçe Kaynak.*GitHub. [Source](https://github.com/orcuntuna/react-turkce-kaynak). [Accessed June 14, 2022]

<a name="k7"></a><sup>[7]</sup> "What Are Play-to-Earn Games? How Do Players Earn Money with NFTs?" [Source](https://www.coinkolik.com/oyna-kazan-oyunlari-nelerdir-oyuncular-nftlerle-nasil-para-kazaniyor/). [Accessed June 14, 2022]

<a name="k8"></a><sup>[8]</sup> Axie Infinity (AXS) Nedir?, Bitlo, Bitlo, [Source](https://www.bitlo.com/rehber/axie-infinity-axs-nedir). [Accessed June 14, 2022]

<a name="k9"></a><sup>[9]</sup> Smooth Love Potion (SLP) Nedir?, Bitlo, Bitlo, [Source](https://www.bitlo.com/rehber/smooth-love-potion-slp-nedir). [Accessed June 14, 2022]


