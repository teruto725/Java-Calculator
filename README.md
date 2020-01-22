

動作環境

eclipse Neon.3

基本機能

・input　の後に計算式を入力することで演算ができます．計算式は逆ポーランド記法で入力してください．

(例)input : 3 2 +

3 2 + = 5

・計算式を&で区切ることで複数入力することができます．ただし，&の両側にスペースが入らないようにしてください

(例)input : 3 2 +&3 1+

3 2 + = 5

3 1 + = 4

・計算式内に
xX(x1,x2\...)を入れることによってX回前の演算結果と代入することができます．

(例)input : 3 2 +

3 2 + = 5

input : 3 x1 +

3 x1 + = 8

・マクロ機能があります．マクロを登録することで登録した演算を再度入力することなく使えるようになります．例えばv1
1.08 \*
を保存しておけばマクロを呼び出しv1を入力するだけで消費税が計算できるみたいな感じ．

コマンド

input : の後に計算式もしくは以下のコマンドを打ち込むことができます

・seido

任意精度を入力することができます．

> 「精度を入力」というメッセージの後に10\^(-X)におけるXに当たる自然数を入力してください．(例)2

・makemacro

マクロを作成することができます．

「マクロを入力」というメッセージの後にマクロを入力してください．

その際，変数はvX(v1,v2\...)というように定義してください．(例)v1 v2 +

・showmacro

> 登録されているマクロの一覧とその番号を確認することができます．マクロ番号はマクロが登録された順に割り振られます．

・deletemacro

登録されているマクロを削除することができます．

> 「削除したい番号を入力」というメッセージの後にマクロ番号を自然数で入力してください．

・use mX

登録されているマクロを使用することができます．

Xはshowmacroで示されているマクロ番号を指定してください．

対象となるマクロが表示されます．その後，各変数を入力してください

(例) input : use m1

v1 v2 +

v1 : 3

v2 : 2

3 2 + = 5

・end

電卓を終了します．

注意

・マクロ内の数字の精度はマクロを使用したときの精度に依存します．

・精度の初期設定は3です．