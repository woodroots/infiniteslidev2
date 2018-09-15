# Infiniteslide.js v2

[日本語の解説はこちら](#ja)

Infiniteslide.js v2 is jQuery plugin that is scrolling infinite.
This is using CSS3 Animation (keyframes), so smooth and light for browser.

### Browser Support
Infiniteslide.js v2 use Flexbox and @keyfremas.
so over IE10,Android 4.4.

## Demo
<http://wood-roots.com/sample/infiniteslidev2/>

## Blog Article
Sorry japanese only.
<http://wood-roots.com/?p=1975>

## Usage
	<script src="https://code.jquery.com/jquery-1.12.4.min.js"></script>
	<script src="infiniteslidev2.js"></script>
	<!--
	if using jsdelivr,write this.
	<script src="https://cdn.jsdelivr.net/npm/infiniteslidev2/infiniteslidev2.min.js"></script>
	-->
	<script type="text/javascript">
		$(function(){
			$('.infiniteslide').infiniteslide({
				'speed': 100, //speed this is px/min
				'direction': 'left', //choose  up/down/left/right
				'pauseonhover': true, //if true,stop onmouseover
				'responsive': false, //width/height recalculation on window resize. child element's width/height define %/vw/vh,this set true.
				'clone': 1 //if child elements are too few (elements can't "infinite"), set 2 or over.
			});
		});
	</script>

	<!-- omitted -->

	<div class="infiniteslide">
		<ul>
			<li><img src="img/1.jpg" alt="" /></li>
			<li><img src="img/2.jpg" alt="" /></li>
			<li><img src="img/3.jpg" alt="" /></li>
			<li><img src="img/4.jpg" alt="" /></li>
		</ul>
	</div>

## Options
+   `speed` : speed / px/min
+   `direction` : direction（choose up/down/left/right）
+   `pauseonhover` : animation stop on mouseover （true/false)
+   `responsive` : responsive support
+   `clone` : Number of times to duplicate child elements. If the number of child elements is small and the loop is interrupted, specify 2 or more.



## History
2018.09.17 English readme add. 
2017.07.11 clone option add. 
2017.07.10 release. 


<a name="ja"></a>

## 日本語の解説

要素を無限スクロールさせるjQueryプラグインです。
CSS3 Animationを使用しているため、滑らかです。

### 対応ブラウザ
Flexboxと@keyframeによるアニメーションを使用しているため、IE10以上、Android4.4以上です。

## デモ
<http://wood-roots.com/sample/infiniteslidev2/>

## ブログ記事
<http://wood-roots.com/?p=1975>


## 使い方

	<script src="https://code.jquery.com/jquery-1.12.4.min.js"></script>
	<script src="infiniteslidev2.js"></script>
	<!--
	jsDelivrから読み込む場合は下記のように記述してください。
	<script src="https://cdn.jsdelivr.net/npm/infiniteslidev2/infiniteslidev2.min.js"></script>
	-->

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
2018.09.17 英語のreadmeを作成（なお作者の英語力は…） 
2017.07.11 cloneオプションの追加。 
2017.07.10 初版公開 