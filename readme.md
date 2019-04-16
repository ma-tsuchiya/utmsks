---
title: Windows インストールマニュアル
author: ngtkana
---
# Windows インストールマニュアル
## 作業の流れと解説

※ まだ電源を入れないでください。

この作業は

- BIOS の設定
- Windows インストール

の二段階に分かれます。コンピューターの電源を入れるとまずは OS（operating system）などの基本的なソフトウェアをメモリに展開し、各種アプリケーションが使える状態にしなければなりません。通常それは BIOS （バイアス、Basic Input/Output System）により自動的に行われますが、今回は USB メモリからそれを行いたいので、BIOS の設定を変えて起動します。以下そのやり方を記述します。

## BIOS の設定
※まだ電源を入れないでください

放っておくと BIOS は設定された通りの手順でブートしてしまうのでそれを中断して、人類の言うとおりにブートしていただけるように設定します。以下その手順を記述します。

### USB メモリをいれる
TA の配布する USB メモリに Windows が入っているので、それを USB ポートに挿してください。差込口が青いものと白いものが両方あるので、青い方に挿し込むと良いと思います。

### 電源を入れてDel連打
お待ちかねです！ 電源を入れましょう

### （日本語に替える）
## UEFI:SanDisk Extreme （UEFI:SanDisk Extreme 0001, Partition1 (30433MB)）をドラッグで一番上に。
## Advanced Mode （F7か右下クリック）
## 起動（Boot）タブ→セキュアブートメニュー(Secure Boot)→OSタイプ:UEFIモード

## 「セキュアブートキーの削除」
## 「セキュアブートキーの初期化」
## 帯出（Exit）→OK
## 
## 

# 新しい方
## F2orDel -> UEFI menu
## Bootタブ
## 「Boot Priority」のリストの1番上に「UEFI: SanDisk Extreme」
## Advanced(orF7)
## ??
## ??
## Save Change and Exit


# Windows Install
# ネットワークを設定しよう スキップ
# 後で時間を節約するために今すぐ接続 スキップ

# コルタナ スキップ 
# アクセシビリティ スキップ
# デバイスのプライバシー 同意