---
description: >-
  In case the front-end get any UI error or the RPC you have been using become
  congested, you could continue your works by interacting with contracts
  directly on blockchain explorers.
---

# How to interact directly with QiDao’s contracts

<figure><img src="../.gitbook/assets/Frame 3(3).png" alt=""><figcaption></figcaption></figure>

## Step #1: Find an address of your vault

Since you have to interact with a contract on blockchain explorers, it is necessary to find the exact addresses of the vault. QiDao has dedicated a specific and actively updated page for important addresses that you could find [here](https://docs.mai.finance/functions/smart-contract-addresses). Scroll down to find the vault address you wish to interact with, which has been already categorized into network sections.&#x20;

![](https://lh4.googleusercontent.com/WP5i\_AzGolnjMaulNuBMI6fU-nlpJx6-mr6PKm2vM5y43i3Uvi27E5Qo9Ny0WuM6qiZPCwtR7TtvhPkecuyStX924vqIh9OPkVy4QA8ZsoQgBBR4ukBHJvxh-fQ1dN7CS0yKY6gSJ-Vz-xYdqfJta3vN0di7wRpUi\_tCTucqa6B5vfhD8hplLR70vcjwpcVUuNuBPbLPLg)\


In our guide, we will take the address of WETH V1 vault and OP V2 vault on Optimism as an example due to the recent raising demand for such vaults on Optimism network.&#x20;

**WETH Vault**

0x062016cd29fabb26c52bab646878987fc9b0bc55

**OP Vault**

0xbf1aea8670d2528e08334083616dd9c5f3b087ae

## Step 2#. Go to a block explorer

Blockchain explorer is a blockchain search engine that allows people to retrieve information about transactions, address, blocks, fees, and more. By using simple operations, you could extract useful information and interact directly with a smart contract under the _Write Contract_ tab.&#x20;

1. Go to a specific blockchain explorer. For example [https://optimistic.etherscan.io](https://optimistic.etherscan.io)
2. Paste the address of vault you want to interact.&#x20;

For exmple: 0x062016cd29fabb26c52bab646878987fc9b0bc55

![](https://lh3.googleusercontent.com/qEKIEWexE2rcj\_Wv1NYEeKYXW70oA3uAII-vjAxkzRDF62Zle5Aqbem99RxgjpkESlLGMbl3U7pHX-FE-zXi53gbEwGjmmzk3Nf8E6icUK\_qWZnsmGps1XVgPdJJmrgI3Bw\_wq1a3O6pWyDJ5G-cxAs94ebt\_r0Oxyv7k5dPJk2m9Ht84x6WXTqBMo-Q81XHPOLJ1MtNuQ)

3\.  Direct to _Contract_ tab then go to _Write Contract._

![](https://lh3.googleusercontent.com/m0GqF-tQNjhoA9yRxcpbDKInq9jWutcJMvY1cYSO4BTNzuiahP-4268XRqxXtZoWkWjU1rfKyx3aDWHYhfxpINlIvlwahoqDM7DseG0\_Wck2yo8\_aTyi-D2czYJgt-v3bi0bETpDdcvby3SpoAa4wEk0RD06ze39pt\_ILwok6ugFe0kxJ9iT8K3aIYw78H2Lv4KieII0nA)

_4.  Connect_ your wallet. For example MetaMask

![](https://lh5.googleusercontent.com/GvgFrgPGIzJ\_r64Y1PXN9IvyhEEb-bPrlNT38SJxGGtym\_WDmjYwKqg3twrIsdtUKDdCUY7-SExjTlJPCu-mBt45\_t6iWTUUVK0I5iCl1vAtpQ67rV1dEeVV6CA95j-HRDiZ\_OTdL-VsyeyHizUyhtp2OATV8QNT5V3RreN2vz0siLl3mQ1FL8cNSozOj5OiUKgDxIIX4g)

_**NOTE**_: Refresh the page if the page doesn’t show its connected wallet.

## Step #3: Interact with a smart contract.

After your wallet connection is completed, there are numerous ways to interact with a contract similar with front-end interactions including vault creation, MAI borrowing, repayment, collateral withdrawal… In this guide, we will use the payBacktoken function as example.

![](https://lh4.googleusercontent.com/A5WAF-9yNuOQh6KfumdSzKhk78puR8ixOppriAEpY31BpX\_ZEVOrW9YGH56TSOJ-jCuUCG14Yfh-CtZ3Z3fViqGc0AnAeD04tS69W90juS5nbRE0bpV8aGdJnDupW81JQmwenPIBlPwXv0EIXJg3yEkpbMLLia9Me17Rb\_X2U\_88VS6ecTNHCZ6Yjdyz5JvDYRs5xUSNNA)

1. Find your vault ID at Manage tab on your vault page on the website to put into \_vaultID space.

![](https://lh4.googleusercontent.com/HXENd4eDyk1wXyGtbVFt9\_BKVVl5FNEuy4v-l\_Q7opn\_Z4\_TcvvS4JfYw0S2zphpNZFEOsQUTPax7WFyEAYYavQydhlEbgPmd8xWU591pKOFy1T1Cimng9-Y248kGCQjNVqyU3vQWDzm2-9K8cu\_Sgi5WWI8sg88TAJ37WoCBq8wQKWIsT-BOrjVd-PRC\_hPEjp0W4E3Tw)

2\.  Write the amount of token you want to repay.\
_**NOTE:**_ The amount of token which you need to deposit/withdraw/repay followed by 18 decimal spots. Therefore, you need to adjust the number format before adding any number by using the automatic convert feature on blockscan as the following pictures show:

* Press the cross button on the amount(unit256) section.

![](https://lh5.googleusercontent.com/jDOZq9rwhAf2JIrvG5TF18wNaA1TlJEXafW033PTq6zVvMBaNEXHKGyvNqB55TH8eZ7KmBZXMm3UDLjEt\_OUeg\_SgHdbjejiNLriPRu9nkfHVmfAZRg4iw\_VlrIhvwoiDubyO3VtE-vALdYMNB8MQq40uFYi25yaZHkNyPbg\_nnXrCKLwUSM\_R9TpT0U1wYf)

* Select the 10 ^18  format for allowing blockscan automatically converts your number.&#x20;

![](https://lh3.googleusercontent.com/AHAwdT9nDNx-3RIwzJlGQqLJ9NF9VhrW2pbHcoVIPchvKLvUa6CS3NFlkhWuF0l\_9ux0MHVcA31HLAUDoD2l-s\_Kfycw17Hk4zk8d6ORTN1ff8KVcyH5Rjmeqv-DqABvwWOzWdpGiqK97asRpdc9dj-wJENcfasA-n6U-LOxXMKedUY7sfbvLcU63C6pc9Qb)\


In case of QiDAO’s V2 contracts (screenshots below), there is an additional space called \_front(unit256) where you also have to put a number zero (0) in order to the function be enable.

![](https://lh5.googleusercontent.com/J9erStzzUEm8Aa22EIu7IkG71HjNx-rXnwUV5aSyaHPwyFJl4FRvtsDDyVoW8FiXzt0acG\_Fgr1GPvfFjcuWnXq8numno05OJVUkFw09UkfW3eZ0ukao29gWmtSaAldcvnVi9Gk2loHOIeDQ8uDHmldPej6q9i5jmvctV3TCUAyhcgm-WoBuhCMg2Mjnu7LI)&#x20;

![](https://lh3.googleusercontent.com/Z7dZCgoAZeG8\_uxj4EqORhA0wzIqHFk7rtkLKn7P44lJeJOEWQEFjpjnPLGHJLfLSy2RWw2KH3PvfWchLrxaYoPpof1sfwDPWLSYAH\_VLjJnE1nlAyx3i9EarbG-qRxfG5WC\_YZRpvRLIV7mWgOFYfpWGSveqJvOuArSXvRMsAgYTCOiuCRcjtDP4TXuMmpq)

3\.  Press _Write_ to proceed your transaction as normal.&#x20;

## Conclusion

We showed the _WriteContract_ features on Optimism, as an illustration, to assist users in interacting with any smart contract deployed by QiDao, which is also on any currently supported EVM blockchain. You should be more careful about the amount token you want to proceed followed by 18 decimal spots. Make sure you write the number correctly in the first time which will save you plenty of gas fees.&#x20;

