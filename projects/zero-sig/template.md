# [Zero-Sig]

- **Track(s):** [Advanced Crypthography, Applied Encryption]
- **Team/Contributors:** [Frank & Drone]
- **Repository:** [[frontend](https://github.com/builders-garden/zero-sign-frontend), [contracts](https://github.com/builders-garden/ZeroSig-smart-contracts), [circuits](https://github.com/builders-garden/zero-sign-circuits)]
- **Demo:** [[video](https://www.youtube.com/watch?v=D2W7NF2qqqQ&feature=youtu.be)]

## Description (TL;DR)
Zero-sig is a privacy-focused multisignature solution. It enables users to vote and propose actions while keeping their identities and actions hidden from both other participants and external observers.

## Problem
While multisignatures are powerful tools, they come with significant privacy concerns. Current implementations expose sensitive information about signers - their addresses, voting patterns, and participation status. This lack of privacy can lead to serious issues like social engineering attacks, bribery attempts, and coercion, phishing attacks, potentially compromising the freedom of action and speech of participants.

## Solution
Our solution is built on Safe multisig and Noir circuits, enabling zero-knowledge proofs that protect privacy at multiple levels.

We developed a "zkOwner" contract, which is the sole owner of a Safe multisig wallet (1-of-1 configuration). This zkOwner contract implements EIP-1271 for validating smart contract signatures. It includes custom logic for verifying Noir-based proofs and implements the isValidSignature function.

As a result, every transaction executed through the Safe smart account must be approved by the zkOwner contract, which verifies a recursive zero-knowledge proof. This proof ensures that a hidden signature from an authorized signer (or signers) meets the required threshold, without revealing their identity.

Key Privacy Guarantees:
External observers cannot see who is participating
Even other signers cannot determine who has voted
Signer authenticity is verified without revealing their identity
This approach ensures secure, privacy-preserving governance and transaction approval.

## Technology Stack
Next.js, Noir, Solidity, Safe, MagicValue

## Privacy Impact
The lack of privacy in traditional multisigs creates numerous vulnerabilities. From bribery and coercion to stalking and targeted attacks, the risks are real. Our solution ensures that everyone can exercise their right to vote or approve actions without fear of retaliation or unwanted attention.

More over zero-sig could prevent adversaries from mapping onchain activity to specific individuals or organizations, reducing surveillance and correlation attacks across wallets or DAOs.

It more importantly enable anonymous signing for high-impact or politically sensitive transactions (e.g., donations, whistleblower support, activist funding) without compromising operational security.

Think about donations toward good causes that might be politically sound to do publicy


## Real-World Use Cases
Our private multisig solution can significantly enhance security and privacy for various scenarios. Whether it's protecting against financial coercion, preventing bribery attempts, or maintaining operational security, hiding signatures from both internal and external observers can be transformative for many organizations and individuals in today's world.

## Business Logic
We dont care about business

## What's Next
After 30+ hours of intense development and sleep deprivation, we're looking forward to enhancing privacy features even further. The journey continues!