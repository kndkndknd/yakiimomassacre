# 2021年2月3日の焼き芋まさかー
## これなに
* [k/a/t/o/ massacre vol.308](https://twitter.com/NOVO_vintage/status/1356206559433379842)でのkndの演目です
### なにするもの
* アクセスしたそれぞれの端末でGPSの取得座標からある地点への距離を計算し、その分だけ音程を高くしたサイン波を再生します
* 何人かいる場だとそれぞれの距離差がサイン波の周波数の差として聴き取ることができ、移動すると音が変化します
* テキストをリアルタイムに全端末にお届けする機能を持ち、動き方などの指示が出るとテキストによるサイン波の音程操作、演奏行為が発生します
* カメラの情報を取得し、ときには皆で撮影会をしたいと考えています、参加は任意で。
* 公園にいないひとの端末は一人でサイン波を再生しても寂しいので、個別のURLで参加者全員分のサイン波を鳴らすようにもできます（比べると動作が重たいのでスペックのいいスマホか、パソコンでの再生をおすすめします）
### 仕組み
* それぞれのアクセスするページのjavascriptでGPS（）とカメラ情報（getUserMedia）の取得を行っています。
* テキストなどの端末間のリアルタイム通信にはsocket.ioを使っています。今回3.X.Xにあげたらだいぶ使い方が変わっててびっくりしました
### 文脈
* この仕組をつくった経緯、これまで作った同様の仕組について書こうと思ってます。あとで書く