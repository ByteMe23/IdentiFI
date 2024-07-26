# IdentiFI

Introduction
The current digital identity landscape is often fragmented and insecure, making it challenging for users to manage and verify their identities across different platforms. identiFi was inspired by the potential of blockchain technology to create a unified, secure, and verifiable digital identity solution that empowers users to manage their identities seamlessly.

Tech Stack
Next.js
TypeScript
Solidity
Hardhat
Chainlink VRF
IPFS

Features
Decentralized Identifiers (DIDs): Create and manage unique DIDs on the blockchain.
Identity Verification: Submit identity documents for verification by trusted third parties.
Credential Verification: Verify the authenticity of credentials.
User Profile Management: Update personal details and manage credentials easily.
Privacy Controls: Control who can access identity information and under what circumstances.
Security Measures: Strong security measures including encryption and secure key management.
Social Media Integration: Share your verified digital identity on various social media platforms.
Profile Editing: Easily update and manage your digital identity profile.

Quick Start
Follow these steps to set up the project locally on your machine.

Prerequisites

Make sure you have the following installed on your machine:

Git
Node.js
npm
Hardhat
Metamask (or any other Ethereum wallet)
Chainlink VRF setup
IPFS setup

Install the project dependencies using npm:

npm install
Compile the Contracts

npx hardhat compile
Deploy the Contracts

npx hardhat run scripts/deploy.js --network yourNetwork
Run the Development Server

npm start
Open http://localhost:3000 in your browser to view the project.

Smart Contract Overview
The main contract, IdentiFi, manages user profiles, DIDs, and credentials.

Key Functions
createUser: Creates a new user profile and requests a new DID using Chainlink VRF.
editUser: Edits an existing user profile.
getUserByUsername: Retrieves user information by username.
getUserByAddress: Retrieves user information by address.
addJob: Adds a job to the user's profile.
getJobs: Retrieves jobs associated with a user.
setVisibility: Sets visibility preferences for user profile information.
getVisibility: Gets visibility preferences for user profile information.
batchCreateUsers: Batch creates multiple user profiles using Monobean.

Storing Images on IPFS
User images are uploaded and stored on IPFS. This ensures that images are stored in a decentralized manner, enhancing security and accessibility.
