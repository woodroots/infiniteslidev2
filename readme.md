# Infiniteslide.js v2

要素を無限スクロールさせるjQueryプラグインです。
CSS3 Animationを使用しているため、滑らかです。

### 対応ブラウザ
Flexboxと@keyframeによるアニメーションを使用しているため、IE10以上、Android4.4以上です。

## デモ
<http://wood-roots.com/sample/infiniteslidev2/>

##ブログ記事
<http://wood-roots.com/?p=1975>


## 使い方

	<script src="https://code.jquery.com/jquery-1.12.4.min.js"></script>
	<script src="infiniteslidev2.js"></script>

	<script type="text/javascript">
		$(function(){
			$('.infiniteslide').infiniteslide({
				'speed': 100, //速さ　単位はpx/秒です。
				'direction': 'left', //up/down/left/rightから選択
				'pauseonhover': true, //マウスオーバーでストップ
				'responsive': false, //子要素の幅を%で指定しているとき
				'clone': 1 //子要素の複製回数
			});
		});
	</script>

	<!-- 途中略 -->

	<div class="infiniteslide">
		<ul>
			<li><img src="img/1.jpg" alt="" /></li>
			<li><img src="img/2.jpg" alt="" /></li>
			<li><img src="img/3.jpg" alt="" /></li>
			<li><img src="img/4.jpg" alt="" /></li>
		</ul>
	</div>


## オプション
オプションは5種類です。

+   `speed` : 速さ
+   `direction` : 向き（up/down/left/right　より選択）
+   `pauseonhover` : マウスオーバーでアニメーションをストップする（true/false)
+   `responsive` : レスポンシブ対応するかどうか。スライドの子要素を%で指定している場合はtrueにしてください。
+   `clone` : 子要素を複製する回数。子要素の数が少なくループが途切れる場合は2以上を指定してください。


## 更新情報
2017.07.11 cloneオプションの追加。
2017.07.10 初版公開