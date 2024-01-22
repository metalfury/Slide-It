# **Table of Contents**
[I. Project Definition](#_toc94390974)

[1. General Overview of the Project](#_toc94390975)

[2. Project Purpose](#_toc94390976)

[3. Project Scope](#_toc94390977)

[4. Product Scenarios](#_toc94390978)

[5. Constraints](#_toc94390979)

[6. Definitions](#_toc94390980)

[II. Requirements Analysis](#_toc94390981)

[7. Use Cases and Table Descriptions](#_toc94390982)

[8. Functional Requirements](#_toc94390983)

[III. Design Documentation](#_toc94390984)

[9. Definition of Design Objectives](#_toc94390985)

[10. Proposed Software Architecture](#_toc94390986)

[11. Class Diagrams](#_toc94390987)

[12. Dynamic Model](#_toc94390988)

[13. Subsystem Decomposition](#_toc94390989)

[14. User Interface](#_toc94390990)

[IV. Test Plans](#_toc94390991)

[15. Testable and Untestable Features](#_toc94390992)

[16. Successful/Unsuccessful Test Evaluation Criteria](#_toc94390993)

[17. Test Cases](#_toc94390994)

[V. Glossary](#_toc94390995)

# **PROJECT MEMBERS**
**Ömer Faruk Can DOĞRUSOY**
**Hüseyin KARAOĞLAN**
**Mert Ömer ŞENER**

# <a name="_toc94306043"></a><a name="_toc94390974"></a>**I. Project Definition**
## <a name="_toc94305650"></a><a name="_toc94305770"></a><a name="_toc94305881"></a><a name="_toc94306044"></a><a name="_toc94390975"></a>**1. General Overview of the Project**
Our project is a "Blockchain-Based Play to Earn Mobile Game." The system operates on the concept of "earning in-game currency by drifting in the game and exchanging it with real cryptocurrency, Slide Coin."

## <a name="_toc94305651"></a><a name="_toc94305771"></a><a name="_toc94305882"></a><a name="_toc94306045"></a><a name="_toc94390976"></a>**2. Project Purpose**
Our team's purpose in choosing this project is to establish a presence in the popular blockchain technology of today. The in-game currency will be a cryptocurrency that we create ourselves, named Slide Coin. The game will be a drifting game, where players earn in-game currency by drifting. The game will feature a market, marketplace, and inventory system. The market will sell cars and tracks, and the marketplace will facilitate the buying and selling of cars in an ecosystem. The prices of cars in the market will not be fixed; they can fluctuate based on demand. Tracks sold in the market will have fixed prices, with both free and paid versions.

## <a name="_toc94305652"></a><a name="_toc94305772"></a><a name="_toc94305883"></a><a name="_toc94306046"></a><a name="_toc94390977"></a>**3. Project Scope**
3a. Current Situation

There are similar games in the market, but most of them are computer-based. Slide It! is playable on mobile devices.

3b. Project Content

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.001.jpeg)

**Figure 3.1: "Component" diagram for the Slide It! project**

3c. Comparison with Competing Products

There is no mobile-based play-to-earn game in existing systems. This gap limits the ecosystem to a specific audience. Our goal is to increase accessibility.

## <a name="_toc94305653"></a><a name="_toc94305773"></a><a name="_toc94305884"></a><a name="_toc94306047"></a><a name="_toc94390978"></a>**4. Product Scenarios**
As developers, we plan to create a cryptocurrency called Slide Coin. For Slide Coin to gain value in the market, it needs demand and usage in trading. Players and traders are essential for creating this circulation. Players create an account on our website, where they can then log in to the game. After logging in, they can earn in-game currency and use it for in-game transactions or convert it into Slide Coin by creating a withdrawal request.

The game includes a market and a marketplace system. In the marketplace, users can buy and sell cars. Users can purchase cars from the game market, buy cars from other players, and sell cars from their inventory. However, cars purchased from the game market only provide visual enhancements. Additionally, players can buy maps from the game market to earn in-game currency more easily.

## <a name="_toc94305654"></a><a name="_toc94305774"></a><a name="_toc94305885"></a><a name="_toc94306048"></a><a name="_toc94390979"></a>**5. Constraints**
**Performance and Scalability:** If the system experiences high traffic, it may become unstable. Transfers could be delayed, and cybersecurity attacks might occur.

**Security:** Security measures on mobile devices are limited compared to computer systems, posing potential security issues.

**Reliability:**
- Users may initially distrust the system, perceiving it as a potential scam.
- If issues are not addressed promptly, user trust may be lost, leading to project failure.

## <a name="_toc94305655"></a><a name="_toc94305775"></a><a name="_toc94305886"></a><a name="_toc94306049"></a><a name="_toc94390980"></a>**6. Definitions**
GC – Game coin: In-game currency

SC – Slide coin: Cryptocurrency created for the project

k.page – User Page: A page where users can view information after logging in.

k. name: User Name

g. auth: Google Authenticator

# <a name="_toc94306050"></a><a name="_toc94390981"></a>**II Requirements Analysis**

## <a name="_toc94305656"></a><a name="_toc94305776"></a><a name="_toc94305887"></a><a name="_toc94306051"></a><a name="_toc94390982"></a>**7 Use Cases and Table Descriptions**

**Use Case Diagrams for the Website**

![Figure 1: Website Viewing](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.002.jpeg)

**Figure 1:** Website Viewing

**Table 1:**

| Use Case       | Main Page Use Case                                      |
| -------------- | ------------------------------------------------------- |
| Pre-Condition  | -                                                       |
| Post-Condition | Page is displayed                                       |
| Basic Path     | User can view the main page as soon as they connect to the website. |
| Alternative Path | -                                                     |
| Exceptional Path | - User cannot view the main page if the web server has crashed. - User cannot view the main page in case of any authorization error. |

![Figure 2: Website Registration](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.003.jpeg)

**Figure 2:** Website Registration

**Table 2:**

| Use Case       | Register Use Case                                       |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | User must not be registered.                             |
| Post-Condition | User registers in the system.                            |
| Basic Path     | - User selects a username. - User selects a password. - User selects a number. - User selects an email address. - These values are queried in the database. If not present, the process continues. - A code is sent to the user via message for number verification. The user proceeds to the email verification step by entering the code. - For email verification, a code is sent to the user via email. The user completes the registration process by entering the code. - The system registers the user in the database. |
| Alternative Path | - If any user data is already present in the database, the system throws an error. - If number and email are not verified, the system throws an error. |
| Exceptional Path | - Number Verification System may encounter an error during verification. - Mail Verification System may encounter an error during verification. |

![Figure 3: Website Login](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.004.jpeg)

**Figure 3:** Website Login

**Table 3:**

| Use Case       | Login Use Case                                          |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | Registered                                               |
| Post-Condition | Logged into the system                                   |
| Basic Path     | - Registered user first enters the username. - If the username is correct, the password entry area opens. The user enters the password. - If the password is correct, the user is asked to enter the Google Authenticator code. - If the Google Authenticator code is correct, the user is redirected to the main page with a logged-in session. |
| Alternative Path | - If the user enters the username incorrectly, they cannot proceed to the password entry area. - If the user enters the password incorrectly, they can use the password reminder system to recall the password, but they cannot proceed to the Google Authenticator step. - If the user enters the correct username and password but does not enter the Authenticator code, they cannot enter the system. |
| Exceptional Path | - If there is an issue with the database, the login process does not take place. - If Google Authenticator does not work, the login process does not take place. - If the Mail Verification system does not work properly, the login process does not take place. |

![Figure 4: View User Page](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.005.jpeg)

**Figure 4:** View User Page

**Table 4:**

| Use Case       | View User Page                                          |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | User must be logged in.                                  |
| Post-Condition | - User can withdraw balance. - User can link a wallet. - User can deposit balance. - User can buy Slide Coin. - User can log out. |
| Basic Path     | - |
| Alternative Path | - |
| Exceptional Path | User cannot view the user page if not logged in. |

![Figure 5: Withdraw Balance](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.006.jpeg)

**Figure 5:** Withdraw Balance

**Table 5:**

| Use Case       | Withdraw Balance                                        |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | - User must be logged in. - User must be viewing the user page. - User must have linked their wallet. - User must have created a withdrawal request in the game. |
| Post-Condition | User converts in-game currency to Slide Coin based on the game's request. |
| Basic Path     | - User creates a withdrawal request from the game. - Later, the user logs in to the website's user operations page. - Views the requests. - Confirms the request. - Both game and user balances are updated. |
| Alternative Path | User can cancel the request. |
| Exceptional Path | - **If the user has no balance in the game, they cannot create a request.** - **If the user is not logged in, they cannot view the user page.** |

![Figure 6: Deposit Balance](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.007.jpeg)

**Figure 6:** Deposit Balance

**Table 6:**

| Use Case       | Deposit Balance                                        |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | - User must be logged in. - User must be viewing the user page. - User must have linked their wallet. |
| Post-Condition | User securely deposits balance through the wallet provider. |
| Basic Path     | - User enters the deposit area. - Links their wallet. - Deposits money through the wallet provider. - Balance is updated. |
| Alternative Path | If the user has already linked their wallet, they can directly deposit money. |
| Exceptional Path | - **If the wallet account cannot be linked, the process cannot be completed.** - **If communication with the database cannot be established, the deposited money will not be credited.** |

![Figure 7: Link Wallet Account](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.008.jpeg)

**Figure 7:** Link Wallet Account

**Table 7:**

| Use Case       | Link Wallet Account                                    |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | - User must be logged in. - User must be viewing the user page. - User must have one wallet account. |
| Post-Condition | User links the wallet account.                           |
| Basic Path     | User directly links a wallet from any registered wallet provider in our system. |
| Alternative Path | - |
| Exceptional Path | - **If the user does not have a wallet account, they cannot perform the linking process.** |

![Figure 8: Buy Slide Coin](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.009.jpeg)

**Figure 8:** Buy Slide Coin

**Table 8:**

| Use Case       | Buy Slide Coin                                          |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | - User must be logged in. - User must be viewing the user page. - User must have linked their wallet. |
| Post-Condition | User buys Slide Coin through the wallet provider.         |
| Basic Path     | - User buys Slide Coin through the wallet provider. - Balance is updated. |
| Alternative Path | If the user has already linked their wallet, they can directly deposit money. |
| Exceptional Path | - **If the wallet account cannot be linked, the process cannot be completed.** - **If communication with the database cannot be established, the purchased amount will not be credited.** |

![Figure 9: Log Out](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.010.jpeg)

**Figure 9:** Log Out

**Table 9:**

| Use Case       | Log Out                                                |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | - User must be logged in. - User must be viewing the user page. |
| Post-Condition | User logs out of the system.                             |
| Basic Path     | - User enters the user page. - Presses the logout button. - Logout process takes place. |
| Alternative Path | - |
| Exceptional Path | - |

![Figure 10: Check Username](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.011.jpeg)

**Figure 10:** Check Username

**Table 10:**

| Use Case       | Check Username                                         |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | User must have entered a username.                      |
| Post-Condition | Username is queried in the database.                     |
| Basic Path     | - User enters a username to register. - Database queries the entered username. |
| Alternative Path | - |
| Exceptional Path | **If the username exists in the database, a negative response is sent to the user.** |

![Figure 11: Check Email Address](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.012.jpeg)

**Figure 11:** Check Email Address

**Table 11:**

| Use Case       | Check Email Address                                    |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | User must have entered an email address.                |
| Post-Condition | Email address is queried in the database.               |
| Basic Path     | - User enters an email address to register. - Database queries the entered email address. |
| Alternative Path | - |
| Exceptional Path | **If the email address exists in the database, a negative response is sent to the user.** |

![Figure 12: Verify Email Address](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.013.jpeg)

**Figure 12:** Verify Email Address

**Table 12:**

| Use Case       | Verify Email Address                                   |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | - User must have entered an email address. - Database must have queried the email address. |
| Post-Condition | Email address is verified.                              |
| Basic Path     | - User enters the email address. - Database queries the email address. - Email verification system sends a code to the email address. - User enters this code into the verification service. |
| Alternative Path | - |
| Exceptional Path | - **If the code is not sent to the email, the process cannot be completed.** - **If the email verification system is not working, the process cannot be completed.** |

![Figure 13: Check Phone Number](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.014.jpeg)

**Figure 13:** Check Phone Number

**Table 13:**

| Use Case       | Check Phone Number                                     |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | User must have entered a phone number.                  |
| Post-Condition | Phone number is queried in the database.                |
| Basic Path     | - User enters a phone number to register. - Database queries the entered phone number. |
| Alternative Path | - |
| Exceptional Path | **If the phone number exists in the database, a negative response is sent to the user.** |

![Figure 14: Verify Phone Number](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.015.jpeg)

**Figure 14:** Verify Phone Number

**Table 14:**

| Use Case       | Verify Phone Number                                    |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | - User must have entered a phone number. - Database must have queried the phone number. |
| Post-Condition | Phone number is verified.                               |
| Basic Path     | - User enters the phone number. - Database queries the phone number. - Phone verification system sends a code to the phone number. - User enters this code into the verification service. |
| Alternative Path | - |
| Exceptional Path | - **If the code is not sent to the phone, the process cannot be completed.** - **If the phone verification system is not working, the process cannot be completed.** |

![Figure 15: Save to Database](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.016.jpeg)

**Figure 15:** Save to Database

**Table 15:**

| Use Case       | Save to Database                                       |
| -------------- | -------------------------------------------------------- |
| Pre-Condition  | - User must have entered a username. - Username must have been checked. - User must have entered a password. - User must have entered an email address. - Email address must have been checked. - Email address must have been confirmed. - User must have entered a phone number. - Phone number must have been checked. - Phone number must have been confirmed. |
| Post-Condition | Data is encrypted and saved in the database.             |
| Basic Path     | \*\*For security reasons, each data is individually encrypted.\*\* - Checked username is saved in the database and encrypted using the encryption system. - Checked password is saved in the database and encrypted using the encryption system. - Confirmed email address is saved in the database and encrypted using the encryption system. - Confirmed phone number is saved in the database and encrypted using the encryption system. |
| Alternative Path | -
|Exceptional Path|<p>If the encryption system fails, the registration process cannot be completed.</p><p>If any saving operation cannot be performed, the registration process cannot be completed.</p>|

**Use Case Diagrams for the Game**

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.017.jpeg)
**Figure 16:** Game Main Screen

**Table 16:**

| Use Case          | Game Main Screen                                  |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | -                                                 |
| Post-Condition    | Player views the initial login screen.            |
| Basic Path        | - Player enters the game.                         |
|                   | - Views the main screen.                          |
| Alternative Path  | -                                                 |
| Exceptional Path  | **If there are issues on the servers, the player cannot connect to the game.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.018.jpeg)
**Figure 17:** Go to Game Main Screen

**Table 17:**

| Use Case          | Go to Game Main Screen                             |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | Player must be logged in.                          |
| Post-Condition    | Player views the game main screen.                |
| Basic Path        | - Player enters the game.                         |
|                   | - Clicks on the main screen from the home page.   |
| Alternative Path  | -                                                 |
| Exceptional Path  | -                                                 |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.019.jpeg)
**Figure 18:** Start the Game

**Table 18:**

| Use Case          | Enter the Game                                    |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Each player is given 1 starting car and 1 starting map. |
|                   | - Player must be logged in.                       |
|                   | - Player must have at least 1 map.               |
|                   | - Player must have selected a map.               |
|                   | - Player must have at least 1 car.               |
|                   | - Player must have selected a car.               |
| Post-Condition    | Player starts the game.                           |
| Basic Path        | - Player clicks on the start game button.         |
|                   | - Selects a map. Opens the car selection area.    |
|                   | - Chooses a car. Opens the enter game area.      |
|                   | - Begins the game.                                |
| Alternative Path  | -                                                 |
| Exceptional Path  | - **If the player does not select a map, they cannot start the game.** |
|                   | - **If the player selects a map but does not choose a car, they cannot start the game.** |
|                   | - **If the player selects a map and a car but chooses not to enter the game, they cannot start the game.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.020.jpeg)
**Figure 19:** Select Map

**Table 19:**

| Use Case          | Select Map                                        |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
| Post-Condition    | Player proceeds to car selection screen.          |
| Basic Path        | - Player enters the map selection screen.         |
|                   | - Directed to the inventory to choose the map.    |
|                   | - Selection is completed.                         |
| Alternative Path  | - Player can go to the game market to buy a map.  |
| Exceptional Path  | **If the player does not select a map, they cannot proceed to the car selection screen.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.021.jpeg)
**Figure 20:** Select Car

**Table 20:**

| Use Case          | Select Car                                        |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
| Post-Condition    | Player is ready to start the game.                |
| Basic Path        | - Player enters the car selection screen.         |
|                   | - Directed to the inventory to choose the car.    |
|                   | - Selection is completed.                         |
| Alternative Path  | - Player can go to the game market to buy a car.  |
|                   | - Player can go to the Marketplace.               |
| Exceptional Path  | **If the player does not select a car, they cannot start the game.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.022.jpeg)
**Figure 21:** Play

**Table 21:**

| Use Case          | Play                                              |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
| Post-Condition    | Player starts the game.                           |
| Basic Path        | - Player starts the game.                         |
|                   | - Earns in-game currency.                         |
|                   | - Database updates the player's balance.         |
| Alternative Path  | Player can return to the main menu without earning currency. |
| Exceptional Path  | **If the player crashes somehow, they cannot play the game.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.023.jpeg)
**Figure 22:** View Inventory

**Table 22:**

| Use Case          | View Inventory                                    |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
| Post-Condition    | Player views their inventory.                    |
| Basic Path        | - Player looks at their inventory.                |
|                   | - Sees car inventory and map inventory.           |
| Alternative Path  | - Player can view car inventory.                  |
|                   | - Player can view map inventory.                  |
|                   | - Player can go to the Marketplace.               |
|                   | - Player can go to the game market.               |
| Exceptional Path  | **If inventory data is inaccessible, the player cannot view their inventory.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.024.jpeg)
**Figure 23:** Enter the Game Market

**Table 23:**

| Use Case          | Enter the Game Market                              |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
| Post-Condition    | Player views the market.                          |
| Basic Path        | - Player enters the market.                       |
| Alternative Path  | - Player can buy a car.                           |
|                   | - Player can buy a map.                           |
|                   | - Player may choose not to buy anything.          |
| Exceptional Path  | - **If the player has no car and did not buy a car, they cannot start the game.** |
|                   | - **If the player has no map and did not buy a map, they cannot start the game.** |
|                   | **To prevent this, each player will be given one car and one starting map.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.025.jpeg)
**Figure 24:** Purchase Map from the Game Market

**Table 24:**

| Use Case          | Purchase Map                                      |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
|                   | - Player must have entered the market.            |
| Post-Condition    | Player purchases the map.                         |
| Basic Path        | - Player enters the market.                       |
|                   | - Buys the map.                                   |
|                   | - Adds to the cart.                               |
|                   | - If the balance is sufficient, makes the payment.|
|                   | - Map is added to the inventory.                 |
| Alternative Path  | - Player can check map details.                   |
|                   | - Player may choose not to buy anything.          |
| Exceptional Path  | **If the balance is insufficient, the transaction is not completed.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.026.jpeg)
**Figure 25:** Purchase Car from the Game Market

**Table 25:**

| Use Case          | Purchase Car                                      |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
|                   | - Player must have entered the market.            |
| Post-Condition    | Player purchases the car.                         |
| Basic Path        | - Player enters the market.                       |
|                   | - Buys the car.                                   |
|                   | - Adds to the cart.                               |
|                   | - If the balance is sufficient, makes the payment.|
|                   | - Car is added to the inventory.                 |
| Alternative Path  | - Player can check car details.                   |
|                   | - Player may choose not to buy anything.          |
| Exceptional Path  | **If the balance is insufficient, the transaction is not completed.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.027.jpeg)
**Figure 26:** Enter the Marketplace

**Table 26:**

| Use Case          | Enter the Marketplace                              |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
| Post-Condition    | Player enters the Marketplace.                    |
| Basic Path        | -                                                 |
| Alternative Path  | - Player can buy a car.                           |
|                   | - Player can sell a car.                          |
| Exceptional Path  | -                                                 |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.028.jpeg)

**Figure 27:** Purchase Car from the Marketplace

**Table 27:**

| Use Case          | Purchase Car from the Marketplace                  |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
|                   | - Player must have entered the Marketplace.      |
| Post-Condition    | Player purchases the car.                         |
| Basic Path        | - Player enters the Marketplace.                  |
|                   | - Buys the car.                                   |
|                   | - Adds to the cart.                               |
|                   | - If the balance is sufficient, makes the payment.|
|                   | - Car is added to the inventory.                 |
| Alternative Path  | - Player can check car details.                   |
|                   | - Player may choose not to buy anything.          |
| Exceptional Path  | - **If the player has never bought a car from the Marketplace, they cannot sell a car.** |
|                   | - **The player cannot sell a car without setting a price.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.029.jpeg)
**Figure 28:** Sell Car in the Marketplace

**Table 28:**

| Use Case          | Sell Car in the Marketplace                        |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
|                   | - Player must have entered the Marketplace.      |
| Post-Condition    | Player puts their owned car up for sale.           |
| Basic Path        | - Player enters the Marketplace.                  |
|                   | - Goes to the sell car section.                   |
|                   | - Sets the price.                                 |
|                   | - Lists the car for sale.                         |
| Alternative Path  | - Player may choose not to sell anything.         |
| Exceptional Path  | - **If the player has never bought a car from the Marketplace, they cannot sell a car.** |
|                   | - **The player cannot sell a car without setting a price.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.030.jpeg)
**Figure 29:** Withdraw Money

**Table 29:**

| Use Case          | Withdraw Money                                    |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
| Post-Condition    | Player creates a request to exchange in-game currency for Slide Coin. |
| Basic Path        | - Player enters the withdrawal section.           |
|                   | - Determines the amount to be exchanged.          |
|                   | - Database checks the balance.                    |
|                   | - System deducts the equivalent in-game currency from the player's balance. |
| Alternative Path  | -                                                 |
| Exceptional Path  | **If the player's balance is insufficient, the exchange request is not processed.** |

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.031.jpeg)
**Figure 30:** View Settings

**Table 30:**

| Use Case          | View Settings                                     |
| ----------------- | ------------------------------------------------- |
| Pre-Condition     | - Player must be logged in.                       |
| Post-Condition    | -                                                 |
| Basic Path        | - Player enters the game main screen.             |
|                   | - Player goes to the settings page.              |
| Alternative Path  | - Player can adjust audio settings.               |
|                   | - Player can change the game language.           |
|                   | - Player can log out.                            |
| Exceptional Path  | -                                                 |


## 8 Functional Requirements

### Table31: Web Page Problem Requirements Definition

| Section/ Requirement ID | Requirement Definition                                       |
| :---------------------- | :----------------------------------------------------------- |
| FR1.0                   | The system must display the main screen to the user.         |
| FR1.1                   | The system must display the login screen to the user.        |
| FR1.1.1                 | The system must display the username entry field to the user.|
| FR1.1.2                 | The system must display the password entry field to the user.|
| FR1.1.3                 | The system must display the Google authenticator code entry field to the user.|
| FR1.1.4                 | The system must redirect the user to the homepage.           |
| FR1.2.0                 | The system must display the registration screen to the user. |
| FR1.2.1                 | The system must prompt the user to enter a username.         |
| FR1.2.2                 | The system must prompt the user to enter a password.         |
| FR1.2.3                 | The system must prompt the user to enter an email address.    |
| FR1.2.3.1               | The system must send a code to the user's email address during the registration process.|
| FR1.2.4                 | The system must prompt the user to enter a phone number.     |
| FR1.2.4.1               | The system must send a code to the user's phone number during the registration process.|
| FR1.2.5                 | The system must add the user's information to the database in encrypted form.|
| FR1.3.0                 | The user must be able to view their user page correctly.      |
| FR1.3.1                 | The user must be able to view balance withdrawal requests.    |
| FR1.3.1.2               | The user must be able to perform balance withdrawal transactions.|
| FR1.3.2                 | The user must be able to deposit funds.                       |
| FR1.3.3                 | The user must be able to link a wallet account.               |
| FR1.3.4                 | The user must be able to purchase Slide Coins.               |
| FR1.3.5                 | The user must be able to log out.                            |

### Table32: Game Problem Requirements Definition

| Section/ Requirement ID | Requirement Definition                                       |
| :---------------------- | :----------------------------------------------------------- |
| FR2.0                   | The system must display the main screen to the player.       |
| FR2.1                   | The system must direct the player to the registration area.  |
| FR2.2                   | The system must prompt the player to log in.                 |
| FR2.2.1                 | The system must ask the player for the username and password used during registration.|
| FR2.3                   | The player must be able to view their inventory.              |
| FR2.4                   | The player must be able to view settings.                     |
| FR2.5                   | The player must be able to enter the Marketplace.             |
| FR2.5.1                 | The player must be able to buy a car.                         |
| FR2.5.2                 | The player must be able to sell a car.                        |
| FR2.5.2.1               | The player must be able to create a listing.                  |
| FR2.6                   | The player must be able to create a withdrawal request.       |
| FR2.7                   | The user must be able to start the game.                      |
| FR2.7.1                 | The system must prompt the player to select a map to start the game.|
| FR2.7.1.1               | The player must be able to buy a map from the game market.    |
| FR2.7.2                 | The system must prompt the player to select a car to start the game.|
| FR2.7.2.1               | The player must be able to buy a car from the game market.    |
| FR2.7.2.2               | The player must be able to buy a car from the Marketplace.    |
| FR2.7.3                 | The system must notify the player that they are ready to start the game.|
| FR2.8                   | The system must transfer the player to the game.             |
| FR2.9                   | The player must be able to earn game currency by playing the game.|
| FR2.9.1                 | The player must be able to exchange the earned money with Slide Coin.|
| FR2.9.2                 | The player must be able to spend the earned money in the game market or Marketplace.|
| FR2.9.3                 | The player must be able to close the game.                   |

# <a name="_toc94306053"></a><a name="_toc94390984"></a>#**III Design Documentation**

## <a name="_toc94305658"></a><a name="_toc94305778"></a><a name="_toc94305889"></a><a name="_toc94306054"></a><a name="_toc94390985"></a>**## 9 Definition of Design Goals**

** Well-defined Interfaces **

Blockchain is a highly complex technology. The primary goal of the Slide It! Project is to enable users to perform transactions without feeling this complexity. Therefore, users should be provided with a simple web user interface that is stripped of unnecessary features for them to carry out transactions. Additionally, an interface should be designed for the game, allowing users to easily adapt to the game when they open it and not get lost in the game menu.

** Adaptability **

The site and the game should be capable of taking action based on market trends. This is because the dynamics of the industry shift towards the current interest in the market. The blockchain ecosystem is vibrant. For example, in the current period, MetaVerse projects are quite popular. Our game and website should be able to undergo minor changes without losing their identity in line with these dynamics. For instance, when a topic becomes popular, extensions related to that topic should be added to the game. The game should not be monotonous and boring.

** User-friendliness **

The game and web ecosystem should be user-friendly. An individual with no prior knowledge should easily become a part of the system. Moreover, interruptions in financial transactions and in-game pricing should be controllable and suitable for users.

** Good Documentation **

To ensure the project's continuity, it is necessary to strategically structure the distribution of "tokenomics." A healthy distribution can create more demand by allocating the necessary budget to marketing. Also, there should be no "liquidity" issue to smoothly operate the "stake" part of the system. Otherwise, people will not want to invest in the project if they cannot get their returns. The correct coin distribution is the most important building block to sustain the project.

Documentation containing such information and outlining how the project will proceed should be presented to the user under the name "whitepaper." Users should be informed about the project without playing the game or making transactions with Slide Coin.

** Minimum Number of Errors **

There should be no errors on paper in the Slide It! Project. However, due to systemic issues, the number of errors should be kept to a minimum. Even the smallest error can cause irreversible financial damage to a user or the system. To avoid such consequences, the system must be created correctly.

## <a name="_toc94305659"></a><a name="_toc94305779"></a><a name="_toc94305890"></a><a name="_toc94306055"></a><a name="_toc94390986"></a>**##**10 Recommended Software Architecture**

In the Slide It! project, considering that users will have features such as inventory and assets, the "Entity Component System" software architecture is deemed appropriate. Another reason for using this architecture is its common use in games.

![Web Page Package Diagram](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.032.jpeg)

**Figure 31: Package Diagram for the Web Page**

- The user communicates with the "Presentation" package to interact with the System package.

- The user can use the "Buy Coin" or "Exchange Coin" packages in the System package.

- To perform all these operations, the "Payment Package" system is used.

- All transactions in the system are integrated with the "Data Management" package.

![Game Package Diagram](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.033.jpeg)

**Figure 32: Package Diagram for the Game**

- The player communicates with the "Presentation" package to interact with the System package.

- The user can use the "Earn Game Currency", "Shopping System", "Currency Exchange", "Inventory" packages in the System package.

- All transactions in the system are integrated with the "Data Management" package.

## <a name="_toc94305660"></a><a name="_toc94305780"></a><a name="_toc94305891"></a><a name="_toc94306056"></a><a name="_toc94390987"></a>**11 Sınıf Diyagramları**

**Web Sayfası İçin Sınıf Diyagramı**

![Web Page Class Diagram](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.034.jpeg)

**Figure 33: Class Diagram for the Web Page**

**Oyun İçin Sınıf Diyagramı**

![Game Class Diagram](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.035.jpeg)

**Figure 34: Class Diagram for the Game**


## <a name="_toc94305661"></a><a name="_toc94305781"></a><a name="_toc94305892"></a><a name="_toc94306057"></a><a name="_toc94390988"></a>**12 Dynamic Model**

In the Slide It! project, the dynamic model will be explained with "Sequence Diagrams."

### **Sequence Diagrams for the Web Page**

**Sequence Diagram 1: Log In**

![Sequence Diagram 1](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.036.jpeg)

The user enters their username for login. If the username is correct, the system grants permission to switch to the password window. The user enters the password. If the password is correct, the system asks the user to enter the Google Authenticator code. The user enters the authenticator code, and the system directs the user.

**Sequence Diagram 2: Sign Up**

![Sequence Diagram 2](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.037.jpeg)

The user enters the registration page. They choose a username. If the username has not been used before, the system grants permission to switch to the password window and asks to set a password. The user sets a password, and the password is saved in the system. Then, the system asks for a phone number. The user enters the phone number. If the number has not been used before, it proceeds to the confirmation step. If confirmed, it moves to entering the email address. The user enters the email address. If the email address has not been used before, it moves to the confirmation step. If confirmed, the database encrypts and saves all data. Then, the system redirects the user.

**Sequence Diagram 3: Withdraw Balance**

![Sequence Diagram 3](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.038.jpeg)

The user can see, approve, or reject notifications from the game. If the user approves any request, the exchange takes place, the balance is updated, and the request status is updated.

**Sequence Diagram 4: Deposit Balance**

![Sequence Diagram 4](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.039.jpeg)

The user creates a swap request. If the requested amount is in the balance, Slide Coin is converted to in-game currency, saved in the database, and can be viewed in the game.

**Sequence Diagram 5: Buy Slide Coin**

![Sequence Diagram 5](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.040.jpeg)

The user connects their wallet through the wallet provider to buy Slide Coin and creates a request. If there is enough balance, the Slide Coin balance is updated, and the transaction is completed.

**Sequence Diagram 6: Log Out**

![Sequence Diagram 6](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.041.jpeg)

The user presses the log out button. The system disconnects.

**Game-specific Sequence Diagrams**

**Sequence Diagram 7: Enter the Game**

![Sequence Diagram 7](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.042.jpeg)

The player enters the game and makes a login request to start the game. The game asks the user for an email address. If the email address is correct, the game asks the user to enter a password. If the password is correct, the user is directed to the game's main screen.

**Sequence Diagram 8: View Inventory**

![Sequence Diagram 8](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.043.jpeg)

The player creates a request to view the inventory. A query is made in the database, and inventory data is displayed.

**Sequence Diagram 9: Buy Car from Game Market**

![Sequence Diagram 9](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.044.jpeg)

The player creates a request to buy a car. The system asks for selecting a car. The player selects a car and makes a payment. If the balance is sufficient, the payment is completed, and the balance and inventory are updated.

**Sequence Diagram 10: Buy Map from Game Market**

![Sequence Diagram 10](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.045.jpeg)

The player creates a request to buy a map. The system asks for selecting a map. The player selects a map and makes a payment. If the balance is sufficient, the payment is completed, and the balance and inventory are updated.

**Sequence Diagram 11: Buy Car from Marketplace**

![Sequence Diagram 11](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.046.jpeg)

The user creates a request to buy a car. Car data is retrieved from the database. The user selects a car and makes a payment. If the balance is sufficient, the transaction is completed. The car database, user inventory, and balance are updated.

**Sequence Diagram 12: Sell Car on Marketplace**

![Sequence Diagram 12](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.047.jpeg)

The user creates a sale request. Inventory data for sale is displayed, and a car is selected. A price is set, and confirmation is requested. Once confirmed, the inventory and database are updated.

**Sequence Diagram 13: Start the Game**

![Sequence Diagram 13](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.048.jpeg)

The player presses the play button, and the system asks to select a map. The player wants to view the maps. Map data is retrieved, and a map is selected. Then, the player is asked to select a car. The player wants to view the cars, car data is retrieved, and a car is selected. After selection, the system directs the player to the game.

## <a name="_toc94390989"></a>**13 Subsystem Decomposition**

In the Slide It! project, Subsystem Decomposition has been schematized using a Deployment Diagram.

![Slide It Projesine Ait Deployment Diyagramı](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.049.jpeg)

**Figure: Deployment Diagram for Slide It! Project**

The user utilizes two subsystems within the Slide It! main system. These two systems are interconnected and inseparable.

The user engages with the game system through a mobile device interface. They can play the game to earn Game Coins and create exchange requests to swap them with Slide Coins. Additionally, the user can perform trading operations as an auxiliary subsystem to the game system.

For the Web Page system, the user accesses it through a web page interface over the internet. In this system, they can manage incoming requests or enhance Slide Coin balances.

## <a name="_toc94305662"></a><a name="_toc94305782"></a><a name="_toc94305893"></a><a name="_toc94306058"></a><a name="_toc94390990"></a>**14 User Interface**
Software used to prepare the UIs:

- Figma
- Adobe Xd
- Adobe Illustrator
- Adobe Photoshop

**\*Some of the game visuals are quoted for representational purposes as the game is not ready.**

![Web Page](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.050.png)

### 1. Home Page

![Registration Page (Username Entry)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.051.png)

### 2. Registration Pages
#### 2.1.1 Registration Page (Username Entry)

![Registration Page (Password Entry)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.052.png)

#### 2.1.2 Registration Page (Password Entry)

![Registration Page (Phone Number Entry & Confirmation)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.053.png)

#### 2.1.3 Registration Page (Mail Address Entry & Confirmation)

![Registration Page (Mail Address Entry & Confirmation)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.054.png)

#### 2.2 Registration Page (Completion & Redirection)

![Registration Page (Completion & Redirection)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.055.png)

### 2.2 Login Page
#### 2.2.1 Login Page (Mail and Password Entry)

![Login Page (Mail and Password Entry)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.056.png)

#### 2.2.2 Login Page (Google Authenticator)

![Login Page (Google Authenticator)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.057.png)

#### 2.2.3 Login Page (Completion & Redirection)

![Login Page (Completion & Redirection)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.058.png)

### 2.3 User Page

![User Page](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.059.png)

#### 2.3.1 Wallet Not Connected User Page (Coin Exchange Page)

![Wallet Not Connected User Page (Coin Exchange Page)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.060.png)

#### 2.3.2 Wallet Connection (Wallet Provider Screen)

![Wallet Connection (Wallet Provider Screen)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.061.png)

#### 2.3.3 Wallet Connected User Page (Coin Exchange Page)

![Wallet Connected User Page (Coin Exchange Page)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.062.png)

#### 2.3.4 Post-Exchange View

![Post-Exchange View](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.063.png)

#### 2.3.5 Wallet Page (Slide Coin Purchase)

![Wallet Page (Slide Coin Purchase)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.064.png)

#### 2.3.6 Post-Purchase View

![Post-Purchase View](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.065.png)

#### 2.3.7 Withdrawal Page (View and Process Requests from the Game)

![Withdrawal Page (View and Process Requests from the Game)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.066.png)

#### 2.3.7.1 Withdrawal Page (Additional Menu)

![Withdrawal Page (Additional Menu)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.067.png)

#### 2.3.8 Logout

![Logout](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.068.png)

**Game**

### 3.1 Game Entry Screen
![Game Entry Screen](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.069.png)

### 3.1.2 Game Login Screen
![Game Login Screen](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.070.png)

### 3.2 Game Main Screen (Representative)

![Game Main Screen (Representative)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.071.png)

### 3.2.1 Start Game (Select Map) (Representative)

![Start Game (Select Map) (Representative)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.072.png)

### 3.2.2 Start Game (Select Car) (Representative)

![Start Game (Select Car) (Representative)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.073.png)

### 3.3 Game View (Representative)

![Game View (Representative)](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.074.png)

*Representative images are quoted from the game "Horizon Chase," with additions made to the pictures.*

# <a name="_toc94306059"></a><a name="_toc94390991"></a>**Test Plans**
In this section, test plans related to the project are outlined.

In large software projects, software testing must be an integral part. During the product development process, it is essential to measure whether a part of the software performs its expected task. This is achievable through software testing.

Given that the Slide It! project involves both a website and game systems, testing is crucial and necessary. As our system needs to be "highly secure and reliable," regular tests and maintenance should be carried out. However, due to the extensive nature of our project, not every test may be feasible during the development phase. After conducting tests, maintenance tests will continue once our project goes live.

Our project includes:

Integration Tests as there will be multiple services.

Unit, Component, and Functional Tests to verify the correct functionality of modules.

Our main plan for the project is as follows:

Design and implement the website. Then, add modules, integrate systems and modules, conduct tests, and ensure that the system works as a whole.

For the game part, begin by designing and testing the game interface. Subsequently, integrate and test buying-selling and market modules into the game system. Finally, develop the playable part of the game and test the entire system.

Ultimately, release an "Alpha" version and conduct an "Acceptance Test" with end-users.

## <a name="_toc94305663"></a><a name="_toc94305783"></a><a name="_toc94305894"></a><a name="_toc94306060"></a><a name="_toc94390992"></a>**15 Testable and Non-Testable Features**

In this section, the constraints of the system that can be tested and those that cannot be tested are presented in tabular form.

**Table 15.1.2: Testable Subsystems/Features of the Slide It! Project's Game System**


| **TESTABLE ITEMS**             | **TEST SCENARIOS**                                          |
|---------------------------------|------------------------------------------------------------|
| **USER OPERATIONS**             | Test the ability to log into the game                      |
|                                |                                                            |
| **SYSTEM DATABASE**             | Test user control                                         |
|                                |                                                            |
| **GAME CONNECTION SYSTEM**      | Test the game's internet connectivity status              |
|                                |                                                            |
| **USER DATABASE**               | Test the ability to view the user's inventory              |
|                                |                                                            |
| **MARKET DATABASE**             | Test the visibility of items in the in-game market         |
|                                |                                                            |
| **MARKETPLACE DATABASE**        | Test the visibility of items in the marketplace            |
|                                |                                                            |
| **MARKETPLACE OPERATIONS**      | Test selling a car in the marketplace                      |
|                                |                                                            |
| **MARKETPLACE OPERATIONS**      | Test buying a car from the marketplace                     |
|                                |                                                            |
| **USER & SYSTEM DATABASE**      | Test balance updates after buying/selling transactions     |
|                                |                                                            |
| **USER & SYSTEM DATABASE**      | Test balance update after Slide Coin exchange              |
|                                |                                                            |
| **GAME SYSTEM**                 | Test the requirements for starting the game                |
|                                |                                                            |
| **GAME SYSTEM**                 | Test ownership of a car to start the game                  |
|                                |                                                            |
| **GAME SYSTEM**                 | Test ownership of a map to start the game                  |
|                                |                                                            |
| **GAME SYSTEM**                 | Test the playability of the game                           |
|                                |                                                            |

**Table 15.2: Non-Testable Subsystems/Features of Slide It! System**

| User Interface Design | Due to different resolutions on various devices, testing the design and appearance individually on each device is not feasible. |
| - | - |
| Wallet Addition and Purchase Transactions After | Since the "Slide Coin" is not yet available in the project phase, testing buying, selling, and swapping transactions is not possible. |
| MetaMask Correct Network Selection | Due to limited access for security reasons, MetaMask provides restricted access to the user's wallet. If the user selects the wrong network and makes a transaction, the coins won't transfer to the correct wallet. Due to limited access, correct network verification is not feasible. |

**Table 15.3.1: Description of Manually Performed Tests**

| Manual Method Test | Tested Features | Test Type |
| ------------------ | --------------- | --------- |
| Web Page 			 | 		 - 		   | - 		   |
| Database Data Entry | System Database | Component/Database Test |
| User Registration Test | System Database/User Interface | Functional/Component Test |
| User Login Test | System Database/User Interface | Functional/Component Test |
| Deposit Balance Test | System Database/User Interface | Functional/Component Test |
| Withdraw Balance Test | System Database/User Interface | Functional/Component Test |
| Wallet Addition Test | System Database/User Interface | Functional/Component/Integration Test |
| Balance Adequacy Test | System Database | Component Test |
| Number Verification Test | Number Verification System | Usability/Integration Test |
| Mail Verification Test | Mail Verification System | Usability/Integration Test |
| G.Auth Control Test | G.Auth System | Usability/Integration Test |
| General Functional Test of the Website | Web Page | Usability Test |

**Table 15.3.1.2: Description of Manually Performed Tests (Game)**

| Manual Method Test | Tested Features | Test Type |
| ------------------ | --------------- | --------- |
| Web Page | Navigations of the Game | Functional/Usability Test |
| Game Interface | Displaying User Inventory | Functional/Component Test |
| Game Interface | Visibility Test of Items in the Game Market | Functional/Component Test |
| Game Interface | Visibility Test of Items in the Marketplace | Functional/Component Test |
| Game Interface | Selling a Car in the Marketplace Test | Functional/Component/Integration Test |
| Game Interface | Buying a Car from the Marketplace Test | Functional/Component/Integration Test |
| Game Interface | Testing Balance Updates After Buy/Sell Transactions | Functional/Component Test |
| Game Interface | Testing Balance Update After Slide Coin Exchange | Functional/Component/Integration Test |
| Game System | Testing Requirements for Starting the Game | Functional/Component Test |
| Game Interface | Testing Car Ownership to Start the Game | Functional/Component Test |
| Game Interface | Testing Map Ownership to Start the Game | Functional/Component Test |
| Game | Testing Game Playability | Usability Test |
| Game/Web Page | Testing the Accuracy of the Game and Web Page | System/Alpha/Acceptance Test |

## <a name="_toc94305664"></a><a name="_toc94305784"></a><a name="_toc94305895"></a><a name="_toc94306061"></a><a name="_toc94390993"></a>**16 Success/Failure Test Evaluation Criteria**

The success/failure test criteria for the Slide It! system are explained in tables.

**Table 16.1: Successful/Failure Test Evaluations**

| Subsystems        | Features                  | Expected Input       | Expected Output                     | Success/Failure |
|-------------------|---------------------------|----------------------|-------------------------------------|-----------------|
| User              | User Registration         | User registration parameters | Displaying information screen indicating successful registration | Successful      |
| User              | User Login(W,O)           | User information parameters | Displaying information indicating successful login | Successful      |
| User              | Add Wallet                | Input of wallet information | Providing feedback that the wallet is active | Successful      |
| User              | Deposit Balance**         | Representative number   | Displaying balance in user presence | Successful      |
| User              | Withdraw Balance**        | Representative number   | Decreasing balance in user presence | Successful      |
| User              | Query User Balance(W,O)   | - (previously added data will be queried) | Displaying representative data | Successful      |
| User              | Query User Inventory      | - (previously added data will be queried) | Displaying inventory | Successful      |
| Interface         | Web Page                  | Testing general functionality of the web page (Button functionality, position, page integrity) | Clicks | Correct returns | Successful      |
| Interface         | Game                      | Testing general functionality of the game interface (Button functionality, position, game interface integrity) | Clicks | Correct returns | Successful      |
| Interface         | Game                      | Testing the playability of the game | Game playing style | Ability to play the game correctly | Successful      |


**Table 16.1.2: Successful/Failed Test Evaluations (Continuation of the Previous Table)**

| Subsystems | Features | Expected Input | Expected Output | Successful/Failed |
| ---------- | -------- | --------------- | --------------- | ----------------- |
| System | System Database | Data Reading | Random Data | Display of Random Data | Successful | - |
| System | System Database | Data Writing | Random Data | Display of Random Data | Successful | - |
| System | Game Market | Representative Item | Display of Added Items | Successful | - |
| System | Marketplace | Representative Item | Display of Added Items | Successful | - |
| Authentication | Mail Verification | Representative Email Address | Output Indicating Email Verification | Successful | - |
| Authentication | Phone Number Verification | Valid* Number | Output Indicating Number Verification | Successful | - |
| Authentication | G.Auth Control | Valid G.Auth Code | Verified Output | Successful | - |

## <a name="_toc94305665"></a><a name="_toc94305785"></a><a name="_toc94305896"></a><a name="_toc94306062"></a><a name="_toc94390994"></a>**17 Test Cases**
</a>**Table 17.1 : Detailed Test Cases and Results(Web Page)**

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.075.png)<a name="_hlk94302882">

**Table 17.1.2 Detailed Test Cases and Results(Page)**

![](https://github.com/metalfury/Slide-It/blob/main/src/Aspose.Words.aa6460c0-4681-4253-a446-2b7972708b33.076.png)

# <a name="_toc94306063"></a><a name="_toc94390995"></a>**V Glossary**
W – Web Page

O – Game

G. Auth – Google Authenticator

VT – Database

KLLNC – User

KYT – Registration

GRS – Login

ARYZ – UI

NVGSYN- Navigation

BGLNT - Connection

ENVNTR – Inventory

MRKT – Market

MRKTPLC – Marketplace

Slide Coin – Real cryptocurrency included in our project

Game Coin – Currency earned from the game
