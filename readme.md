# Windows インストールマニュアル
## 0. 作業の流れと解説

<font color="Pink">※ まだ電源を入れないでください。</font>
この作業は

1. BIOS の設定
2. Windows インストール
3. TAアカウントの作成
4. 受講者アカウントの作成と管理者権限の付与

の4段階に分かれます。

## 1. BIOS の設定
<font color="Pink">※ 電源はまだです！</font>

コンピューターの電源を入れるとまずは OS（operating system）などの基本的なソフトウェアをメモリに展開し、各種アプリケーションが使える状態にしなければなりません。通常それは BIOS （バイアス、Basic Input/Output System）により自動的に行われますが、今回は USB メモリからそれを行いたいので、BIOS の設定を変えて起動します。以下そのやり方を記述します。

### USB メモリをいれる
TA の配布する USB メモリに Windows が入っているので、それを USB ポートに挿してください。差込口が青いものと白いものが両方あるので、青い方に挿し込むと良いと思います。

### BIOS の設定画面を出す
コンピューターの電源を入れてから windows が起動するまでに特定のキーを押すと何かが起こります。どのキーを押すと何が起こるのかはコンピューターに寄ってい異なります。通常は説明書書いてあったり、起動画面の端に小さく書いてあったりします。本講義で使うPCの場合は、いずれも Delete で BIOS 設定画面です。

<font color="Pink">※ お待ちかね。スイッチオンです！</font>

コンピューターの電源を入れて、すぐに Delete キーを連打しましょう。タイミングが割とシビアなのでちゃんと連打しましょう。すると見慣れない画面に遷移するはずです。それが BIOS の設定画面です。なお Windows のログイン画面が出たら連打ゲー失敗なので、一度シャットダウンしてやり直してください。

![BIOS 設定画面](img/img1.JPG)

### BIOS の設定をする
表示言語はおそらく英語か日本語になっていると思います。どちらでも問題ないのですが、変えるには左上の「English」とか書いてある部分をクリックしてプルダウンメニューで選べば大丈夫です。ここで触るのは次の3つです。
- Boot priority
- OS Type
- Secure boot key

#### Boot priority
今からディスクの起動優先度を指定します。初めの画面の右下の方に、Boot priorityと書かれたところがあると思いますが、そのうち「UEFI:SanDisk Extreme」をマウスドラックで一番上にします。

#### OS Type
windows は boot するときに、UEFI（Unified Extensible Firmware Interface）を用いることを義務付けているので、従います。まずは BIOS 設定画面を Advanced mode にしましょう。そのためには、画面右下の「Advanced」とある部分をクリックするか、F7を推せばよいです。そのあと、「起動」（Boot）タブをクリックして、「セキュアブートメニュー」(Secure Boot)をクリックし、「OSタイプ」とあるところを「UEFIモード」にしましょう。

#### Secure key
今「セキュアブートメニュー」にいると思うので、「セキュアブートキーの削除」をクリック＆OKして、そのあと 「セキュアブートキーの初期化」もクリック＆OKしてください。これで BIOS の設定は終わりです。

### Boot する
これからこの画面を保存して閉じ、windows install を始めましょう。そのためには、「退出」（Exit）タブをクリックして、「保存して退出」（Save and Exit）を推せばよいです。すると自動的に windows install 開始画面に遷移します。少し時間が掛かります。

## 2. Windows Install
windows をインストールします。

### 言語～ライセンス条項
「言語と時刻」を「日本語」に、「キーボード」を「日本語キーボード(106/109キー)」にしましょう。そうしたら「次へ」を押して、表示された「今すぐインストール」のボタンを押しましょう。するとプロダクトキーが求められるので入力しましょう。配布されたテープに書いてある25桁の文字列です。ライセンス条項も表示されるので同意しましょう。

### パーティション
インストールの種類は「アップグレード」と「カスタム」があります。「アップグレード」は既にマシンにインストールされている windows を活かす感じで、「カスタム」は無視して一から作ります。ここでは「カスタム」を選びましょう。

すると、「Windows のインストール場所を選んでください。」と言われると思います。これは、マシンのどのメモリのどの辺を何に割り当てるかを決められるところです。ここでは「ドライブ 0 の割り当てられていない領域」に全振りしましょう。そのためには、他のすべての割り当てを削除すればよいです。

それが終わったら「次へ」を推せばインストールが始まり、自動的に再起動されます。少し時間が掛かります。

## 3. TAアカウントの作成
これは基本的には windows くんに言われるとおりにやればよいのですが、一つイレギュラーなこととして

<font color="Pink">※ 初めはTA用のアカウントを作ります</font>

ので注意しましょう。
- まず地域を選択します。「日本」が選ばれていることを確認し、「はい」を押します。
- キーボードレイアウトに「Microsoft IME」が選ばれていることを確認し、「はい」を押します。
- 二つ目のキーボードレイアウトは使用しないので、「スキップ」を押します。
- 「個人用に設定」を選び、「次へ」を押します。
- まずはTAのアカウントを作成します。この画面になったらTAを呼んでください。![アカウント作成画面](img/img3.JPG)
- Cortana の設定画面が出てくるので「後で設定する」をクリックします。
- Windows の初期設定では個人情報が Microsoft に送信されます。それを回避するため、プライバシー設定はすべてオフにして、「同意」を押してください。

これで Windows のインストールが終了しました。 Windows が立ち上がったら TA を呼んで TA アカウントにログインしてください。


## 5. 受講者用アカウントの設定
実習用のアカウントを作って管理者権限を付与します。それは「設定」から作ることができます。
- 「スタートメニュー」（左下のWindowsロゴをクリック）を開いてください。
- 歯車のアイコンをクリックしてください。
- 設定ウィンドウが出てきたら「アカウント」を選択してください。
- 「家族とその他のユーザー」を選択して、「その他のユーザーをこの PC に追加」を選択します。
- 「このユーザーのサインイン情報がありません」→「Microsoft アカウントを持たないユーザーを追加する」を選択します。
- 「この PC 用のアカウントの作成」が出てきたら、受講生用アカウントを作成します。ユーザー名は半角英数字で入力し、空白は含めないようにしてください。パスワードは他人には破られにくく自分では間違えないパスワードを設定しましょう。
- まず、今作成したアカウントをクリックすると出てくる「アカウントの種類の変更」をクリックしましょう。
- 「アカウントの種類」を「管理者」に変更して「OK」をクリックします。
- TAのアカウントはログアウトし、今作成した受講生用のアカウントにログインしてください。
