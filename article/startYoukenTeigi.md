はじめよう！ 要件定義 ～ビギナーからベテランまで 感想

書籍感想

[はじめよう！ 要件定義 ～ビギナーからベテランまで](https://www.amazon.co.jp/%E3%81%AF%E3%81%98%E3%82%81%E3%82%88%E3%81%86-%E8%A6%81%E4%BB%B6%E5%AE%9A%E7%BE%A9-%E3%83%93%E3%82%AE%E3%83%8A%E3%83%BC%E3%81%8B%E3%82%89%E3%83%99%E3%83%86%E3%83%A9%E3%83%B3%E3%81%BE%E3%81%A7-%E7%BE%BD%E7%94%9F%E7%AB%A0%E6%B4%8B-ebook/dp/B00WHUP7UE/ref=tmm_kin_swatch_0?_encoding=UTF8&qid=&sr=)

# なぜこの本を読んだか

転職試験で、「小売のアーキテクチャーの構成を背景を含めて400文字で述べなさい。(要約)」という課題が出ました。

提出には時間をかけてよかったので、この本買って、要件定義の観点を洗い出そうとしました。

# 感想

## 要件定義とは何か、定義を決める

> 実は、要件を日常的な単語に置き換えると「注文（オーダー）」が妥当なものになります。では「注文」とは何でしょうか。それは 作ってほしい人が 作る人に出す 依頼事項（リクエスト） ということになります。

--------------------------------------------------------------------------------

> 依頼した人ができあがったものに対して「これならOKです」と言うために、「何がどうなればよいのか」ということを明確に定めたもの それが仕様書です。

ここで言えるのは、「依頼人」が「求めているものを文章化したもの」が仕様書です。

そんなの当たり前じゃんと思うかもしれないですが、こういう基本的なことを言語化しとかないと後で矛盾が生じる可能性が上がるので、あらかじめ定義しておくのが重要です。

--------------------------------------------------------------------------------

## 要件定義の完成形は何か(成果物は何か)

> UIとはUser Interface（ユーザインターフェース）の略です。インターフェースは接面と訳されることもあります。つまり「ユーザに接するもの」ということになります。 UIの代表例は何と言っても画面（スクリーン）です。そしてもう1つは帳票（プリンタからの印刷物）です。

--------------------------------------------------------------------------------

> 機能とは「ソフトウェアにやらせる仕事」の総称だと考えてください。 たとえば「消費税を計算する」などが機能になります。処理という表現を使うケースもあります。本書でも今後、機能といったり処理といったりすることがありますが、基本的には同じ意味だと理解してもらってかまいません。

--------------------------------------------------------------------------------

> そして3つ目が「データ」です。先ほどの「消費税を計算する」という機能の場合、計算結果の「消費税」はデータです。また計算のもととなる「売上金額」もデータです

--------------------------------------------------------------------------------

> この3つの要素、つまり「UI」「機能」「データ」が明確に定まって、そこで初めてプログラマはソフトウェアを作ることができるようになります。

要件定義の完了とは

- UI
- 機能
- データ

の定義の完了を意味します。

UIの定義は、「スクリーン」か「帳票」か

機能の定義は、どんな「処理」か

データは、どんな「情報」か

この3つを押さえていれば、完璧です。

--------------------------------------------------------------------------------

> データベースとは何か プログラミング的な観点で言えば、データベースはワークセットを越えて、さらにはシステムをすら越えて共有する、超グローバル変数です。

さらにデータベースについても記述があり、上記のように定義されています。

データベースはプログラミング言語としてのスーパークローバルとしての性格を持ち合わせています。

--------------------------------------------------------------------------------

## 完成形を実現するためのプロセスとは

> まずは「ソフトウェアを作る」という取り組みのゴールを確認しましょう。仕事でソフトウェア開発を依頼する・作るからには、当然思いつきだけではない何らかの企画意図が明確に定義されているはずです。そうでなければ予算などが決定しないからです。 そしてこれから作るソフトウェアはその企画意図を達成できるものでなければなりません。つまり企画意図から外れた要件を定義してしまったら、いくらそれをきちんと作ったとしても納得が得られません。

まず目標設定です。

最初に述べたように顧客の求めるものを明確に言語化する必要があります。

--------------------------------------------------------------------------------

> ITの本質はプロセスイノベーションであり、つまりは「中抜きの実現」です。余分な中間コストを排除してエンドツーエンドを実現するフォースこそがITの真骨頂です。

--------------------------------------------------------------------------------

> 本書の肝をひと言で言うなら「画面遷移図を描こう」になります。ここでいう画面遷移図とは、本書で紹介した画面と画面の間にイベントと機能を図示するものです。つまり要件定義とはこの画面遷移図を描くことができればほぼOKであり、それ以外は実は要件定義そのものではなく、その前後の工程で行うべき作業だということです。

最後にこの本が、上記のようにまとめられています。

「画面遷移図」とは、UIと機能説明を含めていると考えれらます。

--------------------------------------------------------------------------------

# 最後に

役立った箇所のみ抜粋しました。

転職試験では、目的を明らかにしてから、アーキテクチャの構成を書けたので、満足のいく論述ができたと思います。

その後、論述試験の合格がきました。
