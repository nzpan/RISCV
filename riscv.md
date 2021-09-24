# RISC-Vとは
- "RISC-V is a free and open Instruction Set Architecture"

[RISC-V International](https://riscv.org/)

# 採用が増加
- RISC-V Open era of computing [[pptx]](https://riscv.org/wp-content/uploads/2021/05/RISC-V-New-Era-04-19-2021.pptx)

- 「20年以内に、おそらくARMは約1兆個のチップを地球上にばらまくことになる」(2016/7/21 SBG孫正義) [記事](https://logmi.jp/business/articles/153432)
このときから5年経ってRISC-VがARMの競合になりつつある

- NVIDIA、Armを400億⽶ドルで買収 [記事](https://www.nvidia.com/ja-jp/about-nvidia/press-releases/2020/nvidia-to-acquire-arm-for-40-billion-creating-worlds-premier-computing-company-for-the-age-of-ai/)
[記事](https://news.yahoo.co.jp/byline/shibatanaoki/20201006-00201672/)

- ルネサスでも採用
ルネサスとSiFive、車載用次世代ハイエンドRISC-Vソリューションの共同開発で提携[記事](
https://www.renesas.com/us/ja/about/press-room/renesas-and-sifive-partner-jointly-develop-next-generation-high-end-risc-v-solutions-automotive)
- ルネサス初のRISC-V搭載ASSPの開発に向けて、アンデス社のRISC-V 32ビットCPUコアを採用[記事](https://www.renesas.com/us/ja/about/press-room/renesas-selects-andes-risc-v-32-bit-cpu-cores-its-first-risc-v-implementation-assps)

# 趣味の世界でも身近に
RISC-V 32 bitコアを搭載したGD32VF103CBT6 MCUベースの開発ボード[switch science](https://www.switch-science.com/catalog/5946/)

雑誌では
Interface(インターフェース) 2019年 12 月号[cq](https://interface.cqpub.co.jp/magazine/201912/)
トランジスタ技術 2019年 [11 月号](https://toragi.cqpub.co.jp/tabid/888/Default.aspx) 、[12月号](https://toragi.cqpub.co.jp/tabid/887/Default.aspx)

# なぜISA(Instruction Set Architecture)が重要なのか？
## ハードウェアとソフトウェアのつなぎ目

- ハードウェア: チップ、デジタル回路
- ソフトウェア: コンパイラ、デバッガ

ハードウェアだけではシステムは作れない。

思ったとおりに動かなかったらデバッガで解析する必要がある。

## ISA比較
ARM, RX, RH850, x86, x86-64

- RISC-V: 32bit固定長命令
[RISC-V specification](https://riscv.org/technical/specifications/)

- RX:     可変長命令
[RX RXv3命令セットアーキテクチャ](https://www.renesas.com/in/ja/search?keywords=RXv3%E5%91%BD%E4%BB%A4%E3%82%BB%E3%83%83%E3%83%88%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3)


# RISC-V企業
- Andes Tech
台湾のcpu core IPベンダ
verilogを提供[link](https://github.com/riscv/riscv-cores-list)

- SiFive
chiselで開発

IntelがSiFiveに20億ドルで買収提案か[記事](https://eetimes.itmedia.co.jp/ee/articles/2106/15/news056.html)

## chisel
Scalaという言語でつくられたハードウェア記述言語。

University of California, Berkeleyで開発。
解説書:
[Digital Design with Chisel](https://github.com/schoeberl/chisel-book)
[pdf](http://www.imm.dtu.dk/~masca/chisel-book.pdf)

instance生成機能が充実。

verilogのgenerate文でやるようなことをScalaの機能を使ってできる。

verilogではgenerate文の記述力が貧弱なのでperlやpythonなどを使ってRTL生成することがある。

さらに高度な機能

ハードウェア記述言語Chiselをもっともっと活用するためのDiplomacy概説[youtube](https://www.youtube.com/watch?v=92rULS6OfjA&t=15s)

## 勉強会
risc-v.connpass.com[link](https://risc-v.connpass.com/event/)

RISC-VとChiselで学ぶ はじめてのCPU自作[link](https://gihyo.jp/book/2021/978-4-297-12305-5)
株式会社フィックスターズRISC-V研究所 ⻄⼭悠太朗, 井⽥健太

勉強会[link](https://www.youtube.com/watch?v=RPytP3YiqdY)


