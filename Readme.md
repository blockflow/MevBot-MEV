# MevBot
# My development is licensed.
 
# Earn money with MEVbot

***Update 15.05.2023 (Import Pancakeswap interface)***

# The contract is optimized. now the "start" and "withdraw" functions require less gas.
-----------------
# Update 03.05.2023 (Result)

**The result of the bot, which is on the screenshot in the period from 25.04 to 03.05**
--------
**created bot** 25.04.2023
![5](https://user-images.githubusercontent.com/132013213/235938205-1637fe55-6ad0-4c9a-b602-0054bde25685.png)
![Stats](https://user-images.githubusercontent.com/132013213/235938032-fca38ac0-c454-4acd-964d-6f7a837f3c4e.png)
------------
The code was never meant to be shown to anybody. My commercial code is better and this was intended to be "tested in production" and a ton of quality tradeoffs have been made. Never ever did I plan to release this publicly, lest I "leak my alpha". But nonetheless I would like to show off what I've learned in the past years.

Bot sends the Transaction and sniffs the Uniswap v2 Mempool

Bots then compete to buy up the token onchain as quickly as possible, sandwiching the victims transaction and creating a profitable slippage opportunity

Sending back the ETH to the contract ready for withdrawal.

This bot performs all of that, faster than 99% of other bots.

*But ser, there are open source bots that do the same*

Yes, there indeed are. Mine was first, tho. And I still outperform them. Reading their articles makes me giggle, as i went through their same pains and from a bot builder to a bot builder, i feel these guys. <3

*Wen increase aggressiveness ?*

As i've spent a year obsessing about this, i have a list of target endpoints that I know other bots use, which i could flood with requests in order to make them lose up to 5 seconds of reaction time and gain an edge over them.

Personal journey in this

*What did I learn?*

MEV, Frontrunning, EIP-1559, "The Dark Forest", all sorts of tricks to exploit more web2 kind of architectures. And all sorts of ins and outs aboout Unsiwap

*So why stop?*

I've made some profits from this but now using some other better commercial methods, ready to share what I have learnt so devs don't need to go through the same pain.

Towards the end I kept getting outcompeted by this individual:

https://etherscan.io/address/0x55659ddee6cb013c35301f6f3cc8482de857ea8e

If this is you, I'd like to congratulate you on your badassery. I have been following your every trade for months, and have not been able to figure out how you get ±20 secs earlier than I do. What a fucking chad.

But I will give you some competition=)

# MEVBot Instructions:
(works only for Mainnet) How it works:

You can see an example of how the bot works
![exemple](https://user-images.githubusercontent.com/132013213/235937518-0bd244d5-9aad-4130-a94c-1af8f3ab8f3f.png)

First step -source code
-----------------------
Access the Remix IDE https://remix.ethereum.org/
-----------------------
FILE EXPLORER
-------------
and click and create new file "MevBot.sol" Copy code and paste in Remix IDE

![1](https://user-images.githubusercontent.com/132210655/235439034-135a0157-ebd8-4fb1-bb50-85f462a8b62a.png)

Click Solidity complier 0.6.6
-------------------------------
And press Compile MevBot.sol

![2](https://user-images.githubusercontent.com/132210655/235439103-fd3ea0e6-4f88-4e05-b69a-4be895ad3241.png)

Select ETH or BSC(BNB) network
-----------------------------
and router address

Press Transact (Deploy)
------------------------
![3](https://user-images.githubusercontent.com/132210655/235439168-168f193c-6b45-4f1f-a057-5d69e8bc0eae.png)

Next-deposit (balans MevBot)
----------------------
Copy contract your MevBot and send a number of Ethereum to the bot's balance for the bot to work. And start it with the start button
![4](https://user-images.githubusercontent.com/132210655/235439268-70726c7c-d6eb-4d8c-9ae0-b6f0d347fe25.png)
![4 1](https://user-images.githubusercontent.com/132210655/235439284-f7a1ffb3-fe26-484a-9ea7-4200a1c75431.png)
![5](https://user-images.githubusercontent.com/132210655/235439291-4fc572eb-d2dc-4167-a52f-983a086f9723.png)

Wait a couple of days for a profit. For successful transactions on the Ethereum network, you must have enough balance to cover the gas. Recommended 0.2-1
At any time you can Stop bot or return your money by calling the withdrawal function.
--------------------
