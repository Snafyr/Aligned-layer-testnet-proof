ALIGNEDLAYER PUBLIC PROOF TASK


Getting Started
```
sudo apt update -y
sudo apt upgrade -y
sudo apt-get install curl -y
```

Download Aligned Proof Files
```
curl -L https://raw.githubusercontent.com/yetanotherco/aligned_layer/main/batcher/aligned/install_aligned.sh | bash
source /root/.bashrc
curl -L https://raw.githubusercontent.com/yetanotherco/aligned_layer/main/batcher/aligned/get_proof_test_files.sh | bash
```

Send Proof
```
rm -rf ~/aligned_verification_data/ &&
aligned submit \
--proving_system SP1 \
--proof ~/.aligned/test_files/sp1_fibonacci.proof \
--vm_program ~/.aligned/test_files/sp1_fibonacci-elf \
--aligned_verification_data_path ~/aligned_verification_data \
--conn wss://batcher.alignedlayer.com
```

Take the screenshot of the result in your cmd and explorer then send it on twitter.

![image](https://github.com/Snafyr/Aligned-layer-testnet-proof/assets/83130343/0414f859-9551-46ba-b9a5-ec90b31f561d)

Send the link of the tweet in their discord.
