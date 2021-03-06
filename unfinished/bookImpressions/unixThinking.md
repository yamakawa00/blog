UNIXという考え方 感想

書籍感想

# なぜ読んだか

重い技術書の休憩に読める軽く読める技術書が読みたくなったためです。

# 引用&感想

## UNIXの考え方:簡単なまとめ

```
1.スモール・イズ・ビューティフル
小さいものは、大きいものにはない利点がいくつもある。小さいものどうなら、簡単に独特の便利な方法で組み合わせることができるというのもその一つだ。

2.一つのプログラムには一つのことをうまくやらせる
3.できるだけ早く試作する
4.効率より移植性を優先する
5.数値データはASCIIフラットファイルに保存する
6.ソフトウェアを梃子(てこ)として使う
7.シェルスクリプトによって梃子の効果と移植性を高める
8.過度の対話的インターフェースを避ける
9.全てのプログラムをフィルタとして設計する
```

## 小さなプログラムは保守しやすい

```
小さなプログラムは、分かりやすい。分かりやすいと保守も容易になる。
(略)
ほとんどのソフトウェア技術者は、他人のフログラムの保守で生活することには満足しない。以前のプログラムの修正よりも、新しいプログラムを書くことの方が良い仕事だと考えている。おそらく、その考えは正しいだろう。だが、不幸なことに、ユーザーは同じようには見てはくれない。ユーザーは、最初からプログラムがきちんと動くと思っている。うまく保守できない会社は長く生き残ることはできない。
(略)
よって、プログラマは、保守作業を好まないにしろ、それに耐えられる程度にはプログラムをきちんと書いておく必要がある。そこで小さなプログラムの出番だ
```

保守が嫌いな気持ちは、よく理解できます。だが、保守はビジネスにおいて継続的な利益を生みだすためには必須です。

嫌いだけど、やらなきゃいけない時はどうするか。そこにかかるストレス、負荷を必要最低限にすることが解決策だと思います。

保守しやすいプログラマにするには、設計時点である程度は決まるので、設計スキルを上げることが保守の負荷を下げる一つの手段ですね。

## 一つのプログラムには一つのことをうまくやらせる

```
一つのことをうまくやるようにアプリケーションを書けば、それは必然的に小さなプログラムになる。
(略)
小さなプログラムは単一機能になる傾向があり、単一機能のプログラムは小さくなる傾向がある。
さらに、この小さなアプローチによる隠れたメリットがある。現在の仕事に集中することによって、やろうとしていることの本質が掴めるのだ。一つのことをうまくやるようにプログラムを作れないのであれば、おそらく問題を完全に理解していないのだろう。
```

## できるだけ早く試作を作成する

```
ほとんどの人は「アプリケーション設計を完全にしてからコーディングにかかれ」と教えられている。「まず、機能仕様書を書かなくちゃ」と言う。背的的なミーティングで方向性を確認する。細部まではっきりさせた考えを設計仕様書に書く。90パーセントの設計ができて始めてコンパイラを使う。
原理的には、もっともな指針に聞こえる。しかしこの考え方は、試作というものの重要性を見過ごしている。あるアイデアがものになりそうかどうか、目に見える現実的な場面でテストするには試作が一番だ。試作以前のアイデアは、これはこう動くはずだという憶測の域を出ない。この時点では、設計構想はほとんど理解されておらず、おそらく人によって解釈が異なっているのだろう。プロジェクトの前進には、全員の合意が必要だ。試作は、具体的に目標を示すことで全員の合意を醸成する。
```

ここでは試作品(プロトタイプ)の重要性を説いています。

実際に手を動かして作る目的は、プロジェクトメンバー全員に対して意識を共有するということです。

## 試作によって学ぶ

```
試作が早ければ早いほど、製品のリリースは早まる。試作によって何がうまくいくかが分かり、さらに重要なことに何がうまくいかないかが分かる。一つの方法を選んだ以上、その方針の適否を早めに判断しなければならない。前提の謝りを早期に発見し、わずかな被害で済ませるのと、誤った前提のまま何ヶ月も開発を進めて、リリース日の3週間前に不意打ちを食らうのと、どちらが良いかいうまでもない。
```

試作品は、プロダクトのメリットデメリットが凝縮されているので、後の問題点が浮き彫りになります。

さらには、0->1のフェーズを自分で経験できるので、そのフェーズが得意になります。

## スピード不足は次の年のマシンで克服される

```
現在のアプリケーションがかろうじて問題ない性能で動作しているのであれば、明日にはスピードは十分なものになっているだろう。2、3年後には、少しスピードを落とさないと人間の手には負えなくなるかもしれない。
```

研究室の教授が言っていたのですが、既存の方法に比べて有用だが、マシンのスペックが追いついていないため非現実的であるという研究手法は、時間が解決するので先行投資すべきだとおっしゃていたのが記憶に残っています。

## 好みに応じて自分で環境を調整できるようにする

```
(UNIXは)一定のレベルに達すると、もう、他のオペレーテイングシステムに戻ることは難しい。UNIXにかけた時間がある一点を超えてしまうと、そのまま放り出してしまうよりは、気に入らない部分を変更しながら使い続けるようになるのだ
```

## 90パーセントの解を目指す

```
90パーセントの解とは、難しい部分を故意に無視することを意味している。
難しい部分とは、問題で高くつく部分、時間のかかる部分、実装しにくい部分だ。一番難しい10パーセントを無視して良いのであれば、世界中のほとんどの問題はすぐにでも解決する。
(略)
90パーセントの解なら、目安としてはまずまずのところだろう。それを認め、ユーザーの大部分にアピールするアプリケーションをかけばいいと心得ると万事がやりやすくなる。
これがUNIXの成功の一員だ。
(略)
90パーセントのニーズを満たすことに徹しているのだ。
```

## UNIXの考え方:統括

```
小さなプログラムは、目的を絞らなければならない。言い換えると、一つのことをうまくこなすことに専念すべきだ
```

```
試作をできるだけ早いうちに作ることが重要だ。設計者の頭の中にあったアプリケーションが、早期に形となって他人の手に渡り、それだけ第三システムへのあゆみも早まる。施策は、将来へ向かっての歩みを加速させる。
```

```
覚えて欲しい。ソフトウェアは、実は作るものでなく、成長していくものなのだ。成長したソフトウェアを新しいハードウェアにも移植できれば、そのソフトウェアの価値は上がる。
```

# まとめ
