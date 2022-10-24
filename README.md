# SSDLAB　Hyperledger-Aries  

現在稼働中のACA-Pyについて，Issuer,Holder,Verifierの３つ別々のVMでdocker-compose upしている．  
もし，何らかの理由でcomposeが消えてしまった際のバックアップとして最終環境構成を示す．  

## フォルダ構成と導入方法
1. VM（導入したい環境）にHyperledger-AriesのリポジトリをGitHubからクローンする．
2. 当リポジトリをクローンし，Ariesのdockerディレクトリに移動する．立てたいAgentフォルダを当リポから選んでフォルダごとコピーする．以下参考  
--ACA-py  
　--docker  
　　--立てたいAgentフォルダ  
3. envファイルに記述された{}の値を変更し，compose upする．
基本的にcomposeファイルを弄る必要はないが，webhookやaca-pyのコマンドを追加したい場合には変更可能である．
変更する際にはenvファイルも確認し,適切に変更することが求められる．

> https://tech.gmogshd.com/dev-env-4-indy-aries-with-docker/