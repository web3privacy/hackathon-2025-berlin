# [Zero-Sig]

- **Track(s):** [Advanced Crypthography, Applied Encryption]
- **Team/Contributors:** [Frank & Drone]
- **Repository:** [https://github.com/builders-garden/zero-sign-frontend, https://github.com/builders-garden/ZeroSig-smart-contracts, https://github.com/builders-garden/zero-sign-circuits]
- **Demo:** [[video](https://www.youtube.com/watch?v=D2W7NF2qqqQ&feature=youtu.be)]

## Description (TL;DR)
[Zero-sig is a privacy-focused multisignature solution. It enables users to vote and propose actions while keeping their identities and actions hidden from both other participants and external observers.]

## Problem
[While multisignatures are powerful tools, they come with significant privacy concerns. Current implementations expose sensitive information about signers - their addresses, voting patterns, and participation status. This lack of privacy can lead to serious issues like social engineering attacks, bribery attempts, and coercion, phishing attacks, potentially compromising the freedom of action and speech of participants.


]

## Solution
[We use Noir circuits to implement zero-knowledge proofs that protect privacy at multiple levels. Our solution ensures that:
1. External observers can't see who's participating
2. Even other signers can't determine who has voted
3. We verify signer authenticity without revealing identities
4. A recursive circuit validates that enough votes are collected based on the contract's threshold]

## Technology Stack
[Next.js, Noir, Solidity, Safe, MagicValue]

## Privacy Impact
[The lack of privacy in traditional multisigs creates numerous vulnerabilities. From bribery and coercion to stalking and targeted attacks, the risks are real. Our solution ensures that everyone can exercise their right to vote or approve actions without fear of retaliation or unwanted attention.

More over zero-sig could prevent adversaries from mapping onchain activity to specific individuals or organizations, reducing surveillance and correlation attacks across wallets or DAOs.

It more importantly enable anonymous signing for high-impact or politically sensitive transactions (e.g., donations, whistleblower support, activist funding) without compromising operational security.
]

## Real-World Use Cases
[Our private multisig solution can significantly enhance security and privacy for various scenarios. Whether it's protecting against financial coercion, preventing bribery attempts, or maintaining operational security, hiding signatures from both internal and external observers can be transformative for many organizations and individuals in today's world.]

## Business Logic
[We dont care about business]

## What's Next
[After 30+ hours of intense development and sleep deprivation, we're looking forward to enhancing privacy features even further. The journey continues!]