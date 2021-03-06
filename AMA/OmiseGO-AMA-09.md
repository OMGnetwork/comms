# OmiseGO AMA 09

**[OmiseGO AMA 09 - December 7, 2018](https://www.reddit.com/r/omise_go/comments/a47365/omisego_ama_9_december_7_2018/)**

***

**Are advisors like Vitalik and the likes still involved in development of OmiseGO?**

Yes, advisors like Vitalik are still involved in advising OmiseGO. As advising goes, some advisors are more closely involved with certain technical aspects (we’re still collaborating closely with Vitalik and others on plasma implementation). Others will advise during certain phases of the project as appropriate, or when advice on their specific area of expertise is sought by the company.

***

**Are crypto friendly regulations required for increased levels of adoption of the OMG Network? If so, how far are we from crypto friendly regulations in SE Asia, etc.?**

Like any good lawyer will tell you, the answer here is "it depends." These regulations are still evolving in SE Asia and everywhere else. Friendly crypto regulations may not be "necessary" for adoption; but such regulations would certainly provide important information for participants in the crypto industry. Regulations will particularly affect the compliance measures centralized providers will have to take in order to be able to offer certain services to their customers. Plenty of use cases of the OMG Network, such as loyalty points or digitized fiat through a licensed e-money provider, involve transacting with assets to which already-established regulatory frameworks apply in a relatively straightforward way.

This also incorporates questions such as licensing or registration requirements under other applicable laws. Regulation is an important part of planning and risk management for any organization. Like any responsible business in a new technology field, we welcome clarity on how both current and future regulations apply to our business and the software we’re building.

Every jurisdiction across the world is distinct. Many government bodies have proven to be interested in input and collaboration from the blockchain community on how to regulate crypto without stifling its potential. If you’re interested to follow this topic more closely, CoinCenter (https://coincenter.org/) is a nonprofit organization that works on both educating lawmakers and the public, and advocating for sound policy around decentralized technologies. The transcript of Peter Van Valkenburgh’s recent testimony to the US Senate on the need for public payments infrastructure is a particularly good read.

***

**What has changed from last year that made you completely avoid the topic of big company (a.k.a. conglomerates)?**

It’s not so much that something has changed; more that nothing has changed as far as what we can say in public. We haven’t talked much about conglomerates lately because there’s nothing new that we can talk about in detail, and more vague references will not lead to any useful discussion.

We answered questions on conglomerates in both AMA #1 & #2:

We have mentioned ShinhanCard more recently as you can see but others we can't release names or more details of until the time is right due to NDAs. When more information can be released, we will be eager for the community to see it.

***

**Do we have anything to look forward to before the end of this year?**

While there’s much we’re looking forward to, we’re not going to hint at anything until we are ready to fully deliver. Since this isn’t much of an answer, we’ll respond to another question instead.

***

**What is it in the tech of Plasma Prime or some other that compensates for multiple plasma chains and How do you say that multiple plasma chains has become less necessary?**

The best way to explain this is to look at exactly what multiple child chains give us. Let's say we add just one more plasma chain to our system (for a total of two chains). Now in a way we've just doubled the throughput of our system because we can handle X transactions on the first chain and X transactions on the second chain. In theory we could just keep adding more chains to increase throughput.

But it’s not this simple in practice. One downside of the nested chains approach is that it's fast for people on the same chain to interact, but it's slow for people on two different chains to interact. But the biggest issue is that for each additional chain you'd like to talk to, you need to download the entire other plasma chain. Even if you never interact with people on the other plasma chains, validators still need to download the data for every single chain - that's potentially a huge amount (terabytes) of data every year.

Plasma Prime mostly solves these problems with some fancy cryptography that ensures you only ever need to keep track of *your own money* (whereas in Plasma MVP you need to keep track of *everyone's money*). That means we can keep adding more users and more transactions (increasing throughput) without really increasing the storage and computational requirements of end users. So not only can we scale just as well as with the nested construction, we can do so in a way that allows people to interact with everyone else in the system without needing to download a bunch more data (like you would need to do in MVP).

This still requires the stakers download data that scales proportional to total throughput, but it's a big improvement over the nested design. There's also no delay for users to interact with one another between chains or fragmentation of liquidity (because it's just one big chain).

**I wonder what will happen to OmiseGO if there is a fork on Ethereum and the community is split half and half? How and who will decide which chain to follow? Could it disrupt the day to day activities of OMG users/merchants? Does it means an update of the SDK and all clients built on it?**

This is quite a complicated matter, and there are so many factors that there’s no way to say anything with certainty until faced with the actual situation - which we have no reason to believe will arise any time soon, but anything’s possible in crypto. In short, If Ethereum forks during the POA phase OmiseGO will consider each chain’s hash rates, market caps, the intentions behind said fork, and social consensus post fork and choose one or both chains to support. If Ethereum forks under POS it will be up to the OMG Networks users and validators to choose whether to support one or both chains. This could potentially have the effect of forking the OMG Network, though this would only be the case if the fork is contentious and users and validators are split on which chain to support.
