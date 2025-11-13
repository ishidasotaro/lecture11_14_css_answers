footer{
position: absolute; サイト上での位置を動かせるようにする
bottom: 30px;　下から30pxの位置に置く
width: 100vw;  横幅を画面幅からみて100%の大きさにする
}
.footer-logo{
    display: flex;　横並びにする　フレックス要素にする
    justify-content: center;　横方向で中央ぞろえ
}
.footer-link{
    color: gray;　文字の色をグレーに
    text-decoration: none;　テキストのデザインをリセットする
    display: flex;　　フレックス要素にする
    justify-content: center;　真ん中におく
    margin-top: 12px;　上方向に余白を12pxおく
}
.footer-icon-list{
    list-style: none;　もともとのリストスタイルをリセットする
    display: flex;　　フレックス要素にする
    justify-content: center;　真ん中におく
}
.footer-icon-item{
    list-style: none;　リストのスタイルをリセットする
    width:65%;　横幅をサイトの65%の大きさで設定する
}
small{
    display: flex;　フレックス要素にする
    justify-content:center ;　真ん中におく（display flexとセット！）
    color: gray; 文字の色をグレーにする
}
.copy{
    border-top: solid;　要素の上側に実線を引く
    border-color: #eeeeee;　線の色をライトグレーにする
    padding:20px;　内側の余白を20px追加

}