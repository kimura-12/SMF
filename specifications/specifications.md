# SMF(Stock Managed reFrigerator)の仕様書  

### 1.システムの目的  
本システムの目的は，冷蔵庫にある食材の種類と賞味期限を一元で管理して、賞味期限切れで無駄になる食材を減らす，多重で購入することを減らすことである．  
これまで一人暮らしでは，自炊はするものの頻度は多くなく，余っている食材を忘れてしまい，賞味期限が切れてしまったり，買い物の際に同じものを買ってしまう，といったことがよくあった．特に，調味料などの賞味期限の長いものの存在は忘れてしまいがちであり，無駄にしてしまうことが多い．  
そこで，冷蔵庫の食材管理を行うシステムをスマートフォンのアプリケーションとして実装し，ユーザーが自身のスマートフォンから，買い物先など，どこからでも，冷蔵庫にある食材の種類と数，賞味期限を確認，変更できるようにする．また，賞味期限が近づいている食材の通知をする機能も提供する．本システムの導入により，ユーザーは賞味期限切れや多重購入などによる食材のロスを削減することができ，さらに買い物の際に必要なものを考える負担を軽減することができる．  
  
### 2. システムの概要  
本システムは，冷蔵庫内の食材の種類，数量，購入日からの賞味期限を一元管理し．賞味期限が近づくとユーザーに通知するスマートフォンのアプリケーションとして構築する．  
![/Figure1.PNG](https://github.com/Keeper-Harry/Trump/blob/master/SMF/Figure1.PNG "図(1)")  
<div style="text-align: center;">
図(1) : システム導入前の現状  
</div>
  
  
これまでの現状は図⑴のように，ユーザーが記憶している範囲で冷蔵庫内の在庫を管理していた．そのため在庫にある食材と必要な食材の管理ができずに多重で購入してしまうことや，賞味期限が切れてしまい廃棄してしまうことが起こっていた.  
![/Figure2.PNG](https://github.com/Keeper-Harry/Trump/blob/master/SMF/Figure2.PNG "図(2)")  
<div style="text-align: center;">
図(2) : システム導入による効果  
</div>
  
  
図⑵はシステム導入後のあるべき姿である．スーパーなどで食材の購入時にスマートフォンで，在庫を確認でき，購入商品を登録する．使用したり廃棄した時に削除することができる．また賞味期限が近づくとスマートフォン上で通知することに加え，登録履歴も蓄積され，その食材の賞味期限予測も可能である．  
  
### 3.機能一覧  
- (1) 食材管理機能    
   ユーザーが食材を登録,確認，更新，削除する機能．管理する情報は食材の種類・賞味期限・在庫状況・登録日・使用日である．食材の在庫状況としては個数，グラム数が選択可能である．
- (2) 賞味期限通知機能  
   冷蔵庫内の食品の賞味期限が近づくと，ユーザーのスマートフォンに通知を行う機能である．
- (3) 賞味期限予測機能  
   過去に登録されたデータより賞味期限を予測し，ユーザーの賞味期限登録の負担を減らす．  