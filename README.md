# GSAP Auto Slider
GSAPを利用した横スクロールの自動スライダーです。

#### デモ
https://codepen.io/sakata-kazuma/details/yLPEbWL

　  

### 使い方
#### CSS読み込み
```
<link rel="stylesheet" href="file-path/auto-slider.min.css">
```
  

#### JS読み込み
```
<script src="file-path/auto-slider.min.js"></script>
```

#### HTMLにレイアウトコードを追加
```
<div class="js-auto-slider-wrap">
  <div class="js-auto-slider-inner">
    <div class="js-auto-slider" id="js-auto-slider">
      <div class="js-auto-slider-elm">
        <div class="js-auto-slider-img">
          <img src="https://picsum.photos/id/101/1740/720" alt="" class="ob-fit-cover posi-full-img">
        </div>
      </div>
      <div class="js-auto-slider-elm">
        <div class="js-auto-slider-img">
          <img src="https://picsum.photos/id/1015/1740/720" alt="" class="ob-fit-cover posi-full-img">
        </div>
      </div>
      <div class="js-auto-slider-elm">
        <div class="js-auto-slider-img">
          <img src="https://picsum.photos/id/109/1740/720" alt="" class="ob-fit-cover posi-full-img">
        </div>
      </div>
      <div class="js-auto-slider-elm">
        <div class="js-auto-slider-img">
          <img src="https://picsum.photos/id/110/1740/720" alt="" class="ob-fit-cover posi-full-img">
        </div>
      </div>
    </div>
  </div>
</div>
```

#### スライダー呼び出し
```
autoSlider({
  target: '#js-auto-slider'
});
```

　  


### オプション
#### ・ページャー追加
##### 任意の場所にページャー用HTMLを追加
```
<ul class="js-auto-slider-pager" id="js-auto-slider-pager"></ul>
```

##### スライダー呼び出しコードにページャーオプションを追加
```
autoSlider({
  target: '#js-auto-slider',
  pager: '#js-auto-slider-pager'
});
```

　  

#### ・その他オプション
```
autoSlider({
  target: null,  //スライダー ターゲット設定
  activeClass: 'is-active',  //スライダー要素 active class
  slideElm: 'js-auto-slider-elm',  //スライダー要素 class
  slideElmClone: 'js-auto-slider-elm-clone',  //スライダー複製要素 class
  slideChildImg: 'js-auto-slider-img',  //スライダー画像要素 class
  activeIndex: 0,  //開始するスライド番号
  scrollTimeBefore: 5,  //前半スクロール時間
  scrollTimeAfter: 0.6,  //後半スクロール時間
  scrollSpeedBefore: 30,  //前半スクロール量
  scrollRatioBefore: 0.4,  //前半スクロール量
  easing: Power1.easeOut,  //後半スクロール GSAPイージング
  pager: null, //スライダーページャー ターゲット設定
  pagerBusy: 'is-busy', //スライダーページャー スライド動作中判別 class
  pagerElm: 'js-auto-slider-pager-elm', //スライダーページャー要素 class
  pagerBtn: 'js-auto-slider-pager-btn', //スライダーページャー要素内 button要素 class
  pagerText: null, //スライダーページャー要素内 button要素に格納するテキスト（デフォルトは index番号が入ります）
  pagerActiveClass: 'is-active', //スライダーページャー要素・button要素 active class
});
```

### 動作環境
Internet Explorer 11  
Google Chrome 最新版  
Firefox 最新版  
Safari 最新版
