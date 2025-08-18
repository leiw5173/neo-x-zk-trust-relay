# neo-x-zk-trust-relay

This is a repository for Neo X ZK-DKG MPC ceremony, please refer [bane-labs/zk-dkg](https://github.com/bane-labs/zk-dkg) about the tool and [neo-x-mpc](https://github.com/bane-labs/zk-dkg/blob/main/neo-x-mpc.md) about the steps.

## Information

|Name              |Property |
|------------------|---------|
|Proof System      |`Groth16`|
|Power of Tau      |`2^24`   |
|NeoFS Network     |`Mainnet`|

## How to Contribute

Please contribute the MPC file according to the order, upload the result through NeoFS, and provide following information through **pull request**:

1. Result file challenge, you can get it from the `zk-dkg` command line output after computation;
2. NeoFS object ID, you can get it from the `neofs-cli` command line output after file upload.

After all of the MPC contributions, NGD will backup the results to cloud, so please leave the `Cloud URL` field as empty in pull requests.

## Phase1 Attestations

### Existing contributions

Container ID: `411d8vuzogogMxXJqTQcu61btgQ6rL2VNYUYnH7r4kE3`

|Participant|File Challenge                                                    |NeoFS Object ID                               |Cloud URL                                                        |
|-----------|------------------------------------------------------------------|----------------------------------------------|-----------------------------------------------------------------|
|NGD        |`071d2176b99861f97e57020cd5ef3904299fffb1fdb8bf0994d9bbf5e36f60ad`|`4t51oBmnwu3UHpC35HAS3aoF2jcMtjmpL9df7vZR447r`|https://zkstorage.blob.core.windows.net/zk-blob/Phase1_1_NGD     |
|NSPCC      |`3446c3cc02a91df93846621f7b9d3641ca2638a0c959e2b5e03bc37823f27625`|`4QNXbGzU3ooJgpsR7EVawyKgtrQSDDw5BwdLYeND9gZT`|https://zkstorage.blob.core.windows.net/zk-blob/Phase1_2_NSPCC   |
|AxLabs     |`4a7b705174f35e07672dbf3271cb2dfe2948b2861df4b7e98fece41fe8c3f21e`|`CpbUnRe4qnxQZQH1SrKqCuCXo8aBis4HsuKDeN2ghB6w`|https://zkstorage.blob.core.windows.net/zk-blob/Phase1_3_AxLabs  |
|Lazynode   |`2a9d15f8d5dbf0117b4cbb7fd43f41ccd1be3c9409e3d6f7da4964aa6447547c`|`8q5JMQ6x3ELp2XkLeqtGpGGHEiqgvRXL4a6AyHHvobi2`|https://zkstorage.blob.core.windows.net/zk-blob/Phase1_4_Lazynode|

### New contributions

|Participant|File Challenge                                                    |NeoFS Object ID                               |Cloud URL|
|-----------|------------------------------------------------------------------|----------------------------------------------|---------|
|           |                                                                  |                                              |         |
