# Sample contract of VRF consumer

There are 2 types of contract to get a random number
## VRFConsumer (Subscription Method)
VRF requests receive funding from subscription accounts. The Subscription Manager lets you create an account and pre-pay for VRF, so you don’t provide funding each time your application requests randomness. This reduces the total gas cost to use VRF.

see more in file `contracts/sample/VRFConsumerSample.sol`

## VRFWrapperConsumer (Direct Fund)
Unlike the subscription method, the Direct funding method does not require you to create subscriptions and pre-fund them. 

Instead, you must directly fund consuming contracts with KDEV tokens before they request randomness.

see more in file `contracts/sample/VRFWrapperConsumerSample.sol`
