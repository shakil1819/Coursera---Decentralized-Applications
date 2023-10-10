# Decentralized Applications (Dapps): Blockchain Server
![[index.mp4]]


[MUSIC] Decentralized applications or DApps, open up the features and services of the blockchain to the whole world for review, interaction, and enjoyment. DApp gives access to people, applications and systems, not necessarily known to each other to transact peer to peer. DApp is an end to end application on a blockchain. We open this course with essential concepts, such as the blockchain server. DApp architecture, and the details of the supporting application programming interfaces or the APIs. We'll go on to experience a hands-on, practical incremental end to end development of a DApp using the Truffle IDE. We will then explore a few smart contract specific best practices to improve the basic design of DApp. And finally, we'll review standards that are essential for transformation of an emerging technology into a mature evolving technology. On with this road map of the DApp development process, you will be prepared to chart your path through the emerging decentralized software culture. A DApp or a decentralized application depends on the functionality of a blockchain for its infrastructure and operations. In its simplest form, a DApp has a client interface as a front-end, and a back-end that includes a blockchain and a smart contract. Consider, for example, a simple wallet application client, and the Bitcoin blockchain decentralized infrastructure. This is similar to the architecture of a web browser and a web server, but with one significant difference. The blockchain enables a decentralized infrastructure. Remember, the blockchain is not in one centralized place, but in the computing nodes of the peer participants. The client or the front-end can be a web app, HTML and Javascript framework. A command line interface, CLI, a desktop application, a mobile application, or even an IoT, Internet of Things. Understand web front-end is outside the blockchain protocol, and it can only link into the blockchain smart contract, using artifacts generated by the smart contract compile process. Recall, we discuss these artifacts generated by Remix IDE in course two. Additionally, a DApp can be created with a non-blockchain back-end. Interplanetary file system, IPFS, is an example of such an architecture. On completion of this course, you will be able to discuss the architecture of a Dapp. Design and develop end to end decentralized application using Truffle IDE, smart contracts, a web client, and a meta mask client. Explore best practices in designing a smart contract in the context of the Dapps. Discuss Dapp models and explore emerging standards that are essential for predictable behavior of Dapps. 
[MUSIC] On completion of this module, you will be able to explain the architecture of the Ethereum blockchain server, and explain the high level architecture for Dapp. This is a high level of the Dapp's stack. It has a peer-to-peer network on which that blockchain operates. The node of a blockchain hosts the EVM and the smart contract runs on the EVM. The user interfaces of the Dapp runs on top of this layer, they use the smart contract for their logic. Next, we'll dig deeper into the architecture of the blockchain based Dapp. Using the actual commands that are used to create the architectural components of a Dapp. It is important that you have mastered the basic concepts from course one and course two. And have some basic knowledge of command line interface to get the most out of this course. We've been looking at bits and pieces of blockchain infrastructure in the last two courses. Now it's time to put them together, and have a grand view of the whole structure. We're going to coin the term blockchain server for representing the infrastructure and the functionality the blockchain provides. This nomenclature is drawn from the similarity in a web server web apps. Mobile server, mobile client apps, database server, database clients, etc. So the term, blockchain server for all the functionality it provides, Blockchain server Dapps. Here you see the set of commands that install the Ethereum services and the application programming interfaces API it exposes. To enable node creation, application development, and transactions on the blockchain. At this point make note of the commands, you don't need to memorize the commands. Just try to understand the concept of the blockchain server, on the base on which the Dapps will be built. The term blockchain server also helps to differentiate the blockchain, the ledger from the protocol services. Now that you've established the foundation, let's create the node on the blockchain server. Here we create a single node, Node 0, at the genesis node for our blockchain server. The network ID for a blockchain server is 15 as you can observe in the third command line, it is still a private local chain. Are you curious to know the network IDs for the common public networks? That network ID for the Ethereum main network including metropolis, is 1. Ropsten, the public cross-client Ethereum testnet is 3, Rinkeby's network ID is 4. There is even a Musicoin, the music blockchain, with network ID 7762959. When you deploy a public blockchain, you should be aware of the network IDs of other public nets. Also, when you're in a private environment, you should be aware of the other network IDs in use if there are any. Think about the highway structure in the US, there can be only one number in state highway that can carry across state lines. For example, the interstate Route 90, there can not be another Route 90 across the nation. In the case shown, we are using geth command, provided by Ethereum server recently installed. We use geth command to install a node by creating a new account number an externally owned account, EOA. Recall that we have discussed EOAs in earlier courses. We then initialize the node using a custom genesis block that has a specification, the first block of the chain. Finally, we specify the network ID and the port to buy into for the node that interact with the blockchain. At the bottom, you will see the Ethereum node, enode address for this genesis node or the bootnode created. Then enode address is used by other nodes to connect to this bootnode, and establish a peer-to-peer network on which the blockchain operates. Recall that a peer-to-peer network is one of the fundamental concepts in blockchain technology. We have not listed all the commands needed for the networking details. That is beyond the scope of this course, the focus of which is on Dapp development. We have completed the creation of one node, let's now create at least one more peer node. Here we are creating node one, and adding it as a peer node to the bootnode we created earlier. After creation of this node, observe that we are using admin APIs, addpeer command, the fourth command, and the enode address of the bootnode we created earlier. The IP address and the binding port of the bootnode, 303xx, which represents the port number of the original node 0 that we create. This is how peer nodes are created and connected to join the blockchain network. Here you see multiple peer nodes 1 to n. When you want to join the blockchain network ID 15, install the base Etherium server. Then execute the commands as shown earlier for a single node creation, and add it as a peer. Thus, we have a peer to peer network enabling the blockchain operation. Recall course one's project that used the same techniques, but the commands were hidden from you. There are alternate methods to create the blockchain network, and we have shown just one approach. Summarizing, we have establish the notion of blockchain server as the foundation for a Dapp. We have demonstrated how to install the blockchain server and establish a peer-to-peer network of nodes. You explored an Ethereum blockchain server and a geth node, so that you can be an informed Dapp developer. It's a common practice to develop and test a Dapp on a local test network before deploying it on a public network. Now, let's move on to developing and testing a Dapp.

## Commands
![[Pasted image 20231010110919.png]]
## Genesis Node creation
![[Pasted image 20231010110945.png]]
![[Pasted image 20231010111226.png]]