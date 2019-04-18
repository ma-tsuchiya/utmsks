<!--- 画面の写真を貼るところから--->
![BIOS 設定画面](img/img1.JPG)

### BIOS の設定をする
表示言語はおそらく英語か日本語になっていると思います。どちらでも問題ないのですが、変えるには左上の「English」とか書いてある部分をクリックしてプルダウンメニューで選べば大丈夫です。ここで触るのは次の3つです。

- Secure boot key
- Boot priority


#### Secure key
- windows は boot するときに、UEFI（Unified Extensible Firmware Interface）を用いることを義務付けているので、従います。
- Securityタブを開きます。
- Install default Secure Boot Keysをクリック＆Yesしてください。



#### Boot priority
ディスクの起動順を変更します。

- Bootタブを開きます
- BootOption #1　をUEFI Sandisk Extremeに設定します。
これでBIOSの設定は終わりです。

### Boot する
これからこの画面を保存して閉じ、windows install を始めましょう。

- Exitタブを開きます。
- Save Change & Exitをクリック＆Yesしてください。

すると自動的に windows install 開始画面に遷移します。少し時間が掛かります。
