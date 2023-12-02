The whole project is composed of these files:


-FundMe.sol:

    It is a smart contract that:

    -Can be funded, but the amount that is going to be funded should be greater than a set limit of USD

    -Tracks all of its funders amd the amount its one of them has totally funded

    -Only the owner of the smart contract can withdraw all the money inside it


-PriceConverter.sol

    It is a smart contract contract that:

    -It is used by the FundMe contract in order to convert ETH amounts in USD


-DeployFundMe.s.sol

    -It deploys FundMe contract


-HelperConfig.s.sol

    -It is used by FundMe in order that we get the correct price feed of the ETH/USD pair in the network that we want to use


-Interactions.s.sol

    -It contains functions with which we can fund FundMe(most_recently_deployed_contract) and the Owner to Withdraw from FundMe


-FundMeTest.t.sol

    -It include tests the FundMe contract 


-InteractionsTests.t.sol

    -It includes test for the contracts of the Interactions.s.sol file