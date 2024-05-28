# PURE: Payments with UWB RElay protection

This project accompanies the paper [pure](https://www.research-collection.ethz.ch/handle/20.500.11850/662474) published at USENIX 2024. 
In this work, we investigated the integration of UWB secure ranging into the Mastercard kernel with the goal of preventing relay attacks. 
We refer to the paper for the details of the proposed protocol and a presentation of the results.

## Why should UWB be integrated in EMV?

In short, to prevent relay attacks.
With the emergence of contactless payments, the awareness and the threat of relay attacks on card payments have also increased.
In the simplest relay attack, the victim does not intend to use their card (e.g., it is in their wallet) but an attacker establishes a relay channel between the victim’s card and a terminal
of the attacker’s choice, thereby charging the victim’s card for the purchase. 
Our work prevents relay attacks by integrating a secure ranging scheme in the  Mastercard Kernel which provides an upper bound (41 cm) on the distance between the card and terminal.

## Content
This project contains three repositories: 
- [pure-poc](https://github.com/pure-uwb/pure-poc): contains the proof-of-concept code which can be run on android phones equipped with UWB boards.
- [pure-sec-rel](https://github.com/pure-uwb/pure-sec-rel): contains the analysis of the proposed protocol in terms of reliability and security.
- [pure-models](https://github.com/pure-uwb/pure-sec-rel): contains the Tamarin models used to formally prove the security of the proposed EMV extension.
  
Follow the README in the respective repositories for further details.
