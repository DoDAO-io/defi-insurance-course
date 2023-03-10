## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Ease
 
 **Introduction**        
### What is RCA 
The present approach for offering protection to users against various risks is similar to that of traditional financial institutions: underwriters provide funding, evaluate risk, establish a cost for coverage, and users buy a policy.  This strategy has been effective so far but also has several drawbacks:  * the extent of coverage that can be offered is limited by the underwriters' available capital * leverage is necessary for the underwriters to be compensated adequately, which raises the possibility of bankruptcy * determining the premium prices is challenging given the limited data and fast-paced nature of the industry.

 Reciprocal insurance, on the other hand, does not charge premiums, and payments are only made when a loss occurs in
one of the vaults of the ecosystem. At that point, a small percentage of every vault is liquidated to compensate the affected vault.
 This system operates like a reciprocal inter-insurance exchange, in which users/subscribers essentially cover each
other against risk. However, all policies are transparent, with no premiums being paid in advance, and there is no reserve capital. This eliminates the complications associated with traditional coverage, such as risk-based pricing, premiums, underwriting, supply issues, solvency and more.
 This approach ensures that users pay only what is necessary, without any additional costs, no profit for
underwriters and no concern of insolvency.
 
 **How RCA is different from traditional Insurance**        
### How RCA is different from Traditional Insurance
|                                                                    Traditional Insurance                                                                   	|                                                                                                                            RCA                                                                                                                            	| |:----------------------------------------------------------------------------------------------------------------------------------------------------------:	|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:	| | Premiums are paid upfront to cover the assets                                                                                                              	| No upfront or continuous premiums are required to maintain the coverage                                                                                                                                                                                   	| | High capital is needed to make the protocol profitable                                                                                                     	| No large amounts of initial funding required. Fund's in the ecosystem underwrite themselves                                                                                                                                                               	| | Premiums are charged periodically till the duration of the policy                                                                                          	| User will be charged only when loss event occurs                                                                                                                                                                                                          	| | Capital Providers provide capital that can be used by the insurance company to pay off the claims.                                                         	| Capital is pooled by the insured. So if there is no claim, the pool remains the same and people who get the cover end up paying almost nothing.                                                                                                           	| | For selling the insurance user's asset doesn't need to be verified.                                                                                        	| To include a user/protocol in the coverage, assets need to be verified.  In DeFi since user or protocols have full custody of their assets, RCA is simpler to implement in DeFi as compared to other industries because assets can be verified on chain.  	| | In case some user/customer in the insurance company loses funds, it doesn't impact other insureds.  As each insured pays premiums only for their coverage. 	| If anyone in the pool loses funds, every other party in the pool can be impacted. If the number of users or participants is very high, the impact should be very low                                                                                      	|
              
 
 **How Ease works**        
### How Ease works
The Ease protocol is a decentralized insurance platform that utilizes smart-contracts, known as vaults, to store and insure assets.  One of the key features of the Ease protocol is that assets are covered reciprocally, which means that there are no initial expenses  for coverage and no premiums required. Instead, remuneration is only disbursed in the event of a claimable occurrence, and a minimal  sum is drawn from each vault to repay the loss, which can be denominated in either Ether or a stablecoin.
The vaults in the Ease protocol act as a smart-contract that stores user's assets and mints ez-tokens as a proof of deposition.  These vaults also participate in the coverage of other vaults in the event of a claimable occurrence. The loss incurred by  each vault is computed by taking the same percentage of funds from the vault's value as the total funds lost from the overall  value of all vaults. This is represented mathematically as Li = Vi * TL / TV L.
The RCA (reciprocally covered assets) model used by the Ease protocol distributes the loss across all vaults. If there is a  loss in one vault, it is covered by the other vaults in the system. This makes the Ease protocol a more efficient and  cost-effective way to insure assets when compared to traditional insurance methods that require underwriters to cover the assets.
When a hack occurs, the admin of the Ease protocol will freeze the reserve amount in each vault according to their maximum fee.  This amount won't be available for withdrawal. The admin will then set the amount to be liquidated from the reserve amount, which  will be unique to each vault and based on the safety ranking and total loss from the hack. The DAO (Decentralized Autonomous Organization)  votes and confirms the liquidation of assets for each vault. 
For example, if we have 10 vaults with equal values rated from riskiest to safest, a hack occurs that affects 0.1% of the ecosystem, and the maximum percent that can be liquidated from each before moving onto the next is 0.5%, we will liquidate the maximum from the 2 riskiest vaults before the loss is fully compensated. If the hack affected more than 0.5% of the ecosystem, the liquidations would simply loop back around to the riskiest protocol and continue, so a hack affecting 0.75% of the ecosystem would end up liquidating 1% from each of the riskiest 5 protocols and 0.5% from each of the safest 5 protocols.
 
 **Claim Assesment and guidelines for coverage**        
### The Conditions or guidelines for Coverage of assets
* In the event of a deliberate manipulation of the Oracle system that causes panic or unauthorized withdrawal of assets, resulting in a crash, assets are covered.
* In instances where there is a discrepancy from intended data sources that leads to Oracle failure, assets are covered.
* If the code is used in a malicious or unintended manner, resulting in the withdrawal of assets from the protocol stack, assets are covered.
* If there is an economic design failure that results in the unintentional confiscation or seizure of underlying assets deposited into the  top protocol or stack directly by the RCA vault, assets are covered.
* In the case of a deliberate governance attack, the decisions in the Ease protocols are made by the DAO and there is a possibility of attack  by the governance, assets are covered.
* In the event of a privileged authority acting in bad faith (such as a rug pull) resulting in unnecessary or unintended withdrawal of assets,  assets are covered.
* If there is negligence or a lack of proper security measures by someone with privileged authority within the framework of a protocol that results in the  withdrawal of assets without the proper owner's knowledge or permission (e.g. a phishing attempt compromising an administrator's credentials, resulting in  loss of assets from the protocol directly), assets are covered. 
It is important to note that these guidelines and the decisions made based on them will be determined by the DAO.

### Claim Assessment
In the event of a security breach or hack, also known as a "covered event," protocol will be implemented to safeguard all assets stored in the vaults. The claims process will be initiated immediately upon the occurrence of a covered event, during which all assets will be frozen to prevent unauthorized liquidation. The liquidation of these frozen assets will be conducted in order to compensate for any losses sustained. Claim payouts will be distributed in the form of Ether or other fiat-denominated stablecoins to the affected vaults. Following the claims process, users will regain access to their assets and will be able to withdraw them.
The claims process in this system is designed to be simple and efficient, as the losses incurred are directly tied to the vaults rather than individual users. As a result, there is no need for claimants to provide proof of loss in order to receive coverage. Losses can be immediately verified by evaluating the impacted vaults, allowing for swift compensation. The Decentralized Autonomous Organization (DAO) will vote on the appropriate amount to be paid to each affected vault, and once the funds have been allocated, the frozen assets will be unfrozen and made available for withdrawal.
The value of a vault after a hack covered event or after a hack is given below
New value of vault = N
Old value of vault = O
New total value locked in RCA = C<sub>N</sub>
Old total value locked in RCA = C<sub>O</sub>
then,
N = O*C<sub>N</sub>/  C<sub>O</sub>
 
 **Tokens**        

### $EASE
The $EASE token is a tradeable Ethereum-based (ERC-20) token with a finite supply. It offers various levels of utility in the Ease DeFi Uninsurance system. The Ease tokens can be used for bribing. It can be staked to get the $gvEASE tokens.
Since Ease is the upgraded version or next version of ArmourFi, the supply of $EASE and $Armor stays the same. The Armour tokens can be swapped for ease in 1:1 ratio.

#### History of $EASE token
1 billion Ease tokens were initially minted, but 250 million were sent to a burn address. The remaining 750 million $EASE is the maximum supply, but 250 million $EASE can be minted through a contract. This can only happen after a DAO vote, and even the team cannot mint extra tokens. The Ease DAO will control the majority of the tokens, i.e. 400 million.

### $gvEASE
The $gvEase tokens are minted by staking the $Ease tokens. These are growing vote tokens which will grow in time.
The $gvEASE token is a unique digital asset that offers a number of properties for users to take advantage of. Firstly, it is not tradable, meaning it cannot be bought or sold on any market. However, the staked Ease tokens can be withdrawn at any time, giving users the flexibility to move their funds as they see fit. However, it is important to note that if the $EASE is withdrawn, the user will receive the $EASE tokens but any additional $gvEASE will be lost.
Another unique property of the $gvEASE is that it can be stacked in vaults. By doing so, the maximum fee is lowered for the vaults, which is the maximum possible fee that can be deducted in case of hack events. Additionally, users can also lease their $gvEASE tokens and earn weekly $EASE rewards. This is a popular option among vaults that have very low maximum fees, as they can earn rewards while still having their $gvEASE available to them for use in DAO voting.
It's important to note that $gvEASE tokens can only be used for staking, not for DAO voting. This is because the ownership of the token remains the same, regardless of whether it is being used for staking or voting. In other words, the briber can only use $gvEASE for staking, but not for participating in DAO voting. This ensures that the integrity of the DAO voting process is maintained.
The main uses of $gvEASE tokens
* $gvEASE tokens are used for DAO voting.
* $gvEASE tokens are used for staking in the vaults which will reduce the maximum fee.

### Bribes and Leasing
Users who want to reduce the maximum fee for their desired vaults can offer $EASE tokens as a bribe to $gvEASE holders. Protocols or users interested in reducing their vaults' max fees can buy $EASE tokens and offer them to $gvEASE holders as a bribe. Bribed $gvEASE cannot be used for DAO votes.
The users can lease their $gvEASE tokens to get weekly $EASE rewards. The leased $gvEASE can be used for staking, but it cannot be used for DAO voting. Mostly, the vaults with very low maximum fees will lease $gvEASE tokens.
 
 
