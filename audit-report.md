# Audit

### Overview

We have researched the current market of blockchain security solutions and came to the conclusion that the auditing standards of the [Obelisk](https://obeliskauditing.com) team are the most suitable for us and our community. Argano team has contacted Obelisk on the _**25th of June**_ in order to start the auditing process. The audit was conducted between the 1st of July 2021 and the 31st of August 2021 and delivered on the 4th of September 2021.

The auditing process was divided into the next parts: manual analysis, static analysis, and on-chain analysis.\
\
During the Obelisk review, Solidity specialists were very attentive to each possible issue and proposed different ways of solutions**.** Obelisk representatives were communicative and went to a meeting to solve existing problems. As the result, they have covered all possible vulnerabilities which were successfully fixed from our side.\
\
A valid audit report can be reached by the [**link**](https://github.com/Tibereum/obelisk-audits/blob/main/Argano.pdf).

{% file src=".gitbook/assets/argano.pdf" %}
Download audit report
{% endfile %}

### **Details**

We have provided comments concerning the following issues:

#### #0021

> ”The main governance token $AGO is minted to the EOA wallet with privileged possibilities in order to manage correct token distribution according to the latest tokenomics featured in the documentation. This was made due to the fact that we didn’t establish a partnership with the fundraising platform at the moment of the audit process.”

#### #0042

> “Community allocation will be minted directly to pools. After defining the reward distribution strategy, the reward controller will be transferred to a special contract to track all token mints. Share tokens will be minted during redeeming. If the hard cap is reached the only way to get back your USDT is just to sell into the pair (if the token price is pegged). We will apply new stimulating pricing strategies in addition to the existing foundry staking.”&#x20;
>
> Obelisk comment: “It may be challenging to change the reward controller. We recommend minting a fixed amount, storing that in a community controlled contract (eg. a DAO), then revoking ownership of the share contracts. While the reward controller is an EOA, the owner of the share contracts is a timelock. This will provide users with advance notice that community rewards are being minted.”

#### #0046

> "Pair oracles will be initialized when the appropriate liquidity pairs will be created. This will be verified once the project launches" - Obelisk.

### Timelock

For deeper security, we have transferred ownership to the Timelock contract and set the 48h delay:

* [Timelock deployment](https://polygonscan.com/tx/0x88b70af7a65b582f6f91164016a984a3087a7f0ca866aa13574305af6b347ece)
* [Set delay](https://polygonscan.com/tx/0x15faa4c95c29b628389ed917990e3b76c3254d35724ac279edc2803d3401419a)

### Hard Cap

Share tokens both for USD and BTC pegged tokens play important role in the algorithmic part. CNUSD & CNBTC tokens have a limited supply, which will prevent unlimited token generation. Together with the stimulating pricing strategies share tokens would never lose their value in the protocol.

Parameters:

* CNUSD: `80,000,000`\
  ****
* CNBTC: `8,000`

####

