---
lab:
  title: 'ラボ 1:データからキャンバス アプリを作成する'
  module: 'Module 1: Get started with Power Apps canvas apps'
---

# 実習ラボ 1 - データからキャンバス アプリを作成する

このラボでは、既存のデータ ソースからキャンバス アプリを設計し、ビルドします。

## 学習する内容

- CoPilot を使ってデータから Power Apps キャンバス アプリを作成する方法
- OneDrive for Business をデータ ソースとして使って Excel に接続する方法

## ラボ手順の概要

- 3 画面のキャンバス アプリを作成する
- アプリをテストする
- CoPilot を使ってキャンバス アプリを作成する
  
## 前提条件

- 以下を完了している必要があります: 「**ラボ 0: ラボ環境を検証する**」

## 詳細な手順

## 演習 1 - データを取得する

### タスク 1.1 - Excel スプレッドシートをダウンロードする

1. [CoffeeMachineData.xlsx](https://github.com/MicrosoftDocs/mslearn-developer-tools-power-platform/blob/master/power-apps/coffee-machine-data/CoffeeMachineData.xlsx) に移動します。

1. **[Raw]** ファイル ボタンを選び、Excel ブックをダウンロードします。

    ![GitHub の [Raw] ダウンロード アイコンのスクリーンショット。](../media/raw-download.png)

### タスク 1.2 OneDrive for Business にアップロードする

1. [Power Apps Maker ポータル](https://make.powerapps.com)で、ブラウザー ウィンドウの左上にある**アプリ起動ツール**を選び、**[OneDrive]** を選びます。

    ![OneDrive アイコンのスクリーンショット。](../media/select-onedrive.png)

1. **[OneDrive の準備ができました]** を選びます。

1. **[+ 新規追加]** を選び、次に **[ファイルのアップロード]** を選びます

    ![OneDrive ファイルのアップロードのスクリーンショット。](../media/select-onedrive-upload.png)

1. [ダウンロード] に移動し、CoffeeMachineData.xlsx ファイルを選び、**[開く]** を選びます。

1. **[マイ ファイル]** を選び、CoffeeMachineData.xlsx がアップロードされていることを確認します。

## 演習 2 – 3 画面のキャンバス アプリをビルドする

### タスク 2.1 - アプリを作成する

1. Power Apps Maker ポータル <https://make.powerapps.com> に移動します。

1. **Dev One** 環境内にいることを確認します。

1. 左側のメニューから **[+ 作成]** タブを選びます。

1. **[開始]** の下にある **[Excel]** タイルを選びます。

    ![[開始] の [Excel] のスクリーンショット。](../media/start-from-excel.png)

1. **[+ 新しい接続]** を選びます

1. **[OneDrive for Business]** を選び、**[作成]** を選び、テナントの資格情報を使ってサインインして **[アクセスを許可]** を選びます。

1. [Excel ファイルの選択] で、**CoffeeMachineData.xlsx** Excel ファイルを見つけて選びます。

1. [テーブルの選択] で **CoffeeMachines** を選びます。

1. **[接続]** を選択します。

1. アプリが作成されるまで待ちます。

    ![3 画面のアプリの [参照] 画面を示すスクリーンショット。](../media/three-screen-app-browse-screen.png)

1. **[Power Apps Studio へようこそ]** ポップアップ ダイアログが表示されたら、**[今後このメッセージを表示しない]** を選び、**[スキップする]** を選びます。

1. Power Apps Studio の右上にある **[保存]** を選び、「`Coffee Machines App`」と入力して、**[保存]** を選びます。

### タスク 2.2 - アプリをテストする

1. Power Apps Studio の右上にある **[アプリのプレビュー]** アイコンを選びます。

1. ギャラリー内の任意のマシンを選びます。 これで詳細画面に移動します。

1. アプリの右上にある **[編集]** アイコンを選びます。 これで [編集] 画面が開きます。

1. **[Machine Price]** を変更し、アプリの右上にある **[項目の送信]** チェック アイコンを選びます。

1. アプリの左上にある **<** アイコンを選びます。

1. アプリの右上にある **+** アイコンを選びます。

1. **[Machine ID]** に「`97`」と入力します。

1. **[Machine Name]** に「`Demo Machine`」と入力します。

1. **[Machine Price]** に「`999`」と入力します。

1. アプリの右上にある **[項目の送信]** アイコンを選びます。

1. **[検索項目]** に「`Demo`」と入力します。

1. 右上にある **[X]** を選んでプレビューを停止します。

1. **[ご存知でしたか?]** ポップアップ ダイアログが表示されたら、**[今後このメッセージを表示しない]** を選択し、**[OK]** 択します。

1. コマンド バーの左上にある **[戻る]** ボタン、**[終了]** の順に選択し、アプリを終了してください。

## 演習 3 - Copilot を使ってキャンバス アプリをビルドする

### タスク 3.1 - アプリを作成する

1. Power Apps Maker ポータル <https://make.powerapps.com> に移動します。

1. **Dev One** 環境にいることを確認します。

1. 左側のメニューから **[ホーム]** タブを選びます。

1. **[アプリをビルドしましょう。何をすべきでしょうか?]** に「`Track coffee machine repairs for customers and assign repairs to technicians`」と入力し、矢印アイコンを選びます。

    ![Copilot プロンプトのスクリーンショット。](../media/copilot-prompt.png)

1. 表を確認する

    ![Copilot テーブルのスクリーンショット。](../media/copilot-table.png)

1. **[アプリの作成]** を選びます

1. アプリが作成されるまで待ちます。

    ![Copilot によるアプリのスクリーンショット。](../media/copilot-app.png)

1. Power Apps Studio の右上にある **[保存]** を選択します。

1. コマンド バーの左上にある **[<- 戻る]** ボタン、**[終了]** の順に選択し、アプリを終了します。

1. Power Apps メーカー ポータルの左側のメニューから **[アプリ]** タブを選びます。
