### **I.Abstract**

> big data era arrived, internet of everything is not far away. The ability of human in produce, acquire, and process data has been dramatically improved. Proper usage of data could greatly advance our knowledge of the world, reaction of demands, plans for the business and society activity, as well as cooperation.

With the rapid development of internet and information technology, the speed of data production increase exponentially in recent years. For the society, data is a continuously expanding treasure. However, as the amount of data skyrocketed, data monopoly and information silo issues becoming increasingly urgent. Get data flowing and utilize it legally could yield unimaginable value to social productivity and economy.

Data is the most important means of production in the future, not only in a giant scale, but continuously change with the evolution of human activity. Data is the key for us to understand business and society, which is indispensable for most industry. Blockchain is one of the inevitable and fundamental technology in the future, building an “internet of value” that could be maintained and participated by everyone. As a trusted internet, blockchain is capable of minimizing the cost of data transfer and exchange.

**The combination of data, the most valuable resource, and blockchain, an essential technology in the future, could discharge huge business and society value, which establishes the mission and vision our team. **

We have been building several products based on blockchain and data. As the cornerstone, GXChain combined big data and blockchain. The aim of GXChain is to build a trustworthy and all around applicable data exchange network, enabling data from every aspects to flow, circulate, and exchange efficiently, saving them from silo and monopoly, and facilitating them to provide more for our life.

### **II.GXChain**

#### **Introduction**

GXChain is a public blockchain for data exchange, developed by GXB team. GXChain is the foundation of GXB data exchange, supporting exchange of data in a million times per second. In addition, GXChain also supports app development. Apps developed on GXChain will be greatly supported by bigdata among various fields, which set GXChain apart with other public blockchain. Apps developed on GXChain would be real life oriented.

GXB data exchange, as the first business to business application based on GXChain, commercialized on September 24th, 2017, proving the commercial feasibility of GXChain. To date, data transaction on GXB data exchange platform passed 700 million times.

Moreover, the second application based on GXChain, GXB Decentralized App (Dapp), which aims for personal credit management and face to face credit verification. The alpha version will release at the end of 2017.

#### **Consensus algorithm**

GXChain is using delegate proof of stake(DPoS) for bookkeeping on blockchain and proof of credit share(PoCS) for data exchange consensus.
DPoS is originated from Graphene, 

PoCS, is a consensus algorithm developed by GXB team, aiming to solve the imbalance of exchange of data between big companies and small companies. Each PoCS score of alliance members will be calculated when they finished exchanging of data. In other words, PoCS score is based on frequency of transaction, and the score will contribute to the transaction fee. Members with lower PoCS score will pay more transaction fee for the data, while members with higher score will spend less on transaction fee.

Here is the psedo code for PoCS mechanism:

```
if ((total_sell + total_buy) >= pocs_threshold) {

    pocs = calculate_pocs(total_sell, total_buy);

    fee = scale_fee(pocs, data_transaction_base_fee);

} else {

    fee = data_transaction_base_fee;
}
```
pocs is the PoCS score, alliance members will have their unique PoCS score.

total_sell is the frequency of data sold by the member.

total_buy is the frequency of data bought by the member.

pocs_threshold is the threshold to determine whether to reduce the transaction fee for members.

data_transaction_base_fee is the basic transaction fee charged for exchange of data.

calculate_pocs is the function to calculate PoCS score.

scale_fee is the function to calculate transaction fee.

#### **Reasons to choose delegate proof of stack(DPoS)**

Currently, most projects employed PoW and PoS as their consensus algorithm, and some projects used modified BFT. Bitcoin, the most successful cryptocurrency based on PoW, demonstrating the stability and fairness of PoW algorithm. However, bitcoin is often criticized by its energy intensive mining activity. Billions of Dollars are investing to perform calculation SHA256 for maintain the network, and besides that, no other utilization was involved in this activity. In addition, current transaction speed of bitcoin is 5 times/second, limited by its controversial block size, and 25 times/sec for another famous project, Ethereum, hindered by maximum GAS of single block. These numbers are far from VISA and Mastercard, that able to deal with thousands of transactions per second.

Peercoin and NXT brought two relatively matured blockchain based on PoS algorithm, featured energy friendly compared with PoW projects. Achieving PoS consensus by introducing the coin age theory. Instead of buying expensive mining equipment, PoS algorithm enable more people to attend bookkeeping. The computing power is correlate with the holding tokens and holding time. One hold more tokens for more time, the more possibility of generating blocks he will be.  Once he generates a new block, the number of whose coin age will be initialized to zero. Then a new loop starts.

Under PoS Consensus, people tend to lock coins for a long time to get more return, limiting coin supply and circulation, which is adverse to the price stability. Moreover, it is also possible that the majority token is hold by a small portion of people, making the whole blockchain network more centralized. Compared to the Consensus of PoW algorithm, the cost for being dishonest is much lower, as a result, it demands more mechanism for preventing fork/double spending attacks, as well as realizing consensus.  Normally blockchain network with Consensus of PoS algorithm could generate 12 transactions per second, however, due to consensus issues and network delay, it takes 60 seconds to finish broadcasting reliable blocks. In the long term, speed for generating new blocks is far lower than network communication and broadcasting, as a result, blockchains based on PoS have to limit the speed of block generation to keep the stability of main net.

DPoS could inherently overcome drawbacks of PoW and PoS in processing efficiency. DPoS algorithm require verification of current block has been signed by a trusted node before generating next block. DPoS employs a committee mechanism to choose trustable nodes(witnesses), who representing other token holders for bookkeeping. Witnesses are required to remain online for long time, solving the block generation delay problems occurred on blockchains based on PoS. Usually DPoS is capable of processing 10000-100000 transactions per second, depending on the network quality, which is suitable for industrial applications. GXB data exchange platform requires high transaction frequency and network stability, making DPoS is an exclusive choice.

#### **4.Features of GXChain**

**High-performance and expandable**

GXChain can process 10000-100000 transactions per second, with 3 seconds blocktime. Considering the growing demand of on-chain business, GXChain can expand horizontally, enabling even higher transaction speed without a hard fork.

**Realtime parameter adjustment**

Instead of fork to realize change parameters, GXChain can change blocktime, blocksize, transaction fee etc. via voting. 

**Supported by bigdata**

GXB data exchange support data transaction or exchange in multiple industry. Companies and individuals could acquire those data via purchase.

**Blockchain as a service**
GXChain also supports services API, including storage and verification.

**Support for application development**

Apps developed on GXChain would get support by numerous data from multiple field on the data exchange

**User-Issued Assets**

GXChain allows individuals and companies to create and issue their own tokens.

**Open source**

We made GXChain code open to public at [https://github.com/gxchain](https://github.com/gxchain)

#### **5.Technical structure**

![](/assets/ta1.png)

#### **6.Application structure**

![](/assets/aa2.png)
