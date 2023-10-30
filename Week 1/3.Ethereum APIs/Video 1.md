# Ethereum APIs
![[Week 1/3.Ethereum APIs/attachments/index.mp4]]
[MUSIC] What is an API? API, or Application Programming Interface,
is a convenient and standard way to expose a set of functions related
to a specific dataset and services. APIs also lend to reusability of code. An API publishes a set of functions or
methods that can be used programmatically to invoke
operations, access data, and store data. Access to an API can be controlled
by specific access method, for example, public keys, if so
warranted by the application. On completion of this lesson you will
be able to list the Ethereum APIs that facilitate Dapp development,
explain the functions and usage details of the various APIs. Two well-known examples of APIs
outside Ethereum blockchain are the Twitter API to access tweets
that can be filtered by query terms, Google Map APIs that allow for
applications to embed the map features, such as geolocation,
in their own applications, leveraging and reusing the power of Google Map API. Why are APIs important? Blockchain server and node provide
the blockchain functionality and data structures. How do applications call the functions
of a blockchain, invoke them? How do they use them for
accomplishing tasks of an application? We need a well-defined standard
approach to get things done for a Dapp. The answer is in the APIs. In our case, the specific APIs expose the services of the blockchain
server using standard functions. When you develop a Dapp,
interactions with the geth node on the blockchain server is
accomplished by invoking these APIs. For example, in the command miner.start(), miner is API, and
start() is the function of the miner API. Why in the context of a Dapp I'll
be learning about APIs? Blockchain technology has ushered in
a whole new culture in software and systems development and management. In the beginning, software systems
were proprietary products. Eventually, some moved on
to become open source. With blockchain technology, developers
are not only contributers to software, many of them help run the network by
standing up nodes, supporting mining, etc. More importantly, developers also
propose an oath on improvements and changes to the blockchain protocol. Thus, we want you to be
more than developers. You can be contributors,
you can be committers to code, you can help the governance,
and help shape the protocol. This is the technology culture
underlying the blockchain revolution. To enable you to be informed
developers in this context, you need a basic knowledge of the APIs and
the inner workings. Ethereum APIs, so
what are the APIs Ethereum provides? There are two major categories of APIs. The first one is the management APIs,
that includes admin, debug, miner, personal, and txpool. They support methods for
management of the geth node. The second one is the web3 API,
web3, eth, and net. They support methods for
development of Dapps. Next, we'll examine each
of the APIs in detail. Admin, the Admin API allows you to use
functions to work with your Geth instance, including network peer and
the RPC endpoint management. Examples, admin.addPeer(), admin.nodeInfo(). In this case, admin is the API,
and addPeer and nodeInfo are functions of the admin API. You can observe that admin supports
functions for management of the node. Debug API, example, Debug.dumpBlock(16). This will display the block
header details of block 16. You can observe that the debug
API provides you the ability to peek into the blockchain, study it, and
debug any issues by looking at the block. Miner API,
the miner API allows you to control the nodes mining operation and
set various mining specific settings. Very easy to understand. Example, miner.start(), miner.stop() are sample functions that will start and
stop the miner. You can also say miner.start(6), where 6 parallel threads are assigned
to the mining operation. Personal API deals with the creation and
management of accounts within a node. It also manages private
keys in the key store, that's why it is called personal API. Example, personal.newAccount() will
create a new account within a node. Txpool API, the Txpool,
or transaction pool API, gives you access to several
non-standard RPC methods to inspect the contents
of the transaction pool, containing all the currently
pending transaction, as well as those queued for
future processing. Example, txpool.inspect() lists you
all the pending transactions for you to peruse and collect for
building a block of transactions. So far, we looked at the management APIs
of Ethereum, now on to the web3 APIs. Web3.js library, when included into Dapp, lets you use web3 object provided by
the web3.js library and all its objects. It also lets you communicate with
a local node through the RPC port. It also provides access to the eth
object and its function via web3.eth, and net object via web3.net,
and their respective function. You can also access other
management APIs to the web3 object. There is also Whisper API, web3.ssh. It is used for secure gossiping and
enables the Whisper protocol. Web3 is a JavaScript library
that's specifically designed for use with web client or Ethereum Dapps. It's a portal through which all
the underlying operations of the Ethereum node on the blockchain
server can be invoked. For example, a Smart Contract deployment
and Smart Contract function invocation. You will use web3 in the development
in the front-end of the Dapp and for interacting with the blockchain. Now that we know the APIs,
here is a simple architecture of a Dapp. It comprises multiple full nodes with
only three of them, Node 1, 2, and N. You can also see all
of the APIs discussed. Geth command is used to expose
the RPC port, as well as the APIs. So far we discussed the architecture and
API details. When a web request is initiated by a user,
and if it's a regular web app request,
it is directed to the HTTP endpoint, say port 8080, and
to the web server to be executed. For a Dapp, the geth client has to expose
an RPC endpoint using RPC port command. A web3 object is instantiated
in the web page script. Recall that web3.js is
a JavaScript library. Requests or
calls are invoked on the web3 object. Requests are transmitted as a JSON or
RPC pipeline between the web client and the geth client. Requested call and function is
executed using appropriate API and Smart Contract code. And the result, return to the back client. As a recap, in this module, we introduce
a way at looking at the blockchain technology, blockchain server, and client. We created a two node peer-to-peer
blockchain network with ID 15. We learned the foundational knowledge
required to be a developer of a Dapp and a blockchain citizen. We explored the Dapp architecture and
the supporting APIs. Armed with all this knowledge,
we are ready to develop our first Dapp.