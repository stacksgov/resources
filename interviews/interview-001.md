*   What is your role?
    *   People don’t usually pay attention to what I do as long as it works
    *   I give an occasional meetup talk often only 1/3 of audience understands
    *   This is usually what I do, the extent of my interaction with the community
    *   Community is very important for cryptocurrencies, even more than for e.g. Linux. A large community is a strong security measure against attacks on the blockchain, since they’re all vigilant and they care.
    *   There’s real money at stake, skin in the game for community members
    *   Reasons for them to care a lot about future of the project
    *   Unlike conventional open source, forking a codebase is not sufficient to resolve problems - e.g., dozens of forks of BTC but their collective market caps are tiny
    *   The notion of wealth/that your tokens have worth is “shared state” across the community - your tokens are only valuable if others believe they’re valuable
    *   So we need to be able to resolve conflicts “in band” i.e. without forking
    *   So the need for a cohesive community and conflict resolution mechanisms is far more important in cryptocurrencies
    *   That said I don’t think governance is anything like it is in meatspace
    *   Unlike governments of the world, you are not bound to one particular “nation” ie. blockchain
    *   What that means is that the people that are most in need of conflict resolution protocols (automated or human-driven) are those who have skin in the game economically as well as emotionally - “I use this thing because I really do believe in the mission"
    *   In academia, software forks happen all the time, it’s celebrated: we forked the Linux kernel and made these changes to test this hypotheses
    *   The word “fork” is overloaded: you can easily fork the code, but forking the community is much harder.
*   How do you make people believe in your legitimacy?
    *   People believe in blockchains for reasons that are monetary but it’s more than that
    *   There’s a mission statement, ethos, set of values that resonate
    *   Demonstrating that you can “walk the walk” of that vision
    *   This is true outside of crypto - any sort of social movement is like this! The ones leading that movement are the ones seen as leading it the strongest
    *   A lot of political revolutions e.g. LGBTQ, civil rights happen because they can appeal to consistency with e.g. freedoms in the Constitution/what the founding fathers said/believed. (Example: “black people and white people should be equal before the law” because “All men are created equal”)
    *   This is generally true outside of “real governments"
    *   And in blockchain - for people who care about that
    *   There’s a lot of value in faking that signal long enough for bag holders to dump - there’s a lot of that faking going on, muddying the waters for economic advantage
    *   You manage to walk the walk even when times are hard - e.g. when your token isn’t doing well
    *   You do it with no skin in the game, or only token skin in the game - e.g. I want this to exist even if I don’t personally hold these tokens
    *   This is true for Bitcoin as well - if Satoshi never spends those tokens - the ethos behind this “banking system independent of government” - whether you believe this mission statement or not is irrelevant, some people do
    *   Ethereum: “We want to be the world computer” where you can execute programs without permission of government - this appeals to a similar segment of people
    *   Blockstack: We want to create the user-owned internet; data, compute, you reap the value that your online activity generates. The notion of ownership is extended into your digital life, you’re a more fully-realized digital citizen whose inalienable rights are met through the deployment/instantiation of this particular protocol.
*   What do we do for lack of a constitution?
    *   Eos was onto something but executed it badly
        *   Constitution is legally binding but you can’t legally bind blockchain validators - there’s no body politic to do this
        *   It was considered an encroachment on their rights
        *   The idea was directionally right - should’ve called them operating principles - “here are the guidelines that make for a good validator” - rather than binding legal guidelines
    *   We have [principles of dapps](https://docs.blockstack.org/develop/dapp_principles.html) - one of our most widely visited docs - based on an hourlong braindump I wrote on a train ride
    *   This happens outside blockchain: e.g., [UNIX philosophy](https://en.wikipedia.org/wiki/Unix_philosophy)
    *   A similar high level ontology could be created for Stacks that also enshrines operating principles
    *   If you succeed in doing this, a trailing success signal of the quality of your principles would be many protocol-level incompatible implementations of those principles that all adhere to those principles
    *   E.g. there are many binary incompatible but philosophically aligned UNIX implementations
*   I no longer believe in most of Barlow’s [Declaration of Independence of Cyberspace](https://www.eff.org/cyberspace-independence)
    *   It’s a “fundamentally undemocratic manifesto”, i.e., “I should be able to do whatever I want, FU for getting in my way”
        *   Does that include money laundering, child porn, financing terrorism?
        *   Some people in Bitcoin reject the idea that these things could be bad since they reject the idea of government telling them what they can do with their money
        *   I reject this idea for Stacks - it’s reprehensible
    *   UNIX philosophy is not a manifesto - they were organically observed
    *   a manifesto is different - goes stale faster than set of design principles - a manifesto is a creation of the political times in which they were written
    *   Not really falsifiable - “it’s my opinion that…” e.g., “I should be able to do whatever the hell I want in cyberspace”
    *   If you put it to the test and let people do this it’ll lead to outcomes that are at odds with western liberal democracies
    *   This is not true for e.g. UNIX philosophies
    *   Lane: design philosophies not designed to address social/economic/political things, so they’re less contentious
    *   Design philosophy doesn’t say anything about social stuff
    *   I disagree with the “apolitical” mentality: you cannot avoid politics
    *   The tyranny of structurelessness happens implicitly
    *   Aaron has a more Hobbesian take on humanity - he’s more cynical than I am
*   What are the values?
    *   People play different roles, wear different hats
    *   You can be a community member, a miner, an operator of a full node - or in multiple roles
    *   I spend the most time thinking about how miners should behave, that’s the closest to what I have to work with
    *   My thoughts are about how to keep the system running “without us” - if we core devs were to step away tomorrow - our job isn’t done until this is a resounding “yes!”
    *   I don’t like the word decentralized b/c it’s not well-defined, it means “whatever feels good"
    *   Our blockchain’s principles of operation cannot be separated from a notion of governance
    *   Those who produce the blocks ultimately decide the evolution of the chain state as a whole
    *   What appeals to me is less decentralization, and more, “how resilient is the system to bad governance?” E.g. if miners were to mine empty blocks? Or invalid blocks? If peer network were attacked and chain were to split? Can system recover by itself from these things?
    *   Someday the governments of the world will pass laws limiting what exchanges can do - can the blockchain be designed in such a way that’s compatible with those laws? Without breaking the system/causing a hard fork?
    *   Hard fork is mechanism of last resort - something more severe than amending the constitution - like an insurgency (not quite a civil war) or a secession
    *   A lot of designs in Stacks chain are such that as miners do their thing, the system can stay in sync with what’s going on, _in situ,_ i.e., _without needing hard forks_
    *   To make sure the system can “keep up with the times”, can adapt to changes in regulation, what users need, etc. - we’ve done the following:
        *   Clarity is a decidable programming language so it’s possible to soft-fork by constraining the set of valid transactions
            *   This means you can tell whether a tx will do “the bad thing” before running it, and soft-fork by agreeing to not mine it
        *   If the DAO were built on blockstack + clarity, you would not need to hard fork - you could tell it will withdraw funds from the DAO - I won’t mine it - soft fork it out of existence, without a chain split
        *   Also, our system can fork, there can be multiple forks of the Stacks chain, that’s vital to surviving periods of miner issues - it’s possible for a longer fork to later invalidate decisions of some miners
        *   The act of mining a block is the act of burning/transferring BTC via PoX
        *   Another level in hands of users - “user support burns” - it’s not just me who is mining a block in the chain, others users can commit BTC to a block - if I’m an honest miner, my supporters can help me produce the chain, or take support away if I stop being good - users can send a transaction directly, their BTC + my BTC is summed together to form my mining power
            *   This is not delegation - those to whom votes are delegated to can keep votes by force by refusing to mine those tx - as a miner, I cannot stop you from un-delegating
        *   Users receive a portion of the coinbase, a fraction relative to their overall size, for each mined block - users aren’t just doing this out of goodness of their hearts
    *   Are you afraid of vote buying?
        *   Economists don’t expect rational actors to ever use user supports because “it’s more profitable to be a miner" and “it’s more profitable to consolidate user-support burns to avoid transaction fees”
        *   Money is not the only thing that motivates people
        *   E.g. segwit getting activated is evidence that people care about BTC’s longevity
        *   A way for users to signal support for miners that are doing the things they want - there is a notion of consent of the governed here - and miners can’t stop you from doing this
    *   What other ways exist to have consent of the governed?
        *   Discord, forum, people talk to each other - we need to have a public forum for the community - in touch with each other, miners, developers, etc.
        *   I try to do my interactions in public (no DMs)
        *   Less technical, more of an operating principle: be as transparent as you can
        *   Do. Not. Lie.
        *   Do. Not. Mislead.
        *   Do. Not. Bullshit.
*   I’ve seen the shitstorm that Twitter can be
    *   Thought about this a lot, not in terms of governance, but how do I build social media apps that I’d enjoy using?
    *   My idealized comms channel with the community would have two properties:
        *   I can shadow ban people, full stop, if you’re a dick I don’t need to hear from you ever again, I’d rather let you “scream into the void”
        *   You should be able to subscribe to my shadow ban list. This is a great way to deal with trolls, if you also don’t want to hear from the same trolls
            *   Has the effect of creating a fishbowl that’s soundproof - you and I as core devs can talk on Twitter, there’s value in our relationship - the people from the outside (w shadow ban turned off) can see miasma of shitpoisting on Twitter - but our conversation is still public, don’t need to deal with psychological burden of shitposting - good for our mental health and also for the community
            *   Don’t want people to burn out because others are horrible to them
            *   My attention isn’t free, so it won’t be wasted on people who waste my time
    *   A lot of people I follow on Twitter are on the receiving end of this - they get doxxed, harassed, even physically harassed, often women and people of color - in e.g. open source communities
    *   Yes people are shitty and I blame people for that but I also blame the platform for encouraging shittiness - I need a way to avoid shittiness, and the platform needs a way to discourage it.
    *   So my idealized channels: need to be able to shadow ban people, subscribe to your shadow ban list, and this info needs to be kept private so the trolls are forced to waste their time - there are studies that show this works and in fact that it’s the only thing that works - the effectiveness of shadow banning - is demoralizing rather than enraging
    *   Free speech stops at my computer - once it’s at my computer I can do what I want with your data - this is not censorship
    *   I as a user should have the right to implement to my own client that does this - you have the ability to build your own client with or without the platform’s blessing - this is an under appreciated feature - ability to curate your experience of the platform to you
*   The ability for users to own their own chain - I briefly described app chains to you - I’m completely ignoring eth2.0 and algorand and dfinity and other shard-based systems because I don’t think they’ll work
    *   The problem I’m interested in solving isn’t building a bigger mainframe
    *   Users can seize the means of production by owning the computing that happens on just their data (didn’t mean this to sound so Marxist!)
    *   The history of computing is largely the history of sharing time on the mainframe - batch jobs went away in favor of the computer multiplexing itself into processes, login shells, virtual computers - giving you the illusion that you have access to the entire computer - with the assumption that none of us will even come close to using the system’s full resources
    *   Preemptive multitasking system - this principle lives on today!
    *   Also true for web servers and the cloud - we call it “login sessions” not “time sharing”
    *   You’re using a tiny sliver of Facebook’s processing might - all those things require computing, state transitions - e.g. updating your feed, image tagging, etc.
    *   Stacks gives users the same kind of power - not by forcing them to all compete over a tiny trickle of bandwidth like blockchains today - but by letting users run their own blockchains, i.e., app chains, that only process requests on the user’s data
    *   The act of mining an app chain is the act of sending transactions to a parent chain that anchors blocks in place and encodes parent-child relationships
    *   Stacking many chains on top of each other - there can be infinitely-many such chains, all just as reorg.-resistant as main BTC chain
    *   There’s a fundamental difference with sharding - each chain has its own token, and there’s no two-way transfer
    *   That these are blockchains is an implementation detail - in reality they are just decentralized personal servers - I have a raspberry pi at home acting as my server - take that away but keep the concept - other people authorize transactions by mining them - the server logic itself is replicated across all your devices and your Gaia hub - Gaia can serve chain data to anybody and thus service read-only requests while you’re offline
    *   It’s offline until you sign into app, then you process incoming transactions, state transitions - because the system can fork, your decentralized personal server is resilient to failure - can restart it at any time to undo things that happened in the past (or pick up where you left off if your device breaks or gets stolen)
    *   There’s no maintenance because the programming model of Clarity is much smaller than sharing e.g. a VM across devices - much more tailored towards realizing this decentralized personal server that carries out state transitions on your data
    *   The fact that we have a token is serendipitous. The token is really just a way to implement time sharing in a resource-accountable manner. There are underexplored business models that would allow me to sell tokens to others to allow them to post data to me:
        *   For me realizing a benefit from the app
        *   Having an easier time mining blocks that requires a tx on a separate chain that I need a token for
        *   Etc.
    *   On “App Chain” concept
        *   That stuff is about business models, but the overall mission of app chains is fundamentally about users owning the internet
        *   App chains also have an impact on governance: there’s no need to change the main chain all the time for every new feature. If you want to try out and use a new blockchain feature in production that’s incompatible with the mainnet, you can spin up your own app chain with that feature. For example, if you want Clarity routines for verifying zero-knowledge proofs, you can fork the Stacks codebase, add that in, and spin up an app chain with those new functions available. You don’t have to modify the Stacks chain itself.
        *   In this model there are three roles:
            *   Stacks chain proper, root chain that stores mining and routing for discovery of chain above it
            *   Intermediate chains - all app-chains, their function is to be hosts for other chains, e.g., “cloud servers” - to increase total no. of chains at periphery that can be supported
            *   User-mined app chains that will only ever have one miner - the user itself within the context of that one app. I as a user can have such a chain for every account I have in every app - just legitimizing writes others make to my state.
    *   Re: governance: GNU herd, obscure kernel that Linux ended up taking over
        *   Stallman tried to put in design principle: OS behaviors - process management, dealing with device drivers, resource allocation policies, etc. - can be set on a per-user basis
        *   Different than normal timesharing systems like UNIX where you’re at the mercy of the sysadmin
        *   Between traditional timeserving and e./g. your own VM on AWS
        *   Difference is lack of coordination - frees users from stepping on each others’ toes
        *   If you put each human in their own “hermetically sealed matrix” - everyone you talk to is a robot - you’re the only real person in your own universe
        *   No need for governance because you’re not interacting w people in the first place
        *   Makes innovation easier to come by - your app chain can be tailored to do anything
        *   “The only way you can interact with my app chain is through my tx which I mine” - wholly acceptable for me not to mine your tx
    *   What about Urbit, or SSB?
        *   Urbit is toxic and I don’t seek to emulate it in any way - it’s “digital naziism"
        *   you are given a name that you don’t own, you’re at whims of galactic senate - it’s neo-feudalism
        *   SSB is very link-local: my state is not externalized anywhere.
            *   the only way you and I can sync is if we are on same LAN or have third party relay server that relays STF
            *   in our model, we make provision, you don’t need to publish blocks, just hashes, but you do have to publish blocks to legitimize the decisions you made
*   How do changes happen now?
    *   Very much by decree. We say a hard fork has happened and it happens.
        *   It’s all been uncontentious so far
    *   I don’t like it, I don’t think it’s sustainable
    *   We’re getting rid of it too.
    *   Stacks 2.0 has mechanisms to do _in situ_ soft forks, and rolling out incompatible features as app chains, it should remove need to do hard forks altogether
    *   If a hard fork is ever needed, we’d have a committee set up for deciding this - Muneeb is best person to talk to about this - a five person committee: one person from PBC, one from Stacks Foundation, one community seat, and two others
        *   They’d have power to say emergency is happening, we have to hardfork
    *   A lot of things won’t need this
    *   Similar to BTC we’d have support for on-chain signalling
    *   App chains for launching new features that are backwards incompatible but still valuable
    *   Technical governance is more like a do-ocracy
    *   Unlike BTC and ETH we’d encourage people to make their own chains
    *   The token is not meant to be money or replacement for money
    *   Do these things because they’re interesting or solve a problem not for money
    *   Token IS an AWS compute credit
