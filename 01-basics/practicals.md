## 最佳实践

正所谓“纸上得来终觉浅，绝知此事要躬行”。本章将介绍一些常用的工具软件或网站以便快速入门区块链。

### 节点

作为区块链的核心，运行一个节点会让你对区块链了解的更深入，当然，也会更偏技术，这也就意味着难度会
稍为增加。但对于 Bitcoin 来说，运行一个全节点或者说是轻节点技术上已经很成熟，和普通的在电脑上安装
运行一个软件没啥区别。

> Note: 正常来说，只推荐运行 Bitcoin 的节点，其他的节点成本太贵，不适合普通人。

因为节点本质其实也是个软件，而软件开发又有不同的编程语言，所以节点的软件也会有多种，对于 Bitcoin
来说，官方的是 Bitcoin-Core，最下版本的下载地址为: https://bitcoin.org/en/bitcoin-core。
如果需要下载指定版本，可以在 [BitcoinCore.org][bc-org] 选择对应的版本下载安装。

[bc-org]: https://bitcoincore.org/en/releases

Bitcoin 节点的使用比较广泛的还有：[Bitcoin Knots][bitcoin-knots] 和 [bcoin][bcoin]。
其他节点的数据参见 [Coin Dance][coin-dance-nodes]。

[bitcoin-knots]: https://bitcoinknots.org
[bcoin]: https://github.com/btcsuite/btcd
[coin-dance-nodes]: https://coin.dance/nodes

> Notes: Bitcoin Core 其实是个节点和钱包都在一起的，它即时节点，也是钱包，毕竟钱包操作是需要
> 连接节点进行操作的。Bitcoin Knots 是 Bitcoin Core 的改造版本，将一些比较新的特性加到了上
> 面，界面和 Bitcoin Core 没有差别。

运行节点很简单：下载 -> 安装 -> 执行/运行。只要有足够的硬盘，网速不是很差，其实就可以正常运行。
如果需要多节点进行定制化的配置，可以使用在线的[**配置生成器**][bc-conf-gen]生成配置后复制粘贴到本地的配置文件中，保存
后重启软件就行。

[bc-conf-gen]: https://jlopp.github.io/bitcoin-core-config-generator

### 钱包

#### All-in-one

如果是为了图省事方便，那么基本上知名的交易所都有自己的 Web3 钱包，因为交易所本身就需要运行各个链
的节点来检查充值体现，所以基本上只要交易所支持充值的币种，其 Web3 钱包也都会支持对应的链。

但是有一点需要注意的是，交易所因为人员流动性大，也比较复杂，所以安全上会略微比一些主流开源的钱包
要差一些，小资金玩一玩可以，毕竟方便，但是大资金只能说 **DYOR (Do Your Own Reasearch)**。

大交易所中最先开始做 Web3 钱包的是 OKX 交易所，其 Web3 钱包的用户和使用体验也比较好，其次是
Binance 了，毕竟是第一大交易所，维权什么的会好一点。

> Tips: 虽然说不太希望又人去维权，但是总是会有意外发生，据身边朋友总结的经验来看，一般来说除了
> 找客服外，最管用的是直接在推特上去 @ 他们的老板，比如说 OKX 的老板 [star-okx][star-okx]，
> 以及 Binance 的 [cz][cz] 和 [heyi][heyi]。尤其是在客服不响应的情况下直接去推特上找老板
> 效果会更好。

[star-okx]: https://x.com/star_okx
[cz]: https://x.com/cz_binance
[heyi]: https://x.com/heyibinance

#### Bitcoin

- [Bitcoin Core][bc-org]

  对于比特币来说，如果你只是个囤币用户，那么你可能只需要 [Bitcoin Core][bc-org] 就够了，
  不过 Bitcoin Core 钱包的导入导出比较麻烦，同时也不能直接支持助记词导出，你只能导出对应的
  私钥（助记词对应的也是份私钥）,或者直接备份 wallets 文件夹。优点是会比助记词稍为安全一点，
  缺点是多设备导入导出麻烦，同时也只支持电脑端，要想导入到其他的设备需要学习对应的 Bitcoin Core
  的命令才能导出对应的私钥。

- [Sparrow][sparrow]

  如果你是个技术，或者想要深入学习，那么 **[Sparrow][sparrow]**，这个对比特币的 **TX(Transaction)**
  的展示非常清晰，有助于理解学习比特币 TX 的 **UTXO (Unspent Transaction Output)**。当然
  这个对于初学者会有一点上手难度，还有一点就是 Sparrow 也只支持电脑端，不支持移动端和浏览器插件。

  [sparrow]: https://sparrowwallet.com

- [Unisat][unisat]

  进几年出现的浏览器插件钱包，国人团队制作，主要是**铭文(Inscription)**的产物，在这之前比特币
  没有浏览器插件钱包，都是独立的 app，因为比特币只需要进行转账，不需要和
  **DAPP (Decentralized Application)** 进行交互，而铭文需要在一些平台进行代打，所以浏览器
  插件钱包也就应时而生，OKX Web3 钱包也是这个时候最先开始推出并且抢占了大部分市场。浏览器插件的
  有点就是方便，不需要下载安装其他的软件，只需要浏览器就行。缺点是会有钓鱼网站，容易被钓鱼，毕竟
  在单独的 app 里是没办法去连其他的网站的。当然 Unisat 也有移动端，但是随着铭文时代的落幕，这个
  可能也成了过去。估计现在已经没有什么活跃用户了，毕竟 OKX Web3 的钱包体验不比它差，而且还支持
  多链。

  [unisat]: https://unisat.io/download

- [BlueWallet][bluewallet]

  在这个人手都有一部手机的情况下，大部分人还是希望有时能在手机上操作的，毕竟手机小巧方便，可以随时
  随地操作。移动端来说，**[BlueWallet][bluewallet]** 的体验很好。首先，这款钱包 app 支持
  **Airgap**，也就是能够直接通过扫码进行签名，也就意味着可以不用联网，就能完成签名操作，这点在
  安全方面基本算是顶级的了。同时这款钱包还支持创建**多签钱包**，如果是大资金的话其实也会更加
  “去中心化安全”，毕竟多签钱包能保证不依赖于单个助记词，如果单个助记词的话，弄丢了就再也找不回来
  了，而多签钱包的话对于丢失部分助记词的话依然可以进行转账，容错性更大。

  > 多签钱包：即需要多个私钥都签名后才能进行转账，就好比一扇门有多个钥匙孔，但是需要多个钥匙一起
  > 才能开门，但是不需要所有的钥匙，只需要满足一定数量的钥匙就能将门打开。一般来说比较通用的的
  > 多签选项有 2-of-3, 3-of-5 和 5-of-7。这些选项的格式是第一个数字是至少需要私钥的数量，
  > 第二个数字是总共的私钥数量。当然，你可以自己定义这些选项，4-of-5, 3-of-7 等都是可以的，
  > 就看你自己允许的容错程度，你当然也可以设置为 3-of-3，但是这和只有一个私钥也没差，唯一的区别
  > 就是这个在资金管理时可以控制资金的安全，必须所有人都同意才能进行转账。

  [bluewallet]: https://bluewallet.io

当然，比特币官网也有对应的工具从多个角度对比钱包，你可以根据自己的需求的钱包，具体参考：https://bitcoin.org/en/choose-your-wallet

#### EVM-ecosystem

对于 EVM 生态来说，钱包数不胜数，这里只推荐一些作者用过的钱包，没用过的不推荐介绍。毕竟“没有调查，
就没有发言权”。

- [Metamask][metamask]

  以太坊最早的钱包，但是这些年没什么作为，尤其是在 **DeFi (Decentralized Finance)** 发展
  的时期，基本没什么改进，唯一值得一提的是他们的钱包安全性比较高，这个安全性是指软件方面，他们
  独有一个沙盒模式，能比较好的防止病毒软件入侵。但是在签名方面做的有点拉垮，都不展示对应的 TX
  中的详细信息。不过最近也支持 Solana 和 SUI 的地址，但是具体来说体验还是不太好，不过怎么说，
  对于 DAPP 的支持是最广泛的，基本上所有的 DAPP 都会支持 metamask。

- [Rabby][rabby]

  专注于以太坊生态以及 DeFi，比较突出的特点是其安全性，即对于一些不知名的网站需要进行签名的话，
  会有警告，同时需要二次确认才能完成签名，这个能很好的规避掉一些钓鱼网站，同时对于个 TX 的数据
  都会解析出来，很清楚明白，对 DeFi 玩家很友好。

- [Uniswap][uniswap]

  DeFi 领头项目方做的一款钱包，体验也不错，专注于 Swap，很丝滑。

[metamask]: https://metamask.io
[rabby]: https://rabby.io
[uniswap]: https://wallet.uniswap.org


#### Solana

- [Solflare][solflare]

  Solana 官方团队出品，支持者 solana 生态，这个是唯一一个亮点，其他的自行探索吧，个人不太喜欢
  solana 这条链，只是偶尔玩一玩 MEME。

- [Phantom][phantom]

  社区开发的钱包，一开始只支持 Solana，后来 Solana 生态起来后也慢慢支持一些主流的公链了，用户
  数量比较多，目前支持的公链有: Ethereum, Base, Sui, Polygon, Bitcoin。大部分 Solana 的
  MEME 玩家都喜欢用这款钱包。

  > 貌似目前接触的产品工具插件来说，好像都是社区做的要比官方做的好，而且用户也比官方的多。

[solflare]: https://www.solflare.com
[phantom]: https://phantom.com

总的来说，如果资金量不是很大的话，同时也不想折腾，那么推荐使用 [OKX Web3][okx-web3] 钱包，
但是安全性自己考虑清楚，看个人的风险偏好了。反正个人是不怎么使用这个钱包，里面的资金不会超过 $300，主要是有时候有一些其他的链需要单独的钱包，懒得再去下个插件然后再创建一个新的钱包，过于折腾。如果是 **DeFi** 玩家，Rabby 钱包是不二之选。如果是比特币玩家的话，个人是推荐 Bluewallet 以及 Sparrow。Solana MEME 玩家的话，那么要么 Solfare 要么 Fantom，但首选是 Fantom。其他链的话，
自行到对应的官网下载对应的钱包吧，唯一需要注意的不要点错网站，下到假的钱包。

[okx-web3]: https://web3.okx.com

### 浏览器

对于区块链来说，每笔交易/转账都需要确认，同时如果想要查看某笔特定的转账时需要怎么办呢？这个时候
就需要学会使用**区块链浏览器**了。

> 注：这里的浏览器与常见的浏览器不是一回事，或者说常见的浏览器全名应该叫做网络浏览器，是为了浏览
> 网页的软件，而区块链浏览器是查看对应的交易的 Web 服务。所以区块链浏览器是个 Web 服务，而不是
> 个软件。

与网络浏览器类似，区块链浏览器能够通过 TX ID/Hash 或者 对应的地址来查看这笔交易的详情或者这个
地址的详细信息。

#### Bitcoin

作为区块链的核心支柱，也是发展最久的，比特币的浏览器有很多，比较常用·的是以下几个：

- mempool: https://mempool.space
- blockstream: https://blockstream.info
- blockchain: https://www.blockchain.com/explorer/assets/btc
- bitaps: https://bitaps.com

其中 mempool 的体验最佳，同时也是多数人的首选。

#### EVM-ecosystem

EVM 生态的链太多，每个链都有自己单独的一个浏览器，不过基本都是和以太坊的类似，而以太坊的浏览器
其实就两个：

- etherscan: https://etherscan.io
- blockscout: https://www.blockscout.com

etherscan 是最老牌的，blockscout 是后续新起的，blockscout 相比于 etherscan 是它支持多链
查询，其他的基本没什么差别，主要就是 UI 界面的不同，etherscan 比较复古一点，blockscout 比较
现代一点。至于各个 EVM 生态的链的浏览器，直接搜索查询 "<链名> scan" 就会得到对应的浏览器地址。

#### Solana

Solana 主要的浏览器就以下三个：

- solscan: https://solscan.io
- solana explorer: https://explorer.solana.com
- SolanaFM: https://solana.fm

其中 solscan 是 etherscan 团队做的，延续了 etherscan 的风格，用户体验式会比其他两个更好。
官方的 solana explorer 对开发者比较友好一点，有开发者友好的 TX 解析。

对于浏览器来说基本都是大同小异，一般是查看一笔交易在**什么时候**从**哪个地址**转了**多少** **币**
到**另外一个地址**。可以自己都体验一下，然后选择一个自己喜欢的就好。
