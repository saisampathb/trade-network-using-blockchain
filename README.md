# sams-trade-network
Sample Trade network created using block chain by using Hyper Ledger Composer on Hyper Ledger Fabric.

To see the network on your local computer, try below:


Step 1:

After download create the business network archive using :

composer archive create -t dir -n .

Step 2:

Create a network admin card on the composer playground / or use any one that you have. I have used the default one here.
You can also import businessnetwork cards into blockchain network using:

composer card import --file networkadmin.card - which could be basically signed certificates or a key-pair.

Deploy the network created using:

composer network install --card PeerAdmin@hlfv1 --archiveFile sams-trade-network@0.0.1.bna

Step 3:

Block chain transactions are carried out using REST calls and are updated using smart contracts. Hyper ledger composer has an inbuilt tool for creating REST server. Use below two commands to generate 

composer-rest-server
yo hyperledger-composer

you can then use REST API to call and query the data ledger.
you can also add more number accounts to the network by modifying the cto file. 

Please do give me a feedback of your experience. 









