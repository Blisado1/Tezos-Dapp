# Auction-Contract
My project for tezos tacode course <br  > 
This is a simple contract that implements an auction, where users can place bids and the bids must be higher than the current bid in storage, and after someone's bid has been outbid, the contract refunds the outbid person, and replaces their details with that of the current highest bidder.

## Storage example
```
Map.literal [ 
(0n, {
  auction_end : 300000000000000000;
  highest_bid : 0.5tz;
  bidder : "tz1Wv5x5MWbBBYPD6JB6ZTZfWNfg9SsTuy9h";
  no_of_bids : 4n});
(1n, { 
  auction_end : 600000000000000000;
  highest_bid : 1tz;
  bidder : "tz1Wv5x5MPBBYPD6JB6ZTZfWNfz9SsTuy9h";
  no_of_bids : 4n }) ; ]
```
