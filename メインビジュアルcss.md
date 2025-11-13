header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    top: 0;
    right: 0;
    left: 0;
    border-bottom: solid; 🟥ここまでは変更なし

    background-color: white;🟥背景色を白に設定

    z-index: 1000;🟥高さを「1000」に設定
}

body{
    height: 5000px; 🟥サイトの縦幅を5000pxまで拡張
    position: relative;　🟥position:absoluteで動く要素の基準に設定
    width: 100vw; 　🔵サイトの横幅を画面幅100%に設定

}
main　メインビジュアルの親要素{
    width: 100vw;　🔵サイトの横幅を画面幅100%に設定
}
.mainvisual　メインビジュアル（背景付き）{
    z-index: 0;　          🟥高さを「0」に設定
    position: absolute;　🟥「relative」を設定したbodyを基準に動けるようにする
    top: 0px;　           🔵上から0pxの位置に置く
    left: 0px;　          🔵左から0pxの位置に置く
    width: 100vw;　       🔵サイトの横幅を画面幅100%に設定
    height: 900px;　      🟥高さを900pxにする
    background-image: url(../img/bg-mainvisual.jpg);　🟥背景にbg-mainvisual.jpgを設定
    background-position-x: center;　🟥背景の位置をX軸方向における真ん中におく
    background-size: cover;　🟥背景が要素全体を覆うように設定
    background-repeat: none; 🟥背景を繰り返して置く設定を無効にする
}
.main-text　メインビジュアルの文字の親要素{
    position: absolute;　🔵「relative」を設定したbodyを基準に動けるようにする
    top: 600px ;　🟥上から600pxの位置に置く
    left: 10%;　🟥「bodyの横幅の10%分」左の位置に置く
}
.main-subtitle　メインビジュアルの文字のうち、小さいほう{
    background-color: #eeeeee;　🔵背景色を白に設定
    color: #0071BC;　🟥文字の色を青色(?)に設定する
    font-family: Noto Sans JP;　🟥フォントの種類をNoto Sans JPに設定
    font-weight: 700;　🟥フォントの太さを700に設定
    font-style: Bold;　🔵フォントを太字に設定
    font-size: 24px;　 🟥フォントの大きさを24pxに設定
    line-height: 180%; 🟥行の高さを文字サイズの1.8倍に
    letter-spacing: 5%;🟥文字と文字の間を、文字サイズの5%分あける
    text-align: center;🟥子要素（今回は文字）を横方向における真ん中に置く 
}
.main-title　メインビジュアルの文字のうち、大きいほう{
    background-color: #eeeeee;　🔵背景色を白に設定
    font-family: Noto Sans JP;　🔵フォントの種類をNoto Sans JPに設定
    font-weight: 700;　🔵フォントの太さを700に設定
    font-style: Bold;　🔵フォントを太字に設定
    font-size: 60px;　 🟥フォントの大きさを60pxに変更
    line-height: 180%; 🔵行の高さを文字サイズの1.8倍に
    letter-spacing: 5%;🔵文字と文字の間を文字サイズの5%分あける
}
.scroll-text　「scrolldown」の文字{
    position: absolute;　🔵「relative」を設定したbodyを基準に動けるようにする
    top:820px; 🟥上から820pxの位置に置く
    right:2%;　🟥bodyの横幅の2％だけ右に動く
    color:white;🟥文字の色を白色にする
    font-weight: bold;🟥フォントの太さを最大に設定
}
.scroll-text::before　「scroll-text」の　前に　要素を追加{
    content:"";　🟥htmlの中身を設定（中身は空だが、存在はする）
    background-color: white;🟥背景色を白色にする
    border-radius: 50%;　🟥完全な円形にする
    width: 15px;　🟥横幅を15pxに
    height: 15px; 🟥縦幅を15pxに
    position: absolute;🟥「scroll-text」を基準に動けるようにする
    transform: translate(-20px,5px);🟥X軸方向(右方向)において20px左に動く＆下方向に5px動く
}
