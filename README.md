# デジタルアーツ東京　2016年度1年生用リポジトリ

# 10回目(7/1)
- 前回の作業
  - https://github.com/tanakaedu/dat161-haru/wiki/0624yoketoru-unity%E3%81%AE%E4%BD%9C%E6%A5%AD%E6%89%8B%E9%A0%86

## yoketoru/unity 開発
- キャラクターを管理する変数の作成
- キャラクターの表示


## 課題(予定)「オプション(或いは分身)を作ってみよう」
- マウスを動かすと、複数のラベルがマウスを追いかけるプログラムを作成する

1. 新しくプロジェクトを作成(プロジェクト名：option)
2. タイマーを設定
3. 必要な変数を定義
3. コンストラクタ内に、ラベルを４つ程度作成して表示(数を自由に調整できるようにするとよい)
4. タイマー処理内で、マウスの座標を取得
5. 取得したマウスの座標を配列に入れる
6. ラベルに座標を設定する

### 締切
- 提出方法は、ネットドライブ上に提出用フォルダーを作成しておくので、そこにプロジェクトをまるごとコピーする

### 考え方
マウスのX座標を入れる配列msx[]を用意したとすると、以下のようなことを考えてみよう。

- msx[0]に、現在のマウスX座標
- msx[1]に、前回のマウスX座標
- msx[2]に、前々回のマウスX座標
- msx[3]に、さらにその前のマウスX座標
- ：
以上のように、配列にマウスのX座標が記録されていくとしよう。msx[0]の座標にラベルを表示したら、X方向が現在のマウスの場所に一致します。もう一つのラベルをmsx[1]の位置に表示すれば、1フレーム前のマウスの座標にラベルが表示されます。msx[2]の位置にまた別のラベルを表示すれば、2フレーム前にマウスがあった場所にラベルが表示されます。これを繰り返したら、複数のラベルが、マウスが通った軌跡をなぞっていくようになります。

上記の例では、1フレームずつ前の場所を参照するので、ラベルはくっついて表示されます。これを10フレーム前にしたらどうなるでしょうか。タイマーを初期設定のまま使っていた場合は、1秒に10フレーム処理しますので、1秒前にマウスがあった場所にラベルが表示されるようになり、より面白い動きになります。

配列は無限に作ることはできません。上記の処理をずっと繰り返すには工夫が必要です。工夫の仕方を考えてみましょう。


# 12回目(7/15)
- 夏休みに向けて、企画を考える
- [染谷翔 Unityスキルがなくても使える短期間ゲーム開発のポイント](https://speakerdeck.com/unitydojo/gemuziyamuyazu-ye-zhi-zuo-dui-ce-unitysukiruganakutemoshi-eruduan-qi-jian-gemukai-fa-falsepointo)
- code.org

## 夏休みの宿題
- ミニゲームを１本完成させる
  - 公開可能であること
    - 全てのリソースが著作権的に問題がないこと
    - 公序良俗に反しない
    - 過度なエロ禁止
    - 基準は、就職活動の時に使えるもの
  - AssetStoreを活用するとよい
  - 著作権に問題がなければ、シナリオライターやその他プロジェクトを活用してもよい
- 夏休み明けにプレゼンテーションを行ってもらうので、パワーポイントなどの資料を作成しておく
  - 持ち時間は一人10分

----

# 9回目(6/24)
## yoketoru/unity 開発
- シーン管理


# 8回目(6/17)
## 前回のまとめ
- 沢山のラベルを跳ね返して、マウスで消すのを、wikiを使って全員で完成させる

## Ｃ＃
- GitHubで新規にプロジェクトを作成
- readme.mdに、習作ミニゲーム「yoketoru」の仕様をまとめる
- 開発開始
  - 作業予定をissueに作成する
    - issueを作る手順をwikiにまとめる
  - 作業を進める
  - 作業が進むごとにcommit
    - commitの仕方をwikiにまとめる
  - 完了した作業はチェックして終える
  - 講義の最後にSync


# 7回目(6/10)
## 前回の課題のチェック
- GitHub DesktopのSign in
- 変数の型の変換リスト

## Ｃ＃
- 前回の復習
  - 跳ね回るラベルを作る
  - マウスが重なるとタイマーが止まる
  - 経過フレーム数の表示
- 配列
- 繰り返し
- 沢山のラベルを跳ね返らせる


# 6回目(6/3)
- 前回の復習
- C#の講義
  - GitHub Desktopで、リポジトリを作成
  - マウス入力
  - 乱数
  - ifの発展
- Unity
  - 上記でやったことをUnityでやる

# 5回目(5/27)
- [日本科学未来館 企画展「GAME ON」特別イベント「ゲームってなんでプログラミング？」](http://www.miraikan.jst.go.jp/event/1604141719829.html)
  - 2016年5月29日（日）14:00～16:00（開場：13:30～）
- [LIG INC. Webサービス同士を連携できる「IFTTT」と自作IoTデバイスを繋いで生活を便利にしてみた](http://liginc.co.jp/263899)
- [Unity 5.4 パブリックベータ版](http://blogs.unity3d.com/jp/2016/03/15/enhanced-visuals-better-performance-and-more-the-unity-5-4-public-beta-is-ready/)
- C#の講義
  - if文

## 課題
- 次回までにp10の課題「違う型の変数への代入」を調べて、GitHubのWikiにまとめておく
  - 手順1 リポジトリを作成
    - Firefoxで、https://github.com を開いて、Sign inする
    - 右上の[+]を押して、[New Repository]を選択
    - Repository name欄に、 gp161-haru と入力
    - Description欄に、「ゲームプログラミング1年春用」と入力
    - [Initialize this repository with a README]にチェックを入れる
    - 上記以外はそのままで、[Create repository]ボタンを押す
  - 手順2 以上でリポジトリが作成される。続いて、wikiを作成
    - 画面上のメニューから[wiki]をクリック
    - [Create the first page]を押す
    - [Create new page]の下の[Home]を消して、「違う型の変数への代入」を入力
    - 下のテキストボックスの[Welcome to・・・」の行を削除して、課題の内容を記入する
    - 書き方は、github マークダウン]などで検索すると、さまざまな記述があるのでそれを利用してもよい
    - 書き終わったら、画面右下の[Save Page]ボタンを押して完成
以上。


# 4回目(5/20)
- 変数の学習-動的に動くプログラム-
- Unityで同じことをやってみる

# 3回目(5/13)
- [5/24 自作キャラのゲーム作成を無料体験【Unity/iClone/Maya】](https://kenjin.unity3d.jp/events/show/365)
- [日本科学未来館 GAME ON](http://www.fujitv.co.jp/events/gameon/)
- [塚本直樹 sorae.jp カナダの少年、「マヤ文明の古代都市」を星座の星の配置から大発見](http://sorae.jp/030201/2016_05_11_maya.html)


# 2回目(4/29)
- Visual C# 書く教科書
- [CAREER DESIGN CENTER まつもとゆきひろ氏が「生涯プログラマー」でやっていきたい若手に贈る3つの言葉](http://type.jp/et/feature/243?utm_content=buffer8884b&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer)
- [Pico Pico Cafe](http://www.picopicocafe.com/)
- 東京インディーズ
  - [HP](http://www.tokyoindies.com/)
  - [Facebook](https://www.facebook.com/events/264884527192215/)
  - [デジゲー博2016](http://digigame-expo.org/)
- [Unity県人会議イベント一覧](https://kenjin.unity3d.jp/events)
- [さいたまゲームス](https://atnd.org/events/77043)
- ドットインストールでUnityの練習


# 過去のページ
- [1回目(4/22)](https://github.com/tanakaedu/dat161-haru/blob/master/01/01.md)
