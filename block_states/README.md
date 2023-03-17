ブロック状態の一覧。

.md : これ。ファイルの説明とブロック状態関するメモ。  
.json : ブロックごとのブロック状態のデータ。

# .json

[xx].id : ブロックID。  
[xx].states : ブロック状態のリスト。  
[xx].states[xxx].name : ブロック状態名。  
[xx].states[xxx].value : ブロック状態値のリスト。  
[xx].states[xxx].value[xxx].state : ブロック状態値。ブロック状態によって値の型が違うことに注意。(真偽値・整数・文字列の3種)  
[xx].states[xxx].value[xxx].data : (他のブロック状態を0としたときの)ブロック状態値に対応するデータ値。対応するデータ値がないなら値は-1。  
[xx].states[xxx].default : ブロック状態値のデフォルト値。  
[xx].states[xxx].bit : ブロック状態がデータ値で使うビット。対応するデータ値がないなら値は0。例えば、0 - 5 の 0b0111 の範囲を使うなら値は0b0111 = 7。  

## Todo
* 使用できないブロック状態値を調査し省く

`"rail_direction"`は`0`から`9`までの整数値を取る。(公式のdocumentationに書かれているしβPre1.19.80.20以降の補完でも出てくる)  
が、`golden_rail ["rail_direction":6]`は設置できない。7, 8, 9もそう。

* ブロック状態に過不足がないか・データ値の振る舞い・ブロック状態値との対応関係を確かめる

もう全部じゃねぇか。めんどくせ

# データ値のメモ

1.19.70から使えなくなったが、バージョンを下げたfunctionなら使える。

例: golden_rail
"rail_direction"は0b0111、"rail_data_bit"は0b1000に対応する。
|データ値|バイナリ|rail_direction|rail_data_bit|
|-:|-:|-:|:-|
|0|0000|0|false|
|1|0001|1|false|
|2|0010|2|false|
|3|0011|3|false|
|4|0100|4|false|
|5|0101|5|false|
|6|0110|0|false|
|7|0111|0|false|
|8|1000|0|true|
|9|1001|1|true|
|10|1010|2|true|
|11|1011|3|true|
|12|1100|4|true|
|13|1101|5|true|
|14|1110|0|true|
|15|1111|0|true|
|16|10000|0|false|
|17|10001|0|false|
|18|10010|0|false|

各ブロック状態で、対応するブロック状態値がなければデフォルト値になる。(6, 7, 14, 15)  
ブロック状態全体での使用bit数を超えるとすべてのブロック状態値がデフォルト値になる。(16以降)

# 情報源

https://minecraft.fandom.com/wiki/Block_states  
Block states - Minecraft Wiki