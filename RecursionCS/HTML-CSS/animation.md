# CSS アニメーション

CSS では、ある状態から次の状態へアニメーションを追加できる。
よく出てくるプロパティ

- transform
- Keyframe
- animation

## translate

- transform-translate 　 → 　要素を X 方向、Y 方向に移動できる
- transform-rotate 　 → 　要素を回転可能
- tranform-Scale 　 → 　要素を拡大できる
- tranform-oringin 　 → 　追記することで要素の起点を変更可能

一定時間で変化するアニメーションは transition プロパティを使用する

## keyframe と animation

より細かいアニメーションの実装に使う

keyframe は以下のように記述

```CSS
@keyframe Animation Name {
0% {...}
100% {...}
}
```

- @keyframe では、任意の名前を決めることができ、それを後述する animation プロパティでコントロールすることができる。
- また 0% はアニメーションの開始時を示しており、100% はアニメーションの終了時を意味します。

例：6 秒間で四角い緑の要素が、赤い丸に変化し、ピンクの四角になるアニメーションを実装

```HTML
<div class="box">
</div>
```

```CSS
.box {
   width: 100px;
   height: 100px;
   background-color: yellowgreen;

   /*  keyframe内のアニメーションを呼び出し、6秒間で変化させる */
   animation: box-animation 6s;
}

/*  @keyframesの横でアニメーションの名前を指定 */
@keyframes  box-animation {
   0% {
      background-color: yellowgreen;
   }
   50% {
      background-color: salmon;
      border-radius: 50%;
   }
   100% {
      background-color: pink;
   }
}
```
