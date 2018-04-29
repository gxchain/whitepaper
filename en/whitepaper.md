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

Moreover, the second application based on GXChain, GXB Decentralized App \(Dapp\), which aims for personal credit management and face to face credit verification. The alpha version will release at the end of 2017.

#### **Consensus algorithm**

GXChain is using delegate proof of stake\(DPoS\) for bookkeeping on blockchain and proof of credit share\(PoCS\) for data exchange consensus.  
DPoS is originated from Graphene, it is an alternative consensus mechanism that requires coin holders to vote for “delegates”, who are then responsible for validating transactions and maintaining the blockchain. In DPoS, stakeholders elect what are known as witnesses. Witnesses are responsible and rewarded for generating blocks which are then added to the blockchain. DPoS is an alternative to the more commonly known, Proof-of-Stake model which requires miners to put up a stake in a cryptocurrency in-order for them to be able to validate transactions.

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

total\_sell is the frequency of data sold by the member.

total\_buy is the frequency of data bought by the member.

pocs\_threshold is the threshold to determine whether to reduce the transaction fee for members.

data\_transaction\_base\_fee is the basic transaction fee charged for exchange of data.

calculate\_pocs is the function to calculate PoCS score.

scale\_fee is the function to calculate transaction fee.

#### **III.Reasons to choose DPoS consensus algorithm**

Currently, most projects employed PoW and PoS as their consensus algorithm, and some projects used modified BFT. Bitcoin, the most successful cryptocurrency based on PoW, demonstrating the stability and fairness of PoW algorithm. However, bitcoin is often criticized by its energy intensive mining activity. Billions of Dollars are investing to perform calculation SHA256 for maintain the network, and besides that, no other utilization was involved in this activity. In addition, current transaction speed of bitcoin is 5 times/second, limited by its controversial block size, and 25 times/sec for another famous project, Ethereum, hindered by maximum GAS of single block. These numbers are far from VISA and Mastercard, that able to deal with thousands of transactions per second.

Peercoin and NXT brought two relatively matured blockchain based on PoS algorithm, featured energy friendly compared with PoW projects. Achieving PoS consensus by introducing the coin age theory. Instead of buying expensive mining equipment, PoS algorithm enable more people to attend bookkeeping. The computing power is correlate with the holding tokens and holding time. One hold more tokens for more time, the more possibility of generating blocks he will be.  Once he generates a new block, the number of whose coin age will be initialized to zero. Then a new loop starts.

Under PoS Consensus, people tend to lock coins for a long time to get more return, limiting coin supply and circulation, which is adverse to the price stability. Moreover, it is also possible that the majority token is hold by a small portion of people, making the whole blockchain network more centralized. Compared to the Consensus of PoW algorithm, the cost for being dishonest is much lower, as a result, it demands more mechanism for preventing fork/double spending attacks, as well as realizing consensus.  Normally blockchain network with Consensus of PoS algorithm could generate 12 transactions per second, however, due to consensus issues and network delay, it takes 60 seconds to finish broadcasting reliable blocks. In the long term, speed for generating new blocks is far lower than network communication and broadcasting, as a result, blockchains based on PoS have to limit the speed of block generation to keep the stability of main net.

DPoS could inherently overcome drawbacks of PoW and PoS in processing efficiency. DPoS algorithm require verification of current block has been signed by a trusted node before generating next block. DPoS employs a committee mechanism to choose trustable nodes\(witnesses\), who representing other token holders for bookkeeping. Witnesses are required to remain online for long time, solving the block generation delay problems occurred on blockchains based on PoS. Usually DPoS is capable of processing 10000-100000 transactions per second, depending on the network quality, which is suitable for industrial applications. GXB data exchange platform requires high transaction frequency and network stability, making DPoS is an exclusive choice.

#### **IV.Features of GXChain**

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

#### **V.Technical structure**

![](/assets/gxsaa.png)

#### **VI.Application structure**

![](/assets/gxsproduct.png)

### **1.For individual**

### **Wallet**

Wallet is for asset management on GXChain, we developed wallets for PC, mobile, web browser, and command line. For PC, Windows 32/64 Bit, Linux, and Mac OS supported. For mobile, IOS and Android supported, besides digital asset storage, mobile wallet will support real time price display from exchange in the future. Wallet on web browser is for online usage, supporting all functions compared with PC wallet. Command line wallet is more sophisticated for advanced user or developer.

### **DApp**

Dapp is for personal credit management, designed by GXB core developers. It could realize face to face credit verification and personal information management. After acquired targets authorization, one can check their credit information via GXB data exchange to easily achieve face to face credit evaluation. This application could broadly apply to recruiting, dating, renting, lending, over the counter trading etc.

### **2.For company**

### **Decentralized data exchange**

GXB team built a decentralized data exchange based on GXChain, personal data will not be cached on the exchange, protecting privacy of customers. In addition, GXB data exchange protects data copyright, prevents data fraud, and supports bilateral anonymity, which could be applied to various field, including personal loan, auto loan, banks, institutions, insurance, healthcare, credit bureau, logistics etc. GXB data exchange solved persistent problems in above industry for data transfer, circulation, and exchange in a decentralized and safely way, releasing the value of data for developing more applications which aim for improving quality of life of people.

### **DApp enterprise version**

Personal credit verification making GXB Dapp suitable for job interview, renting, second-hand transactions, and over the counter transactions. We planned to develop a web based software for enterprises to verify credit information from individuals.

### **3.For Developers**

GXChain supports app development using opened API, including data exchange, BaaS, Cli-wallet, statistical analysis, and blockchain explorer. Data exchange API will allow developers to use all interface from data exchange after installing GXB-BOX. BaaS API is for data storage, object-based storage, and verification, Cli-wallet API enable use command-line wallet, which could visit ledger and transfer directly. Statistical analysis API helps to develop further computing and visualization functions. Blockchain explorer API enable checking various information, including block, transaction, account information, and support developers to using web and API manners [https://block.gxb.io/\#/](https://block.gxb.io/#/).

For more details and events for developers, visit [https://forum.gxb.io/](https://forum.gxb.io/)

#### **VII.GXC and GXS**

GXC is for companies and individuals enrolled at data exchange to trade data. The conversion rate is always 1 GXC equals 1 CNY.  
GXS is the cryptocurrency on GXChain, issued by GXB team. GXS has the following values:  
•    GXS is the unique token on GXChain, it would be consumed/burned for app development, certification, and service will cost.  
•    GXB team will use 10% of the income from Data Exchange to buyback and destroy GXS every 3 months. One can expect data exchange would yield more income as more companies and data sources employ the exchange.  
•    GXS could be used as ballot paper for voting witnesses.  

**GXS Token distribution**

•    Total supply: 100,000,000.

•    Circulating supply: 60,000,000.

•    ICO amount: 39,000,000.

•    Private equity distributed amount: 10,000,000.

•    GXB foundation: 51,000,000.

•    GXS hold by GXB foundation is limited for circulation, released 6,000,000 for the first year, the funds will be used for hiring, community development, marketing, and business development, and will release for maximum 5,000,000 annually until total supply amount reached.

**GXS Buyback**

GXB team will use 10% commission from data exchange to buyback GXS, which will be transferred to the buyback account for destruction permanently, nobody, including our company, have the private key. We will make sure this procedure transparent and open, one could check it through blockchain explorer, and the buyback process will continue until all ICO and Private equity issued GXS \(34,510,000\) destroyed. The first buyback will proceed in Dec, 2017, then every 3 months. Second year, the buyback will proceed every 2 months. Third year, the buyback will proceed every month. Buyback account: null-account, one could use blockchain explorer to monitor this procedure.

### **VIII.GXChain team**

#### **Minqiang Huang** 
Founder and Chief Executive officer

Minqiang has over 10 years experience in data exchange, financial technology, and blockchain, he dived into cryptocurrency in 2012, and initiated several projects since then. He used to be CTO at Hakim Unique Internet Co Ltd \(SHE:300300\), and Director at financial services of HAKIM UNIQUE. He received his bachelor in computer science at Shandong University of Science and Technology, He received his master in management at Hong Kong Finance and Economics College. Besides blockchain, Minqiang is interested in ultramarathon, trail running, and mountain biking.

#### **Guojun Tu** 
Co-founder and Vice President

Guojun was a senior executive at 3 public traded IT company, he is a serial entrepreneur, who had more than 21 years’ experience in the field of information security, payment, and IT. Guojun received his bachelor degree in computer science at Hunan Univeristy.

#### **Cheng Wang** 
Chief Technology Officer

Cheng is a data expert, proficients in data collection, cleaning, machine learning and mining. He used to work as a full stack engineer at 51.com. Before 51 he worked at treefinance.com, and Vobile Info Tech Co., Ltd. as a core developer.

#### **Ruosong Xu** 
Chief Marketing Officer

Ruosong used to work at Huawei Technologies, China Mobile, and Tongdun. He is an expert in credit risk control.

#### **Xiaopeng Xu** 
Operations Director

Xu has 6 years experience of sales and marketing. He used to be marketing project manager at ZheJiang Media Group, Simei Media \(SHE: 002712\), and NetEase, Inc. \(NASDAQ: NTES\)

#### **Liyu Wu** 
Product manager

Liyu used to work as a senior product manager at NetEase,Inc.\(NASDAQ: NTES\), before NetEase he worked at Hithink Flush Information Network Co Ltd\(SHE: 300033\) and weidai.com.cn as product designer. He experienced in product management for both customer and business application.

#### **Xin Cai** 
Operations Manager

Xin used to be oversea technology manager at a fortune 500 company, she is proficient in Japanese, English and Korean. Currently she is responsible for business development of GXB data exchange. Xin received her master degree in wireless communication at Osaka University.

#### **Haoxiang Lan** 
Full stack Engineer, Data Exchange Product Director

Haoxiang is an expert in Node.js, iOS, frontend/backend development. He is experienced in blockchain development, especially for application layer. He used to work at 51.com and treefinance.com as frontend engineer. Together with Cheng Wang, he developed a unique data crawling method for backend/frontend interaction, which has been widely imitated by competitors.

#### **Junjie Zhang** 
Full stack engineer, UI design, Front-end/back-end web development

Junjie proficient in node.js, python. He used to lead front-end development of several renowned fintech companies in China.

#### **Liting Zhu** 
Blockchain developer

BS in Mathematics, MS in Computer Science, Proficient in P2P web development, C/C++, Python, Shell, he used to be core developer at Vobile Info Tech Co., Ltd.

#### **Jiahua Tu** 
Blockchain developer

Jiahua used to be cybersecurity project manager and core developer at Hangzhou Hikvision Digital Technology Co., Ltd., yielding multiple upgrades of the security platform.

#### **Lei Xu** 
Blockchain developer

Lei is a full stack engineer, who proficient in PHP, Node.js, Python. He experienced in cross end developing and data visualization product developing. Lei used to work as a core developer at ZhejiangDailyMedia and tops001.com.

#### **Jun Yao** 
Blockchain developer

As a JAVA engineer, Jun is used to work at treefinance.com as a core developer, he is proficient in data collection, data mining, and data analysis.

#### **Dongming Shen**
Blockchain developer

Dongming is a backend engineer, JAVA expert. He used to work at ddyc.com as core developer, he is an expert in App development for Android OS.

#### **Diwu Ye** 
Blockchain developer

Diwu is a backend engineer, he has abundant experience for data modeling, he developed data collection service with component-based approach.

