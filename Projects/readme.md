# Crypto Wallet

![](https://github.com/thumulakaru/Unit-1/blob/main/Projects/Crypto_wallet.gif)  
Giphy. “Crypto Wallet.” GIPHY, GIPHY, 14 Jan. 2022, https://giphy.com/gifs/crypto-wallet-coolwallet-cryptowallet-VMdnWZBRJO25bJInj7.

# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all his transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. 

Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.

## Proposed Solution

Design statement:
I will to design and make a Electronic ledger for a client who is Mr. Sato. The ledger will about Tren coin and is constructed using the software Python. It will take Project Week to make and will be evaluated according to the criteria below. I will be using the cryptocurrency TRON.


Justify the tools/structure of your solution

## Tron coin
TRON was founded by Justin Sun in 2017. The TRON Foundation was established in July 2017 in Singapore. The TRON Foundation raised $70 million in 2017 through an initial coin offering shortly before China outlawed the digital tokens. The implementations of TRON require minimal transaction fees in order to prevent malicious users from performing DDoS attacks for free. 1 Tron(TRX) is now exchanged for 8.77 JPY.
“TRON Coin.” TRON, https://tron.network/about?lng=en. 

## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4. The electronic ledger is password protected.
5. The electronic ledger is able to show records of a selected month.
6. The electronic ledger shows all transactionas related to a category.

# Criteria B: Design

## System Diagram
1. Dual core Intel Core i5 1.8 GHz
2. 8GB, 1600 MHz DDR3
3. Intel HD Graphics 6000, 1536 MB
4. 13.3 Inch Display
5. 121.12 GB HDD
6. Mac OS 12.5

![](https://github.com/thumulakaru/Unit-1/blob/main/Projects/System_diagram.png)

## Flow Diagrams

### Function for checking the records of a month
![](https://github.com/thumulakaru/Unit-1/blob/main/Projects/Function%20for%20checking%20the%20records%20of%20a%20month%20flowchart.png)

### Balance checking function
![](https://github.com/thumulakaru/Unit-1/blob/main/Projects/Balance%20checking%20function%20flowchart.png)

### Month validation function
![](https://github.com/thumulakaru/Unit-1/blob/main/Projects/Month%20validation%20function%20flowchart.png)

## Record of Tasks
| Task No | Planned Action                                                                   | Planned outcome                                                                                  | Time estimate | Target completion date | Criterion |
|:-------:|----------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|---------------|:----------------------:|-----------|
| 1       |                               Create system diagram                              | To have a clear idea of the hardware and software  requirements for the proposed solution        |     10 min    | Sep 22                 | B         |
| 2       |                       Creating a database for the password                       |                              Store the password in an encrypted file                             |     10 min    | Sep 23                 | C         |
| 3       |                           Creating the log in  function                          |                                   Prevent un-authorized log in                                   |     30 min    | Sep 23                 | C         |
| 4       |                                   Password Test                                  |                              Checking if the password properly works                             |     10 min    | Sep 23                 | C         |
| 5       |                              Planning the entry menu                             |                              To have a clear idea of the entry menu                              |     5 min     | Sep 23                 | A         |
| 6       |                              Creating the entry menu                             |                                 Displaying the entry menu to user                                |     30 min    | Sep 23                 | C         |
| 7       |                      Creating the month validation function                      |                 Using the function later to validate a month entered by the user                 |     20 min    | Sep 23                 | C         |
| 8       |                       Creating the date validation function                      |                  Using the function later to validate a date entered by the user                 |     20 min    | Sep 23                 | C         |
| 9       |                     Creating the integer validation function                     |           Using the function later to validate an input as integer entered by the user           |     20 min    | Sep 27                 | C         |
| 10      | Drawing the flow diagram for the function that checks whether a deposit is valid | Making it easier for program the function while having a better understanding about the function |     10 min    | Sep 27                 | B         |
| 11      |           Creating the function that  checks whether a deposit is valid          |              Using the function later to check whether  an inputted deposit is valid             |     15 min    | Sep 27                 | C         |
| 12      |           Drawing flow diagram for the function that checks the balance          |   Making it easier for program the function by having a better understanding about the function  |     20 min    | Sep 27                 | B         |
| 13      | Planning what the end message would look like                                    |       Have a good idea about the what the user would like to see at the end of the program       |     20 min    | Sep 27                 | A         |
| 14      |                              Coding the end message                              |                Printing a pleasant message for the user at the end of the program                |     10 min    | Sep 27                 | C         |

## Record of tests

|          Description         |      Type      |                                                Input                                               |                                                                                                     Expected Output                                                                                                    |
|:----------------------------:|:--------------:|:--------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|    Start up message & menu   | Unit test      |                                                None                                                | ===========TRON Wallet - 2022=========== Welcome to TRON wallet - 2022.  1. Check the balance. 2. Enter a transaction. 3. Check the records of a month. 4. Check transactions by category |
| Option selection by the user | Unit test      | Input between 1- 4 Input not between 1-4                                                           | Please enter the password: Error! You entered a wrong input(5). Please enter a valid input:                                                                                                                            |
|           Password           | Unit test      | Incorrect password   Correct password                                                              | You have 4 tries left. Please re-enter the password:  Continue the program                                                                                                                                             |
|   Option 01 (Balance Check)  | Unit test      |                                                None                                                | Your current balance is {Balance} TRX. Which is {Balance*8.8}JPY.                                                                                                                                                      |
|           User test          | Usability test |                                                None                                                | Ability of the user to understand the program just by reading the instructions printed                                                                                                                                 |
|     Date input validation    | Usability test | Invalid month(If the user enters a non-numerical value or if the user enters an invalid month no.) | Program prompts user that the month input is wrong and  prompts user to input again.                                                                                                                                   |
| Wrong password counter       | Usability test | 1. User inputs wrong  password when logging in                                                     | Program prompts user to retry logging in.  When the amount of times the username/password is wrong exceeds 5,  the program terminates itself.          

## Video of the program

[Recording of the program](https://drive.google.com/file/d/1tGeICXd6YiKwnQNiSdzueJF9GsfSNixO/view?usp=sharing)
