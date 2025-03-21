# パブリックテストネット
物理的なネットワークを構築せずに実験を始めたい場合は、パブリックレティキュラムテストネットに参加してください。テストネットはまさにそれであり、テストと実験のための非公式なネットワークです。ほとんどの時間稼働しており、誰でも参加できますが、それは同時にサービスの可用性に対する保証がないことも意味します。

テストネットは最新のレティキュラムのバージョンを実行しており（公開される前の短い期間でもあることがよくあります）、時折実験的なレティキュラムのバージョンがテストネット上のノードに展開されることがあり、それにより奇妙な動作が発生する可能性があります。それでも怖くない場合は、TCPまたはI2Pを使用してテストネットに参加できます。

次のいずれかのインターフェースをReticulumの設定ファイルに追加してください：

```
# Dublin HubへのTCP/IPインターフェース
  [[RNS Testnet Dublin]]
    type = TCPClientInterface
    enabled = yes
    target_host = dublin.connect.reticulum.network
    target_port = 4965

# BetweenTheBorders HubへのTCP/IPインターフェース（コミュニティ提供）
  [[RNS Testnet BetweenTheBorders]]
    type = TCPClientInterface
    enabled = yes
    target_host = reticulum.betweentheborders.com
    target_port = 4242

# I2P Hub Aへのインターフェース
  [[RNS Testnet I2P Hub A]]
    type = I2PInterface
    enabled = yes
    peers = g3br23bvx3lq5uddcsjii74xgmn6y5q325ovrkq2zw2wbzbqgbuq.b32.i2p
```

テストネットには[Nomad Network](https://github.com/markqvist/nomadnet)ノードおよび[LXMF](https://github.com/markqvist/lxmf)伝播ノードも含まれています。

# コミュニティ エントリポイント
コミュニティによって、Reticulum ネットワークへの公開エントリポイントが多数提供されています。日常的な使用には、テストネットではなくこれらを使用することをお勧めします。

デバイスまたはインスタンスをこれらの 1 つ以上のエントリポイントに接続して、物理的に接続されている Reticulum ネットワークにアクセスできます。

理想的には、自分のデバイスがローカルでアクセスできる Reticulum トランスポート ノードを設定し、そのトランスポート ノードをいくつかのパブリック エントリポイントに接続します。これにより、いずれかのエントリポイントがダウンした場合でも、効率的な接続と冗長性が提供されます。

{PUBLIC_ENTRYPOINTS}

<p align="right"><a href="docs_jp.html">次のトピック：マニュアルを読む</a></p>