---
# Page settings
layout: default
keywords:
comments: false

# Hero section
title: AI Consumers

# extralink box
extralink:
    title: All Docs
    title_url: '/docs'
    external_url: false
    description: Find an overview of our full documentation here.

# Market Place
dev_news: true

# Micro navigation
micro_nav: true

# Page navigation
page_nav:
    prev:
        content: Concepts Overview
        url: '/docs/concepts'
    next:
        content: SingularityNET Services
        url: '/docs/concepts/service'
---

## Calling a Service



All complexity of invoking a service is abstracted from the users.
For example it becomes easy for the user to Input the values that need to be sent and view the computed expected result in the Output field, even without knowing the complexity of the gRPC calls/generating signatures for authorization to call a  service.  


Please note that the the Marketplace offers a **free trial** version, where registered users can access service(s) for a specified number of calls. 

![marketplace](/assets/img/dapp/free_call_feature.png)


Once your freecalls are exhausted , you will need to pay for any new calls to the service. for this you need need a wallet, some ethers in your wallet , some AGI in your wallet 


***You can either pay through Metamask or through a General wallet(paypal)***

- Select a Wallet -
![marketplace](/assets/img/dapp/select_awallet.png)


Lets look at each of the wallet options in detail below

### Using Metamask
**Important**: Metamask is a plugin which is used by the SingularityNET platform. This extension, allows you to perform the following in the context of the marketplace:

- Transfer AGI funds into escrow, 
- Setup payment channels to enable calls to any of the listed services.

As a first step you will need to Authorize the Dapp to connect to your metamask account
- Authorize Metamask -
![marketplace](/assets/img/dapp/authorize_metamask.png)


#### Depositing tokens from Metamask to the Escrow Wallet.

Steps
1.	Let start by depositing some tokens from Metamask to the Singularity Escrow Wallet. So you can pay for service
2.	On the Home page click on Account link
3.	Confirm you have sufficient balance in your Metamask Wallet
4.	In your Account details, check the Total Balance, This is the number AGI token you have in Metamask wallet
5.	In the Manage your Escrow account section, Enter the amount of money you want to deposit to the Escrow wallet
6.	Click Deposit. A Metamask Window should pop-up. If it Metamask Window does not pop-up, click on the Metamask icon on the top of your browser.
7.	Check the transaction and click confirm.
8.	Wait for the transactions to be mined.
9.	This is two step transactions; you will need to confirm both steps.(Gas fee and Total)
10.	Wait for the transactions to be mined again
11.	Confirmation message show that the token has been deposited to the Escrow wallet 
12.	You might need to refresh if your token still appears as authorized.

If you dont have money on Escrow account, you will be asked to ***Deposit into Escrow***
![marketplace](/assets/img/dapp/depositinEscrow.png)
Now click on **Deposit**

You need to confirm every Blockchain transaction when using metamask as your mode of payment
![marketplace](/assets/img/dapp/confirmationfrommetamask.png)

Based on the number of calls you wish to invoke ,select the option and the channel will be 
funded accordingly
![marketplace](/assets/img/dapp/metamaskmultiplecalls.png)

Once the funds are in the channel, you are all set to invoke the service !


### Using General Wallet 

Select the 'General Wallet' Option
![marketplace](/assets/img/dapp/marketplaceimage.gif)


### To call a service 

1.	View a list of service from the home page.
2.	Filter the list by using the search text box.
3.	Look for  image recognition service
4.	Click on **Demo**. 
    This will take you to the corresponding service details page.



If you are using General Wallet and you have sufficient funds , you will see the continue button 
![marketplace](/assets/img/dapp/generalwalletUse.png)

5.	Now you have the access to the invoke section of the service 
    The interface will change according to the input need for each service.
6.	Choose a Method to identify the service -  An Image
7.	After setting-up all that you need,  click the **Invoke** button.
8.	If you are using Metamask , then the transaction will need to be signed again using metamask before invoking 
9.	Wait for the response
10.	You are now eligible to write a review
![marketplace](/assets/img/dapp/reviewscree.png)

You can now continue to use the Service till you have sufficient funds before the expiry date of the channel

### claim back the reserved fund
1.	Go the **Account** page
    If there is any expired channel it displays under the **Expired Channel Details** section
3.	Select the channel you want to claim
4.	Click **Claim Channel**
5.	Confirm this transaction on Metamask
6.	Wait for it to mined
    Displays the message confirming that funds have been successfully claimed.  Once you do this, the payment channel you claimed is unlisted.

### Withdraw tokens from Escrow wallet to Metamask
1.	Go to the **Account** page
2.	In the**Manage your Escrow account** section, select  **Withdraw**
3.	Confirm that you have sufficient funds in the Escrow wallet.
4.	Enter the money you want to withdraw and click **Withdraw**
5.	Confirm this transaction on the Metamask
6.	Wait for it to be mined
    A message displays that the withdraw has been successful
8.	Refresh the page to see the balance is updated.
    You will be able to see the token back in to your Metamask wallet. 


## Marketplace Requirements

If you are a service author, need the service to be visible to others and listed on the marketplace you must:
1.	Build and publish your service 
2.	Use SSL with the snet-daemon. 
    **Note:** if you don't already have an SSL certificate for your domain, it is recommend you use certbot and letsencrypt .
3.	Fork the snet-dapp repo, build a react component as the user interface for your service, and submit a pull request. 
    **Note:** Identify the services on your networks, organization and service names being used. For more details, refer to dapp repo README.md.
4.	Last is some paperwork that we are still finalising, and we'll update this list when we have that. If you are itching to get your service listed, reach out to us via one of our community groups.
    **Note** that your service can be published to SingularityNET without being listed on the marketplace, but your service may be less discoverable to potential customers if it is not listed. 
