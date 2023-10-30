# Practitioner's Perspective: Public Network Architecture
![[Week 1/3.Ethereum APIs/attachments/index_2.mp4]]


[MUSIC] The problem is those private
networks are invisible. You don't know that they exists. There is no telling how many hyperledger
fabric networks are out there today. We don't think that there is millions
of them or thousands of them, but it's an honorable number because it's not
any kind of subscripts like the public network, where you can actually
do any kind of analysis on that. So what's needed is a registar. And we think that the public network
is where that's going to live, just like you have DNS today and
you can go and register a name. There is something on Ethereum
called the ENX, right? The naming service for Ethereum. And that allows you to do
some really cool things. In fact, students of this course should
really look at the naming service on Ethreum, because it's a structure that
allows you to some really interesting things around, not only identity,
but around organization and things like access control and
user management. The naming services is vastly
underutilized compared to where it's going. It's very important piece of technology,
the Ethereum main net. And with that and some other things,
you can start to imagine having a registrar of both
private networks and public ones. So from ConsenSys's point of view,
I think and from Ethereum's point of view,
there's a vision that some of us share that I think is right where the public
main net becomes sort of the referee of millions of what we call en
lateral peer-to-peer connections. You and me, us this room, bigger group,
huge group, public group, right? And you want all those to be able to
coordinate so that our smart contract and they book other smart contracts,
they can book other smart contracts, ultimately with a public network, but
without invoking race conditions and all the other problems that
the classic distributed systems have. So here you have this sort of a kind
of time keeper, you have a timestamp on the block and you have this
public massive public network that's pretty hard to corrupt, vanishingly
small probability of corrupting, right? Not zero probability,
but limiting the zero. And that public network,
especially Ethereum, because it's got the attributes of
the turn and complete system and it's more than a key
value per storage system. It's a little more complex. It allows for more attributes. We think it's a pretty god referee for
all these millions of this factorial of
peer-to-peer connections, peerwise connections between
individual nodes, right? And once you have that, then you can say,
I want to register that. I'm going to register my node,
my node and your node, our connection. I can register it, or
I can say this is a network, or this is another bigger network. This is the supply chain for
the automotive industry network, but here is the rubber providence supply
chain or providence network for making sure that we don't have conflict
materials in our rubber supply. All right, those are two different
networks that created at different times without even knowing about each other. But if they're all coordinated
by the public main net, then they can start to as long as we
don't get the data models too wrong. We can start to bring those together and
say, all right, we started here. But now we're going to start doing
transactions with this larger thing. All right, I'm good here. I'm a tire manufacturer. I've got this rubber
providence supply chain, but I'm part of the automotive supply chain. I need to be part of both networks. And I don't want to have two
separate nodes that do one and the other separately. I want one set of nodes
that does everything. If I'm setting up that consortium, I want to be able to register that as
a thing that I can join on the main net. What tools are out there to
build interesting solutions or to tackle these problems, right? The interesting thing is that a lot
of these tools are just merging. There's a lot of opportunity
to build new tools, so if you're a tool builder, now's your time. Get out there, tell us about it. My job is the seeker of awesomeness,
so if you've got an awesome tool, come to me, something about it. Maybe we can turn you into a new venture. But there are tools and
then there are tools. So there are tools like plasma and
protocol level tools, and then there are tools on top of that,
just like computer science has always been a layer, a set of abstraction
layers all the way down and up, right? So here we are at this abstraction layer. We've got distributed systems. We have ways of managing
those distributed systems. We have consensus layers and
all these other things. We have the data layer and
on top of that, we have this layer of enabling tools that
help you build interesting solutions. Two of my favorites are uPort and OpenLaw.