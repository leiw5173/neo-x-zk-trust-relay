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

1. Download the latest version of `mpc-cli` here: [zk-dkg](https://github.com/bane-labs/zk-dkg/releases/tag/v0.3.0);
2. Download the latest version of `neofs-cli` here: [neofs-node](https://github.com/nspcc-dev/neofs-node/releases/tag/v0.48.3);
3. Get the previous result file from the `NeoFS Object ID` field in the existing contributions, with the following command:

   ``` bash
   ./neofs-cli object get --cid <container_id> --oid <object_id> -r grpc://st3.storage.fs.neo.org:8080 --timeout 1000s --file <new_local_file_path>
   ```

4. Run the following command to get the result file challenge:

   ```bash
   ./mpc-cli phase1 contribute --phase1file <previous_file_path> --output <new_file_path>
   ```

5. Upload the result file to NeoFS and get NeoFS object ID:

   ```bash
   ./neofs-cli object put --cid <container_id> -r grpc://st3.storage.fs.neo.org:8080 --timeout 3000s --file <result_file_path>
   ```

6. Create a PR to update your file chanllange and Object ID.
    - Result file challenge, you can get it from the zk-dkg command line output after computation;
    - NeoFS object ID, you can get it from the neofs-cli command line output after file upload.
    - After all of the MPC contributions, NGD will backup the results to cloud, so please leave the `Cloud URL` field as empty in pull requests.
7. Wait for the PR to be merged.

## Requirements for Participation

- Operating System: A Linux or macOS system, or Windows Subsystem for Linux 2 (WSL2) if you are on Windows.
- Github Account:
  - Your account must be at least one month old.
  - You must have at least one public repository.
  - Your account must follow at least 5 GitHub accounts and have at least 1 follower
- Internet Connection: A stable and reliable internet connection is required. The most common cause of failure is a timeout due to slow or unstable uploads. 
- Recommended Hardware:
  - CPU: Intel Core i5 or better
  - RAM: 16GB or more
  - Storage: 100GB or more
  - Network: Fast internet connection

## Existing contributions

Container ID: `411d8vuzogogMxXJqTQcu61btgQ6rL2VNYUYnH7r4kE3`

|Participant|File Challenge                                                    |NeoFS Object ID                               |Cloud URL                                                        |
|-----------|------------------------------------------------------------------|----------------------------------------------|-----------------------------------------------------------------|
|NGD        |`071d2176b99861f97e57020cd5ef3904299fffb1fdb8bf0994d9bbf5e36f60ad`|`4t51oBmnwu3UHpC35HAS3aoF2jcMtjmpL9df7vZR447r`|https://zkstorage.blob.core.windows.net/zk-blob/Phase1_1_NGD     |
|NSPCC      |`3446c3cc02a91df93846621f7b9d3641ca2638a0c959e2b5e03bc37823f27625`|`4QNXbGzU3ooJgpsR7EVawyKgtrQSDDw5BwdLYeND9gZT`|https://zkstorage.blob.core.windows.net/zk-blob/Phase1_2_NSPCC   |
|AxLabs     |`4a7b705174f35e07672dbf3271cb2dfe2948b2861df4b7e98fece41fe8c3f21e`|`CpbUnRe4qnxQZQH1SrKqCuCXo8aBis4HsuKDeN2ghB6w`|https://zkstorage.blob.core.windows.net/zk-blob/Phase1_3_AxLabs  |
|Lazynode   |`2a9d15f8d5dbf0117b4cbb7fd43f41ccd1be3c9409e3d6f7da4964aa6447547c`|`8q5JMQ6x3ELp2XkLeqtGpGGHEiqgvRXL4a6AyHHvobi2`|https://zkstorage.blob.core.windows.net/zk-blob/Phase1_4_Lazynode|

## New contributions

Container ID: `2wDsJfm4bQvxTbywAzgd7RpA7Yf13xdY383FcykKwWN6`

|Participant|File Challenge                                                    |NeoFS Object ID                               |Cloud URL|Contributing Start Time|Contributing End Time|
|-----------|------------------------------------------------------------------|----------------------------------------------|---------|-----------------------|---------------------|
|           |                                                                  |                                              |         |                       |                     |
