
# 1. はじめに(Introduction)

このドキュメントでは、[Scratch 3.0](https://scratch.mit.edu/download)でビデオモーションセンサーを使ったゲームの作成方法を説明します。

This document explains how to develop games using video sensing in [Scratch 3.0](https://scratch.mit.edu/download).

ドキュメント作成者：脇本 一彌

Document Author：Kazuya Wakimoto

![Common](figure/top-balloon_game.gif)

# 2. 準備(Preparation)

## 2-1. 準備①:開発環境(Preparation①:Development environment)

- [Scratch公式サイト(https://scratch.mit.edu/download)](https://scratch.mit.edu/download)から、Scratch 3.0をダウンロード、インストールする。(Scratch 3.0は、Windows、macOS、chromeOS、Androidに対応。(2020/05/06時点))

  Download and install Scratch 3.0 from the [Scratch official website(https://scratch.mit.edu/download)](https://scratch.mit.edu/download).(Scratch 3.0 is compatible with Windows, macOS, chromeOS, Android. (As of 2020/05/06))

- 開発で使うパソコン等に、カメラがついていることを確認してください。

  Confirm that the camera is attached to the personal computer or other device used for development. 

- カメラが使用可能であることを確認してください。

  Confirm the camera is ready for use.

## 2-2.準備②：拡張機能(Preparation②:Plugin)

- Scratch 3.0を起動後、![plugin](figure/plugin.png) をクリックしてください。

  After launching Scratch 3.0, click on ![plugin](figure/plugin.png).

![start-plugin](figure/start-plugin.png)

- **『ビデオモーションセンサー』を追加** してください。

  Add a "Video Motion Sensor".

![plugin-screen](figure/start-plugin-screen.png)

- ビデオモーションセンサーが追加されていることを確認してください。

  Confirm you have added a video motion sensor.

![start-vmc](figure/start-vmc.png)

# 3. 作り方(How to develop)

## 3-1.作る前の準備(Preparation before developing)

- Scratch 3.0を起動し、スプライト1を削除してください。(スプライト1を選択→×をクリック)

  Start Scratch 3.0 and delete sprite 1.(Select sprite 1　→　Click ×)

![sprite_cat-delete](figure/predev-sprite-cat-delete.png)

- ![sprite-button](figure/predev-sprite-button.png)をクリックしてください。

  Click on the![sprite-button](figure/predev-sprite-button.png)button.

- Baloon1を選択、クリックしてください。

  Select a Baloon1 and click on it.

![add-sprite](figure/predev-add-sprite.png)

- スプライトが設定されていることを確認してください。

  Confirm that the selected sprite is set.

![predev-confirm-sprite](figure/predev-confirm-sprite.png)

- 大きさを **『90』** に変更してください。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  change the size to "70".(Double-clicking on a number, you will be able to edit the number.)

  ![predev-set-size](figure/predev-set-size.png)

## 3-2. プログラムの作り方(How to develop a program)

### 3-2-1.完成イメージ(Completed image)

![dev-program-complate](figure/dev-program-complate.png)

### 3-2-2. 詳細(Details)

- ![dev-variable](figure/dev-variable.png)を押してください。

  Press ![dev-variable](figure/dev-variable.png).

- ![dev-make-variable](figure/dev-make-variable.png)を押してください。
  Press![dev-make-variable](figure/dev-make-variable.png).

- 以下の画面が表示されるので、 **『変数名』を『とくてん』に変更** してください。

  When the following screen is displayed, change the "Variable Name" to "Score" and press the OK button.

![dev-set-variable](figure/dev-set-variable.png)

- 同じ手順で、**『たかさ』、『はば』**を作ってください。
  
  In the same way to make "Height" and "Width"

- **『とくてん』、『たかさ』、『はば』**を作ったら**とくてんのみ**にチェックをしてください。

  Check only "Score"
  
  ![dev-check-variable](figure/dev-check-variable.png)

- 以下のブロックを画面中央にドラック＆ドロップします。

  Drag and drop the following blocks to the center of the screen.

![dev-event](figure/dev-event.png) ![dev-flag](figure/dev-flag.png)

![dev-video-sensing](figure/dev-video-sensing.png) ![dev-turnon-video](figure/dev-turnon-video.png)

![dev-movement](figure/dev-movement.png) ![dev-set-xy](figure/dev-set-xy.png)

![dev-movement](figure/dev-movement.png) ![dev-static-rotate](figure/dev-static-rotate.png)

- 以下のブロックを**3つ**画面中央にドラック＆ドロップします。

  Drag and drop the following three blocks to the center of the screen.

![dev-variable](figure/dev-variable.png) ![dev-set-height](figure/dev-set-height.png)

- ![dev-set-xy](figure/dev-set-xy.png)の**左の数字を0、右の数字を94**に変更します。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  Change the number on the left to 0 and the number on the right to 94.(Double-clicking on a number, you will be able to edit the number.)

![dev-set-xy_2](figure/dev-set-xy_2.png)

- ![dev-set-height](figure/dev-set-height.png)の▼ボタンを押し、表示される変数の一覧から **『とくてん』** を選んでください。

  Press the ▼ button on ![dev-set-height](figure/dev-set-height.png) and select "Score" from the list of variables displayed.

![dev-score](figure/dev-score.png)

- ![dev-set-height](figure/dev-set-height.png)の▼ボタンを押し、表示される変数の一覧から **『はば』** を選んでください。

  Press the ▼ button on ![dev-set-height](figure/dev-set-height.png) and select "Width" from the list of variables displayed.

![dev-width](figure/dev-width.png)

- ブロックをくっつけてください。

  Connect the blocks.

![dev-connect-initial](figure/dev-connect-initial.png)

- 以下のブロックを画面中央にドラック＆ドロップします。

  Drag and drop the following blocks to the center of the screen.

![dev-event](figure/dev-event.png) ![dev-flag](figure/dev-flag.png)

![dev-control](figure/dev-control.png) ![dev-while](figure/dev-while.png)

![dev-variable](figure/dev-variable.png) ![dev-set-height](figure/dev-set-height.png)

![dev-variable](figure/dev-variable.png) ![dev-variable-height](figure/dev-variable-height.png)

![dev-movement](figure/dev-movement.png) ![dev-set-xy](figure/dev-change-y.png)

- ![dev-height](figure/dev-set-height.png)の数字を**-3に変更**します。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  Change the number![dev-height](figure/dev-set-height.png)to -3.(Double-clicking on a number, you will be able to edit the number.)

![dev-set-height_1](figure/dev-set-height_1.png)

- ![dev-change-y](figure/dev-change-y.png)の**10**に![dev-variable-height](figure/dev-variable-height.png)をドラッグ&ドロップしてください。

  Drag and drop the![dev-variable-height](figure/dev-variable-height.png) into "10" in ![dev-change-y](figure/dev-change-y.png)

![dev-change-y-to-h](figure/dev-change-y-to-h.png)

- ブロックをくっつけてください。

  Connect the blocks.

![dev-connect-main_01](figure/dev-connect-main_01.png)

- 以下のブロックを画面中央にドラック＆ドロップします。

  Drag and drop the following blocks to the center of the screen.

![dev-control](figure/dev-control.png)  ![dev-if](figure/dev-if.png)

![dev-calc](figure/dev-calc.png) ![dev-vs-cond](figure/dev-cond_01.png)

![dev-video-sensing](figure/dev-video-sensing.png)  ![dev-video-sensing-variable](figure/dev-video-sensing-variable.png)

![dev-variable](figure/dev-variable.png)   ![dev-change-variable](figure/dev-change-variable.png)

![dev-sound](figure/dev-sound.png)  ![dev-play-sound](figure/dev-play-sound.png)

![dev-variable](figure/dev-variable.png)  ![dev-set-height](figure/dev-set-height.png)

- ![dev-if](figure/dev-if.png)の6角形の空いているところに![dev-vs-cond](figure/dev-cond_01.png)をドラッグ＆ドロップしてください。

  Drag and drop the![dev-vs-cond](figure/dev-cond_01.png) into blanks in ![dev-if](figure/dev-if.png)

- ![dev-vs-cond](figure/dev-cond_01.png)の左の空いているところを**30に変更**し、右に![dev-video-sensing-variable](figure/dev-video-sensing-variable.png)をドラッグ&ドロップします。(空いているところをクリックすることで、数字を編集できる状態になります。)

  Change the left blanks to "30", and drag and drop the ![dev-video-sensing-variable](figure/dev-video-sensing-variable.png) into right in ![dev-vs-cond](figure/dev-cond_01.png)

![dev-changed-if_01](figure/dev-changed-if_01.png)

- ![dev-change-variable](figure/dev-change-variable.png)の▼ボタンを押し、表示される変数の一覧から **『とくてん』** を選んでください。

  Press the ▼ button on ![dev-change-variable](figure/dev-change-variable.png) and select "Score" from the list of variables displayed.

![dev-changed-score](figure/dev-changed-score.png)

- ![dev-set-height](figure/dev-set-height.png)の数字を**20に変更**します。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  Change the number![dev-height](figure/dev-set-height.png)to 20.(Double-clicking on a number, you will be able to edit the number.)

![dev-changed-height_01](figure/dev-changed-height_01.png)

- ブロックをくっつけてください。

  Connect the blocks.

![dev-connect-main_02](figure/dev-connect-main_02.png)

- 以下のブロックを画面中央にドラック＆ドロップします。

  Drag and drop the following blocks to the center of the screen.

![dev-control](figure/dev-control.png)  ![dev-for](figure/dev-for.png)

![dev-calc](figure/dev-calc.png) ![dev-vs-cond-equal](figure/dev-cond-equal.png)

![dev-variable](figure/dev-variable.png)   ![dev-change-variable](figure/dev-change-variable.png)

![dev-movement](figure/dev-movement.png)  ![dev-change-y](figure/dev-change-y.png)

![dev-variable](figure/dev-variable.png)  ![dev-variable-height](figure/dev-variable-height.png)

![dev-variable](figure/dev-variable.png)  ![dev-variable-height](figure/dev-variable-height.png)

- ![dev-for](figure/dev-for.png)の6角形の空いているところに![dev-vs-cond-equal](figure/dev-cond-equal.png)をドラッグ＆ドロップしてください。

  Drag and drop the![dev-vs-cond-equal](figure/dev-cond-equal.png) into blanks in![dev-for](figure/dev-for.png)

- ![dev-vs-cond-equal](figure/dev-cond-equal.png)の左の空いているところに![dev-variable-height](figure/dev-variable-height.png)をドラッグ&ドロップし、右の数字を**0に変更**します。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  Drag and drop the ![dev-variable-height](figure/dev-variable-height.png) into the left blanks, and change the right number to 0. 

![dev-changed-for](figure/dev-changed-for.png)

- ![dev-change-y](figure/dev-change-y.png)の**10**に![dev-variable-height](figure/dev-variable-height.png)をドラッグ&ドロップしてください。

  Drag and drop the ![dev-variable-height](figure/dev-variable-height.png) into "10" in ![dev-change-y](figure/dev-change-y.png)

![dev-change-y-to-h](figure/dev-change-y-to-h.png)

- ![dev-change-variable](figure/dev-change-variable.png)の数字を**-1に変更**します。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  Change the number![dev-change-variable](figure/dev-change-variable.png) to -1.(Double-clicking on a number, you will be able to edit the number.)

![dev-changed-height_02](figure/dev-changed-height_02.png)

- ブロックをくっつけてください。

  Connect the blocks.

![dev-connect-main_03](figure/dev-connect-main_03.png)

- 以下のブロックを画面中央にドラック＆ドロップします。

  Drag and drop the following blocks to the center of the screen.

![dev-control](figure/dev-control.png)  ![dev-if](figure/dev-if.png)

![dev-calc](figure/dev-calc.png) ![dev-vs-cond](figure/dev-cond_01.png)

![dev-movement](figure/dev-movement.png)  ![dev-y](figure/dev-y.png)

![dev-sound](figure/dev-sound.png)  ![dev-play-sound](figure/dev-play-sound.png)

![dev-control](figure/dev-control.png)   ![dev-stop](figure/dev-stop.png)

- ![dev-if](figure/dev-if.png)の6角形の空いているところに![dev-vs-cond](figure/dev-cond_01.png)をドラッグ＆ドロップしてください。
  Drag and drop the![dev-vs-cond](figure/dev-cond_01.png) into blanks in ![dev-if](figure/dev-if.png)

-  ![dev-vs-cond](figure/dev-cond_01.png)の左の空いているところに![dev-y](figure/dev-y.png)をドラッグ&ドロップし、右の数字を**-140に変更**します。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  Drag and drop the ![dev-y](figure/dev-y.png) into the left blanks, and change the right number to -140. 

![dev-changed-if_02](figure/dev-changed-if_02.png)

- ブロックをくっつけてください。

  Connect the blocks.

![dev-connect-main_04](figure/dev-connect-main_04.png)

- 以下のブロックを画面中央にドラック＆ドロップします。

  Drag and drop the following blocks to the center of the screen.

![dev-event](figure/dev-event.png) ![dev-flag](figure/dev-flag.png)

![dev-control](figure/dev-control.png) ![dev-while](figure/dev-while.png)

![dev-control](figure/dev-control.png) ![dev-loop](figure/dev-loop.png)

![dev-calc](figure/dev-calc.png) ![dev-random](figure/dev-random.png)

![dev-calc](figure/dev-calc.png) ![dev-random](figure/dev-random.png)

![dev-variable](figure/dev-variable.png)  ![dev-variable-width](figure/dev-variable-width.png)

![dev-variable](figure/dev-variable.png)  ![dev-set-height](figure/dev-set-height.png)

![dev-movement](figure/dev-movement.png)  ![dev-change-x](figure/dev-change-x.png)

![dev-movement](file:///Users/kazuya.wakimoto/develop/scratch_edu/balloon_game/figure/dev-movement.png?lastModify=1588769459)  ![dev-bounce](figure/dev-bounce.png)

- ![dev-loop](figure/dev-loop.png)の**『10』**に![dev-random](figure/dev-random.png)をドラッグ＆ドロップしてください。

  Drag and drop the ![dev-random](figure/dev-random.png) into "10" in ![dev-loop](figure/dev-loop.png)

- ![dev-random](figure/dev-random.png)の**左の数字を50、右の数字を100**に変更します。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  Change the left number to 50, right number to 100.(Double-clicking on a number, you will be able to edit the number.)

![dev-changed-loop_01](figure/dev-changed-loop_01.png)

- ![dev-set-height](figure/dev-set-height.png)の▼ボタンを押し、表示される変数の一覧から **『はば』** を選んでください。

  Press the ▼ button on ![dev-set-height](figure/dev-set-height.png) and select "Width" from the list of variables displayed.

- ![dev-set-height](figure/dev-set-height.png)の**『0』**に![dev-random](figure/dev-random.png)をドラッグ＆ドロップしてください。

  Drag and drop the ![dev-random](figure/dev-random.png) into "0" in ![dev-set-height](figure/dev-set-height.png)

- ![dev-random](figure/dev-random.png)の**左の数字を-5、右の数字を0**に変更します。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  Change the left number to -5, right number to 0.(Double-clicking on a number, you will be able to edit the number.)

![dev-changed-width_01](figure/dev-changed-width_01.png)

- ![dev-change-x](figure/dev-change-x.png)の**『10』**に![dev-variable-width](figure/dev-variable-width.png)をドラッグ＆ドロップしてください。

  Drag and drop the ![dev-variable-width](figure/dev-variable-width.png) into "10" in ![dev-change-x](figure/dev-change-x.png)
  
  ![dev-changed-x](figure/dev-changed-x.png)

- ブロックをくっつけてください。

  Connect the blocks.

![dev-connect-sub_01](figure/dev-connect-sub_01.png)

- 以下のブロックを画面中央にドラック＆ドロップします。

  Drag and drop the following blocks to the center of the screen.

![dev-control](figure/dev-control.png) ![dev-loop](figure/dev-loop.png)

![dev-calc](figure/dev-calc.png) ![dev-random](figure/dev-random.png)

![dev-calc](figure/dev-calc.png) ![dev-random](figure/dev-random.png)

![dev-variable](figure/dev-variable.png)  ![dev-variable-width](figure/dev-variable-width.png)

![dev-variable](figure/dev-variable.png)  ![dev-set-height](figure/dev-set-height.png)

![dev-movement](figure/dev-movement.png)  ![dev-change-x](figure/dev-change-x.png)

![dev-movement](file:///Users/kazuya.wakimoto/develop/scratch_edu/balloon_game/figure/dev-movement.png?lastModify=1588769459)  ![dev-bounce](figure/dev-bounce.png)

- ![dev-loop](figure/dev-loop.png)の**『10』**に![dev-random](figure/dev-random.png)をドラッグ＆ドロップしてください。

  Drag and drop the ![dev-random](figure/dev-random.png) into "10" in ![dev-loop](figure/dev-loop.png)

- ![dev-random](figure/dev-random.png)の**左の数字を50、右の数字を100**に変更します。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  Change the left number to 50, right number to 100.(Double-clicking on a number, you will be able to edit the number.)

![dev-changed-loop_01](figure/dev-changed-loop_01.png)

- ![dev-set-height](figure/dev-set-height.png)の▼ボタンを押し、表示される変数の一覧から **『はば』** を選んでください。
  Press the ▼ button on ![dev-set-height](figure/dev-set-height.png) and select "Width" from the list of variables displayed.

- ![dev-set-height](figure/dev-set-height.png)の**『0』**に![dev-random](figure/dev-random.png)をドラッグ＆ドロップしてください。

  Drag and drop the ![dev-random](figure/dev-random.png) into "0" in ![dev-set-height](figure/dev-set-height.png)

- ![dev-random](figure/dev-random.png)の**左の数字を0、右の数字を5**に変更します。(数字をダブルクリックすることで、数字を編集できる状態になります。)

  Change the left number to 0, right number to 5.(Double-clicking on a number, you will be able to edit the number.)

![dev-changed-width_02](figure/dev-changed-width_02.png)

- ![dev-change-x](figure/dev-change-x.png)の**『10』**に![dev-variable-width](figure/dev-variable-width.png)をドラッグ＆ドロップしてください。

  ![dev-changed-x](figure/dev-changed-x.png)

- ブロックをくっつけてください。

  Connect the blocks.

![dev-connect-sub_02](figure/dev-connect-sub_02.png)



# 4. 音の変更方法(How to change the sound)

- 『音』をクリックしてください。

  Click on the ”Sound” tab.

![sound-select-tab](figure/sound-select-tab.png)

- ![sound-select-sound-button](figure/sound-select-sound-button.png)をクリックしてください。

  Click on the![sound-select-sound-button](figure/sound-select-sound-button.png)button.

![sound-select-sound](figure/sound-select-sound.png)

- 『A Bass』をクリックしてください。

  Click on the "A Bass" tile.

![sound-add-sound](figure/sound-add-sound.png)

- 『コード』をクリックしてください。

  Click on the "Code" tab.

![sound-return-code](figure/sound-return-code.png)



- 以下のブロックを画面中央にドラック＆ドロップします。

  Drag and drop the following blocks to the center of the screen.

![dev-sound](figure/dev-sound.png)  ![dev-play-sound](figure/dev-play-sound.png)



- ![dev-play-sound](figure/dev-play-sound.png)の▼ボタンを押し、表示される一覧から **『A Bass』** を選んでください。

  Press the ▼ button on ![dev-play-sound](figure/dev-play-sound.png) and select "A Bass" from the list displayed.

![sound-change-sound](figure/sound-change-sound.png)






# 5. プログラムの保存方法(How to save the program)

Scrachのファイルのメニューから『コンピューターに保存する』を選択し、実行してください。

From the Scrach file menu, select "Save to computer" and run it.

![save](figure/save.png)

# 6. プログラムの実行・停止方法(How to run and stop the program)

## 6-1. プログラムを実行(Run the program)

旗のボタンを押してください。

Press the flag button.

![run](figure/run_app_button.png)

## 6-2. プログラムを停止(Stop the program)

赤いボタンを押してください。

Press the red button.

![stop](figure/stop_app_button.png)