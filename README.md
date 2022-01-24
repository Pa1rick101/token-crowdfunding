# token-crowdfunding

Crowdfunding campaigns such as Kickstarter are on the rise. Not only the number of succesfull fundings, but also the soaring number of frauds. Fashioning the new term: Fraudfunding. 

Blockchain has the ability to create trustless interactions which benefit both, entrepreneur and investor.


# Architecture

![Architecture](https://github.com/Pa1rick101/token-crowdfunding/blob/main/readme_images/crowdfunding-architecture1.png)


# Contract Details

| Variables   |      type      |  info |
|----------|:-------------:|:------|
| manager |  address | address of the person whi is managing this campaign |
| minContribution |    uint   |   Minimum donation required to be considered a contributor or 'approver' |
| approvers | address[] |    List of addresses for every person who has donated money |
| requests | Request[] |    List of requests that the manager has created. |

<br />
<br />

| Functions  |  info |
|----------|:------|
| Campaign |  Constructor function that sets the minimumContribution and the owner |
| contribute |   Called when someone wants to donate money to the campaign and become an 'approver' |
| createRequest  |    Called by the manager to create a new 'spending request' |
| approveRequest |    Called by each contributor to approve a spending request |
| finalizeRequest |    After a request has gotten enough approvals, the manager can call this to get money sent to the vendor |




