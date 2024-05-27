# PURE: Payments with UWB RElay protection

This project accompanies the paper [pure](https://www.research-collection.ethz.ch/handle/20.500.11850/662474) published at USENIX 2024. 
In this work we invstigated the integration of UWB secure ranging into the Mastercard kernel with the goal of preventing relay attacks. 
We refer to the paper for the details of the proposed protocol and a presentation of the results.

## Relay Attacks
With the emergence of contactless payments, the awareness and the threat of relay attacks on card payments havealso increased.
In the simplest relay attack, the victim does not intend to use their card (e.g., it is in their wallet) but an attacker establishes a relay channel between the victim’s card and a terminal
of the attacker’s choice, thereby charging the victim’s card for the purchase. In more sophisticated relay attacks, similar to the chip-and-PIN fraud, an attacker plays the role of a
(malicious) merchant who presents a fake terminal to the victim customer. By relaying the communication, and even the victim’s PIN, the attacker can use the victim’s card to
pay for more valuable goods at a legitimate terminal or towithdraw a large sum of money from an Automatic Teller Machine (ATM).

## Content
This project constains two repositories: 
- `pure-poc`: contains the proof-of-concept code which can be run on android phones equipped with UWB boards.
- `pure-sec-rel`: contains the analysis of the proposed protocol in terms of reliability and security.

## Usage

Use the `pure-poc` repository to run a mock UWB protected transaction.
Use the `pure-sec-rel` repository to analyze the collected data.
Follow the README in the respective repositories for further details.
