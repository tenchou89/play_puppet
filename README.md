# play_puppet
 攻殻機動隊(ghost in the shell)に出てくる笑い男の再現
 
![笑い男_Trim](https://user-images.githubusercontent.com/49236225/121814643-1a71b480-ccad-11eb-9939-ca0fe65eddc2.gif)

# 問題点
現状FPSを調べたらマイナス値が出たのでおそらく処理が重いのだろう。解決策としてはとしては、
- OPENCVのvideo libraryのモジュールの性能が貧弱。
- C++でやればいい
- 解像度を低くする
- カスケード識別機で顔を認識しているので認識処理が軽いアルゴリズムなどを採用する。
などを考えています。ほかにも以下の記事を参考にしながら修正

[OpenCVのカメラ読み込みを高速化し、遅延時間も短くする](https://qiita.com/iwatake2222/items/b8c442a9ec0406883950)

[ラズパイのOpenCV処理を速くする](http://project12513.blog-fps.com/raspberrypi%E9%96%8B%E7%99%BA/%E3%83%A9%E3%82%BA%E3%83%91%E3%82%A4%E3%81%A7opencv%E3%81%AE%E5%87%A6%E7%90%86%E3%82%92%E9%80%9F%E3%81%8F%E3%81%99%E3%82%8B)
