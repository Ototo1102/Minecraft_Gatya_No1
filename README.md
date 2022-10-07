<html>
    <body bgcolor="2B2B2B">
    <body>
<head>
 <h1>
 <font color="1CFFBB">-おとミニブログ-
 </font>
</h1> 
<p>
    <font size="5" color="CD03FF">>コマンド編<
    </font>
</p>
<p><img src="htmlimage/Impulse_Command_Block.png" alt="-すいません! なにかしらの原因で画像が表示されないようです!!-"></p>
<h1><font size="3" color="FCFCFC">今回はMinecraftJava版の「ガチャガチャ」の作り方を解説していきたいと思います!! </font></h1>
<h1><font size="3" color="FCFCFC">あ 初投稿でしたね笑 おとミニです!! よろしくお願いします!!笑 </font></h1>
<h1><font size="3" color="FCFCFC">まずこちらのコマンドをコピーしてしてコマンドを打ち込みます</font></h1>
<h1><font size="3" color="FCFCFC">/give @p bat_spawn_egg{display:{Name:'[{"text":"[tag:Gatya]","color":"aqua","bold":true},{"text":"アーマースタンドのスポーンエッグ","color":"#F7FF0A","bold":true}]'},EntityTag:{id:"minecraft:armor_stand",Tags:["Gatya"]}} 1</font></h1>
<p><img src="htmlimage/putcommandNo1.png" alt="何かしらの原因で画像が表示されないようです! "width="576" height="360"></p>
<h1><font size="3" color="FCFCFC">コマンドブロック入手コマンド「/give @p command_block」</font></h1>
<h1><font size="3" color="FCFCFC">次にコマンドブロックの中身を指定していきます。</font></h1>
<p><img src="htmlimage/command_Jyunnbann.png" alt="何かしらの原因で画像が表示されないようです! "width="576" height="360"></p>
<h1><font size="3" color="FCFCFC">この中身はガチャの中身のアイテム一個一個のコマンドになります。</font></h1>
<h1><font size="3" color="FCFCFC">例えば①は「/give @p apple 10」("りんごを10こ与える"という意味)を入れるとガチャの中身①がりんご10個になるということになります。</font></h1>
<h1><font size="3" color="FCFCFC">僕はこんな感じにしました!</font></h1>
<h1><font size="3" color="FCFCFC">①/give @p apple 10 ②/give @p minecraft:bread 10 ③/give @p minecraft:golden_apple 10</font></h1>
<h1><font size="3" color="FCFCFC">④/give @p minecraft:carrot 10 ⑤/give @p minecraft:cake 10</font></h1>
<h1><font size="3" color="FCFCFC">次にガチャの見た目を作ります! コマンドブロックを見せたくない場合は地面に埋めちゃって大丈夫です!</font></h1>
<p><img src="htmlimage/GatyaNo1.png" alt="何かしらの原因で画像が表示されないようです! "width="576" height="360"></p>
<h1><font size="3" color="FCFCFC">そしてこのコマンドを入力します。</font></h1>
<h1><font size="3" color="FCFCFC">/execute at @e[type=minecraft:armor_stand,tag=Gatya,limit=1,sort=random] run setblock ~ ~ ~ minecraft:redstone_block</font></h1>
<h1><font size="3" color="FCFCFC">意味は「tag「Gatya」を持っているアーマースタンドをランダムに一体選びそのモブにレッドストーンブロックを設置する。」</font></h1>
<h1><font size="3" color="FCFCFC">そしてこれができたらできたらボタンを押してみましょう!!</font></h1>
<h1><font size="3" color="FCFCFC">アイテムが出てきましたね!!</font></h1>
<h1><font size="3" color="FCFCFC">ですがこの状態だと何回も同じものが出てくることがありません! 手動でリセットするのはとてもめんどくさいですよね...笑</font></h1>
<h1><font size="3" color="FCFCFC">なのでこのような状態にします!!向きと色はしっかり揃えてくださいね!(上の部分には先ほどのコマンドを入れてください!)</font></h1>
<p><img src="htmlimage/GatyaFillNo1.png" alt="何かしらの原因で画像が表示されないようです! "width="576" height="360"></p>
<h1><font size="3" color="FCFCFC">次に画面のようにレッドストーンを敷き詰めます。この時座標の指定が難しい時何十回か押して下の画面のように埋め尽くすようにしてください。</font></h1>
<h1><font size="3" color="FCFCFC">埋め尽くすと言いましたが,右端と左端のレッドストーンブロックの座標だけわかれば大丈夫です!</font></h1>
<p><img src="htmlimage/GatyaNo1RedStoneBlock.png" alt="何かしらの原因で画像が表示されないようです! "width="576" height="360"></p>
<script src="https://code.jquery.com/jquery.min.js"></script>
<h1><font size="5" color="FF12D0">-座標の見方-(知っている方は飛ばしてください!)</font></h1>
    <h1><font size="3" color="FCFCFC">「F3キー」を押すことで座標を見ることができます。
<p><img src="htmlimage/ZahyouMikata.png" alt="何かしらの原因で画像が表示されないようです! "width="576" height="360"></p>
        こんな画面が出ると思うんですが,左側の中心ちょっと上あたりに「XYZ」というのがあると思います。
        それを「座標」と言います。 家の場所を覚えるために使われたり,コマンドで使ったりするので覚えといてくださいね笑
    </font></h1>
    <h1><font size="5" color="FF12D0">------------------------------------------------------------</font></h1>
    <h1><font size="3" color="FCFCFC">そうしたら下の水色に「/fill (レッドストーンブロック左の座標) (レッドストーンブロック右の座標) air」と入力してください。</font></h1>
    <h1><font size="3" color="FCFCFC">するとレッドストーンブロックが消えたと思います。 そしてもう一度押すと...</font></h1>
    <h1><font size="3" color="FCFCFC">アイテムがゲットできましたあああああ笑</font></h1>
    <h1><font size="3" color="FCFCFC">何回も押してみてください。 成功なら押してもレッドストーンが見えないと思います。 これで完成です!!</font></h1>
    <h1><font size="5" color="FF12D0">---確率調整方法---</font></h1>
    <h1><font size="3" color="FCFCFC">「でもこれじゃあ確率が調節できないじゃん...」と思った方もいるかもしれません。</font></h1>
    <h1><font size="3" color="FCFCFC">確率調整方法は簡単で確率を増やしたいところに先ほどのアーマースタンドを置くだけです!!</font></h1>
    <h1><font size="3" color="FCFCFC">そうするとアーマースタンドを置いたところの確率を増やすことができます!</font></h1>
    <h1><font size="5" color="FF12D0">------------------------------------------------------------</font></h1>
    <h1><font size="3" color="FCFCFC">今回のガチャの作り方は以上です!</font></h1>
    <h1><font size="3" color="FCFCFC">とっても簡単にできたんじゃないでしょうか!笑</font></h1>
    <h1><font size="3" color="FCFCFC">是非覚えてくださいね笑</font></h1>
    <h1><font size="3" color="FCFCFC">ではまた!!</font></h1>
    
</div>
</body>
</head>
</html>
