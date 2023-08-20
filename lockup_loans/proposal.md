# Introduction
I'm Anunay, I've contributed to [hsd](https://github.com/handshake-org/hsd) in the past in a few small ways ([1](https://github.com/handshake-org/hsd/pull/639), [2](https://github.com/handshake-org/hsd/pull/651)).

# Proposal
## Lockup Loans
*or Staking on Handskake*

Bids on the Handshake network can be masked using a higher lockup amount than the bid itself, refunding the difference (aka the blind) after the auction. This conceals bids to avoid getting outbid by a dollarydoo, but still sets an upper bid limit and ties up funds.

## Solution

Since the blind (`lockup_value` - `true_bid`) is refunded to the user post-auction. One can issue a "loan" of that amount for the duration of auction. This benefits those with surplus holdings, letting them earn interest (similar to "staking"), while boosting bidder privacy.

## But can it be decentralized?

Doing so on a centralized platform is pretty straightforward. However, pinheadmz suggested a possible approach to do this in a non-custodially during the last handycon. Unfortunately nobody really came forward with a implementation because of the immense complexity of the project.

I have a slightly modified from original approach documented [here](https://gist.github.com/Anunayj/750c85c9bea6a707e7e32a72f9ef6e83). Much of the ideas used here are thanks to Matthew Zipkin and Fernando Falci.

[Original Approach by pinheadmz](https://gist.github.com/pinheadmz/644870fa2c08ea19ff373bf70bf425e8).

# Completion Criteria
1. Research, and document possible approaches. (A HIP possibly)
2. Implement a reference implementation (a integration test perhaps) covering all edge cases.
3. (Optional) Implement a library that can be used by various wallets (and stakers) to facilitate lockup loans.

# Timeline
I understand the project timeline is limited to a maximum of 4 weeks. However, considering the complexity and potential impact of this project, I suspect it would take atleast 8 weeks to ensure a thorough and well-tested implementation. This proposal can possibly be split into two (or more) parts (possibly worked on by multiple people!?): Research, Documentation and Implementation.

# Sidenote
It's crucial to acknowledge the potential dangers posed by any flaw in the implementation. A critical flaw could result in irreversible loss of funds. Rigorous testing is essential to mitigate the risk of such flaws, and honestly I feel a little unqualified to do this alone.

# Contact Information

Email: me [at] anu [dot] ninja
Discord: @anu9001
Telegram: @anunayj