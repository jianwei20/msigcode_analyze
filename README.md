# Msigcode_analyze
  Misg-bft is fork from go ethereum,the system architecture follows NCCU-BFT and Hydrachain.<br>
  
 1.(Consensus Manager):The Consensus Manager is used to manager the height manager,The consensus manager also interacts with Miner Modul,to receive non-vaildated block and return vaildated block. Whenever the nodes receives a message with heigher block than current block,the consensus manager of two node call the synchronizer to request the block between two heights.
 
 2.(Height Manager):The Height Manager is used to process th data communication between Consensus Manager and Round Manager.The height manager sends the message from consensus manager to round manager.The height manager collects the data from round manager and send it to the consensus manager to be broadcasted or signed.
 
 3.(Round Manager):The Round Manager is used to process the consensus of given round at given height.........

<img src="/picture/01.png" width = "500" height = "400" />


## Contents

 - [0.Introduction](/zh/0.Introduction.md) (簡介)<br>
     [0.1 Consensus Algorithm Introduction](/zh/0.1Consensus_Algorithm_Introduction.md)(演算法簡介)<br>
 - [1.Download and Execution](/zh/1.Dowload_and_Execution.md) (程式下載及安裝執行)
 - [2.Miner Code Analyze](/zh/2.Miner_Code_Analyze.md)(共識演算法程式碼分析)<br>
     [2.1 miner/agent.go](/zh/2.1miner_agent.md)<br>
     [2.2 miner/miner.go](/zh/2.1miner_miner.md)<br>
     [2.3 miner/worker.go](/zh/2.1miner_worker.md)<br>
 - [3.Consesus Code Analyze](/zh/3.Consesus_Code_Analyze.md)(共識演算法程式碼分析)<br> 
     [3.1 consensus/bft/bft.go](/zh/3.1consensus_bft_bft.md)<br>
     [3.2 consensus/bft/bft_manager.go](/zh/3.2consensus_bft_bft_manager.md)<br>
     [3.3 consensus/bft/bft_peer.go](/zh/3.3consensus_bft_bft_peer.md)<br>
     [3.4 consensus/bft/bft_handler.go](/zh/3.4consensus_bft_bft_handler.md)<br> 
     [3.5consensus/bft/bft_protocol.go](/zh/3.5consensus_bft_bft_protocol.md)<br>
     
 - [4.Experiment results]()(實驗結果分享)
 - [5.](https://github.com/polaris1119)(review书)
 - [6.](https://github.com/qyuhen)(review第二章)






# Referece

- Go Ethereum [github](https://github.com/ethereum/go-ethereum) 

- Hydrachain [github](https://github.com/HydraChain/hydrachain)

- PBFT [paper](https://www.usenix.org/legacy/publications/library/proceedings/osdi99/full_papers/castro/castro.ps)

- Tendermint [paper](https://cdn.relayto.com/media/files/LPgoWO18TCeMIggJVakt_tendermint.pdf),
   [github page](https://github.com/tendermint/tendermint)


# Multiple Language Versions


## Contributors

- See [contributors page](contributors.md) for full list of contributors.

## Community

E-mail：jinwei's email(sujianwei20@gmail.com)
