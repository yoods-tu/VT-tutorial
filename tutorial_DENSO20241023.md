<!DOCTYPE html>

<html>

<head>
   <link href="/Users/tuchiyama/Desktop/md_manual/tutorial.css" rel="stylesheet"></link>
<h1>VTチュートリアルマニュアル構成
<br>ロボット接続編（DENSO）
</h1>
</head>
<br>

<table class="headpage" border=1>
   <tr> 
     <td>Revision</td>
     <td>第1版</td>
   </tr>
     <td>作成者</td>
     <td>株式会社YOODS</td>
   </tr>
   <tr>
     <td>作成日</td>
     <td>2024年3月25日</td>
   </tr>
　 <tr>
     <td>最終更新日</td>
     <td>2024年3月25日</td>
   </tr>
   <br>
</table>
<br>

<div class="pageblock">
<h2>7. データ通信設定（DENSO）</h2>
<table style="margin:auto" border=1>
    <tr>
      <td class="number">No</td>
      <td class="tejun">手順</td>
      <td class="hosoku">補足</td>
    </tr>
    <tr> 
      <td class="number">A140</td>
      <td class="tejun">ロボットのIPアドレスを設定します。
          <br><br>初期画面の下部「 設定 」メニューから
          <br>下記の順で選択してください。
          <br><br>1.「 通信と起動権 」
          <br><br>2.「 ネットワークと通信権 」
      </td>
      <td class="hosoku"><img class="data_setting" src="/Users/tuchiyama/Desktop/md_manual/image/img/1724129501848.png" alt="">
      <br><img class="data_setting" src="/Users/tuchiyama/Desktop/md_manual/image/img/1724129521739.png" alt="">
      </td>
    </tr>
    <tr> 
      <td>A141</td>
      <td>イーサネットを選択、下記項目を設定。
          <br><br>通信権：読込/書込可
          <br>DHCP：無効
          <br>IPアドレス：192.168.221.10
          <br>サブネットマスク：255.255.255.0
          <br><br>
      </td>
      <td><img class="data_setting" src="/Users/tuchiyama/Desktop/md_manual/image/img/1724129544258.png" alt="">
      <br>※IPアドレスはデフォルト値です。</td>
    </tr>
    <tr>
      <td>A142</td>
      <td>データ通信設定を行います。
          <br><br>初期画面の下部 「 設定 」 メニューから
          <br>下記の順で選択してください。
          <br><br>１．「 通信と起動権 」  
          <br><br>２．「 データ通信 」
          <br><br>
      </td>
      <td><img class="data_setting" src="/Users/tuchiyama/Desktop/md_manual/image/img/1724129572874.png" alt="">
      </td>
    </tr>
    <tr>
      <td>A143</td>
      <td>デバイス：イーサネットを選択
          <br>サーバ回線の設定を行います。
          <br>「サーバ回線番号４」を選択、右記項目を設定。
      </td>
      <td>TCP/UDP：TCP
          <br>ポート：50000
          <br>データタイプ：テキスト
          <br>デリミタ：LF
          <br><br>
      </td>
    </tr>  
    <tr>
      <td>A144</td>
      <td>デバイス：イーサネットを選択
　　　　　 <br>クライアント回線の設定を行います。
          <br>「クライアント回線15」を選択、右記項目を設定。
          <br><br>※IPアドレスはデフォルト値です。
          <br>クライアント回線で設定するIPアドレスは
          <br>PCのIPアドレスです。
          <br>チュートリアルA1-ロボット接続　A114を
          <br>参照してください。
      </td>
      <td>TCP/UDP：TCP
          <br>IPｱﾄﾞﾚｽ：192.168.221.2
          <br>ポート：8888
          <br>データタイプ：テキスト
          <br>デリミタ：LF
          <br>ヘッダ：なし
          <br><br>
      </td>
    </tr>  
</table>
</div>

<div class="pageblock">
<h2>8. プログラムのロード（DENSO）</h2>
<table class="programload" style="margin:auto" border=1>
    <tr>
      <td class="number">No</td>
      <td class="tejun">手順</td>
      <td class="hosoku">補足</td>
    </tr>
    <tr> 
      <td>A150</td>
      <td>PCデスクトップ「VTマニュアル」のリンクを選択して
          <br>ダブルクリックしてください。
          <br><br>使用するロボットメーカーのフォルダを開き
          <br>「Robot_program」のフォルダを開いてください。
      </td>
      <td>※ロボットコントローラとWINCAPSが接続、使用
          <br>出来る環境をご準備ください。
      </td>
    </tr>
    <tr> 
      <td>A151</td>
      <td>PCへUSB メモリを挿してください。
          <br><br>robot_programフォルダ内の
          <br>プログラムファイルを全てUSBへ
          <br>コピーしてください。
          <br><br>コピー完了後、USBを抜いてください。
          <br><br>
      </td>
      <td>
          USBメモリフォルダは自動で出てきますが
          <br>出ない場合、ファイルマネージャーを開いて
          <br>デバイス内のUSBフォルダを開いてください。
          <br><br>USBを抜く際は、ファイルマネージャー左側メニュー
          <br>デバイス内にあるUSBの
          <br> 
          <img class="programload" src="/Users/tuchiyama/Desktop/md_manual/image/img/1724130934532.png" alt="" >マークを押してから抜いてください。
          <br><br>
      </td>
    </tr>
    <tr>
      <td>A152</td>
      <td>
          <br>WINCAPSを使用しているPCへ
          <br>コピーしたプログラムファイルを移行し
          <br>WINCAPSの画面から
          <br>コピーしたプログラムをインポートしてください。
          <br><br>インポート後、右記のプログラムを
          <br>ロボットへ送信してください。
          <br><br><br>プログラムはルートフォルダに置いてください。
      </td>
      <td>
          プログラム
          <br>● VTSample.pcs
          <br>● VTMove.pcs  
          <br>● rovi.pcs  
          <br>● RCalib.pcs
          <br>● RCalibAuto.pcs
          <br>● tsr0011.pcs
      </td>
    </tr>
    <tr>
      <td>A153</td>
      <td>
          操作盤パネルプログラムを使用すると
          <br>TPから撮影等が実行できます。
          <br>ご使用の 「Main.pns9」 から
          <br>「rovi_panel.pns9」 を呼び出すように
          <br>変更してください。
          <br><br>
          </td>
      <td>
          操作盤パネルプログラム
          <br>● rovi_panel.pns9
      </td>
    </tr>  
    <tr>
      <td>A154</td>
      <td>
          WINCAPSのPanelDesignerで
          <br>「Main.pns9」へ右記コマンドを追加してください。
      </td>
      <td>
          プッシュボタンを追加する場合
          <br><br>Sub PB1_CLICKED()
          <br>　　 PageChange rovi_panel
          <br>End Sub
          <br><br>
      </td>
    </tr> 
</table>
</div>

<div class="pageblock" style="margin:auto" border=1>
<h2>9. 特権タスク設定（DENSO）</h2>

<table class="tasksetting" style="margin:auto" border=1>
    <tr>
      <td class="number">No</td>
      <td class="tejun">手順</td>
      <td class="hosoku">補足</td>
    </tr>
    <tr> 
      <td>A160</td>
      <td>
          PCへロボットの現在値（軸値）を
          <br>送信するため特権タスクを実行させます。
          <br><br>特権タスクで使用しているプログラムは
          <br>「 tsr0011.pcs 」 です。
          <br><br>
      </td>
      <td>
          ※VTの機能を使用する時は
          <br>　特権タスクが起動されている事を確認してください。
      </td>
    </tr>
    <tr> 
      <td>A161</td>
      <td>
          初期画面の下部 「 プログラム 」 メニューを選択
          <br><br>下部　「 補助機能 」　を選択し、
          <br>プログラム補助機能画面を開いてください。
          <br>
          <br>「 プログラムパラメータ 」　を選択してください。
      </td>
      <td>
      <img class="tasksetting" src="/Users/tuchiyama/Desktop/md_manual/image/img/1724131164924.png" alt="">
      </td>
    </tr>
    <tr>
      <td>A162</td>
      <td>
          項目名
      <br>「32. タスク終了時の通信回線自動切断」を
      <br>選択し、編集を押してください。
      <br>
      <br>「有効　１」 に設定後、プログラムパラメータ画面
      <br>下部 「 OK 」 ボタンを押して
      <br>設定を完了させてください。
      <br><br>
      </td>
      <td>
      <img class="tasksetting" src="/Users/tuchiyama/Desktop/md_manual/image/img/1724131209228.png" alt="">
      </td>
    </tr>
    <tr>
      <td>A163</td>
      <td>
          初期画面の下部 「 プログラム 」 メニューを選択
          <br>
          <br>下部 「 補助機能 」 を選択し、
          <br>プログラム補助機能画面を開いてください。
          <br>
          <br>「 プログラム設定 」を選択してください。
      </td>
      <td>
      <img class="tasksetting" src="/Users/tuchiyama/Desktop/md_manual/image/img/1724131532254.png" alt="">
      </td>
    </tr>  
    <tr>
      <td>A164</td>
      <td>
          プログラム設定画面の上部
      <br>「 特権タスク 」 を選択してください。
      <br>
      <br>下記、表の設定を行ってください。
      <br>
      <br>
      </td>
      <td></td>
    </tr>
</table>   
<br><br>
</div>
    <table class="programset" style="margin:auto" border=1>
    <tr>
      <th>項目</th>
      <th>設定内容</th>
    </tr>   
    <tr>
      <td>1. 電源立ち上げ時の起動設定</td>
      <td>ルートのみ起動</td>
    </tr> 
    <tr>
      <td>2. 電源立ち上げ時にエラー発生した場合の起動設定</td>
      <td>起動する</td>
    </tr>
    <tr>
      <td>3. 自動モード切替時の起動設定</td>
      <td>ルートのみ起動</td>
    </tr> 
    <tr>
      <td>4. 電源エラー発生時の停止対象</td>
      <td>全特権タスク</td>
    </tr> 
    <tr>
      <td>5. 特権タスク実行中のI/O出力設定</td>
      <td>任意（特権タスク起動中を監視したい場合はONに設定）</td>
    </tr>
    </table>  
<br>  
  <table class="tasksetting" style="margin:auto" border=1>
    <tr>
      <td class="number">A165</td>
      <td class="tejun">特権タスクはプログラム保存の操作を
      <br>行うと停止されます。
      <br>
      <br>停止後は、再度特権タスクを起動してください。
      <br>
      <br>
      </td>
      <td class="hosoku"></td>
    </tr>
    <tr>
      <td>A166</td>
      <td>
          特権タスク停止状態でPCから
      <br>撮影を実行すると、ロボットからの軸値送信が
      <br>できていないため 「 901 」 エラーが
      <br>発生します。
      <br>
      <br>エラー発生時は特権タスクを起動してください。
      <br>
      <br>
      </td>
      <td></td>
    </tr>
  </table>
</div>
<br>

<h2>10. 動作確認</h2>
  <table class="dousa" style="margin:auto" border=1>
    <tr>
      <td class="number">No</td>
      <td class="tejun">手順</td>
      <td class="hosoku">補足</td>
    </tr>
    <tr> 
      <td class="number">A170</td>
      <td class="tejun">デスクトップの VT 起動アイコンをダブルクリックして、
          <br>ビジュアルコントローラを起動します。
          <br>※起動済みの場合は、念のため再起動
      </td>
      <td class="hosoku" style="text-align:center"> 
      <img class="dousa" src="/Users/tuchiyama/Desktop/md_manual/image/img/1724132479205.png" alt="">
      <br>VT起動アイコン</td>
    </tr>
    <tr> 
      <td class="number">A171</td>
      <td class="tejun">
      ご使用のロボットが画面に表示されることを
          <br>確認します。
          <br>DHCP:無効
      </td>
      <td class="hosoku" style="text-align:center">
      <img class="dousa" src="/Users/tuchiyama/Desktop/md_manual/image/img/1724132525621.png" alt=""> 
      <br>画面上にロボットが表示されます。
     </td>
    </tr>
    <tr>
      <td class="number">A172</td>
      <td>TPでロボットを動かし、画面上のロボットと
      <br>実際のロボットの動きが連動していることを
      <br>確認してください。
      </td>
      <td>各軸座標系で6軸それぞれを動かし
          <br>連動しているか確認してください。
      </td>
    </tr>
    <tr>
      <td class="number">A173</td>
      <td>これで接続は全て完了です。</td>
      <td></td>
    </tr>
</table> 
</html>
