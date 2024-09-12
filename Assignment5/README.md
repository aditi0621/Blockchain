# Solidity Smart Contracts

This repository contains two Solidity smart contracts: one for a Crowdfunding platform and another for a Voting System. These contracts allow users to interact with Ethereum-based decentralized applications for crowdfunding and voting on proposals, respectively.

## Contracts

### 1. Crowdfunding Contract

The `q1.sol` contract allows users to create crowdfunding campaigns, contribute to them, and finalize the campaigns based on whether the target funds are raised by the deadline.

#### Features:

- **Create a Campaign:** Users can create a crowdfunding campaign with a target goal and a deadline.
- **Contribute to a Campaign:** Users can contribute funds to an active campaign.
- **Finalize the Campaign:** After the deadline, the campaign can be finalized. If the target is reached, funds are transferred to the campaign creator. If not, contributors can withdraw their contributions.

#### Functions:

- `createCampaign(uint _goal, uint _durationInDays)`: Creates a new campaign with a funding goal and duration in days.
- `contribute(uint _campaignId)`: Contribute Ether to a campaign.
- `finalizeCampaign(uint _campaignId)`: Finalize the campaign and either release the funds to the campaign creator or allow contributors to withdraw their funds.

### 2. Voting System Contract

The `q2.sol` contract allows users to create proposals, vote on them, and determine the winning proposal.

#### Features:

- **Add Proposals:** Users can create new proposals to be voted on.
- **Vote on Proposals:** Each user can vote once for a proposal.
- **Get Winning Proposal:** View the proposal with the highest number of votes.

#### Functions:

- `addProposal(string memory proposalName)`: Adds a new proposal to the list.
- `vote(uint proposalIndex)`: Allows users to vote for a proposal by index.
- `getWinningProposal()`: Returns the index of the winning proposal based on vote count.
- `getProposalName(uint proposalIndex)`: Returns the name of a specific proposal by index.

## How to Use

### Prerequisites:

- Install [Remix IDE](https://remix.ethereum.org/) for easy testing and deployment.
- Ensure you have a MetaMask wallet or any other Ethereum wallet installed if you want to interact with the contracts on a live Ethereum network.

### Steps to Deploy and Test in Remix IDE:

1. **Open Remix IDE:**
   - Visit [Remix IDE](https://remix.ethereum.org/).
2. **Create a New File:**

   - In the Remix file explorer, create two files named `Crowdfunding.sol` and `VotingSystem.sol` and paste the respective contract code into each.

3. **Compile the Contracts:**

   - Go to the "Solidity Compiler" tab and compile both contracts. Ensure you are using Solidity version `^0.8.0`.

4. **Deploy the Contracts:**

   - Go to the "Deploy & Run Transactions" tab.
   - Select **JavaScript VM** for local deployment or **Injected Web3** to interact with the Ethereum network.
   - Deploy the contracts by clicking the **Deploy** button.

5. **Interacting with Crowdfunding Contract:**

   - After deploying the `Crowdfunding.sol` contract, you can:
     - Call `createCampaign` to start a campaign.
     - Use `contribute` to contribute to a campaign.
     - Call `finalizeCampaign` to release or refund contributions after the deadline.

6. **Interacting with Voting System Contract:**
   - After deploying the `VotingSystem.sol` contract, you can:
     - Call `addProposal` to add a new voting option.
     - Use `vote` to vote on a proposal.
     - Call `getWinningProposal` to determine the proposal with the most votes.
