.event　イベント全体{
    width: 100vw; 🟥サイトの横幅を画面幅100%に設定
    position: absolute;
    top:1000px;
    display: block
}
.event-up　イベントの上半分{
    display: flex;
    justify-content: center;
    flex-direction:column;🟥並ぶ方向を縦に
    margin: auto;🟥外側の余白を左右均等につけることで、要素を真ん中におく
}
.event-title　イベントの大文字タイトル{
    display: flex;
    justify-content: center;
    font-family: Noto Sans JP; 🟥フォントの種類をNoto Sans JPに設定
    font-weight: 700; 🟥フォントの太さを700に設定
    font-style: Bold; 🔵フォントを太字に設定
    font-size: 36px; 🟥フォントの大きさを36pxに設定
    line-height: 150%; 🟥行の高さを文字サイズの1.5倍に
    letter-spacing: 5%; 🟥文字と文字の間を、文字サイズの5%分あける
    text-align: center; 🟥子要素（今回は文字）を横方向における真ん中に置く
}
.event-subtitle　イベントの小文字タイトル{
    display: flex;
    justify-content: center;
    font-family: Plus Jakarta Sans;
    font-weight: 700; 🟥フォントの太さを700に設定
    font-style: Bold; 🔵フォントを太字に設定
    font-size: 14px; 🟥フォントの大きさを14pxに設定
    line-height: 150%; 🟥行の高さを文字サイズの1.5倍に
    letter-spacing: 10%; 🟥文字と文字の間を、文字サイズの10%分あける
    text-align: center; 🟥子要素（今回は文字）を横方向における真ん中に置く
    color:#0071BC; 🟥文字の色を青色に設定
}
.event-text　イベントの文章{
    display: block;
    text-align: center; 🟥子要素（今回は文字）を横方向における真ん中に置く
}
.event-down　イベントの下半分{
    width: 100%; 🟥サイトの横幅を画面幅100%に設定
}
.event-list　イベントのカードリストの全体{
    margin:0;
    padding:0;

    display:grid;⭐グリッド機能でレイアウトするように設定
    grid-template-columns:repeat(auto-fit, minmax(240px, 1fr));
    ⭐「カードの最小サイズを240pxに保ちながら、残っているスペースを、他のカードと同じ比率で分ける。
    ＋画面幅に合わせて列数を自動調整する設定」
    gap:28px;🟥子要素すべてに28pxの余白をつける

}
.event-item　カード一枚の全体{
    list-style: none;
    width: 100%; 🟥サイトの横幅を画面幅100%に設定
    height: auto;
    background-color:#F7F9FB; 🟥背景色を淡いグレーに設定
    border-radius:16px; 🟥角を16px丸めてカード状にする
}
.event-img　カードの画像{
    border-top-right-radius:16px; 🟥右上の角を16px丸める
    border-top-left-radius:16px ; 🟥左上の角を16px丸める
    display:block;
    width:100%; 🟥横幅を100%に設定
    height:auto;
    object-fit:cover; 🟥画像を要素全体を覆うようにトリミング
}
.event-date　カードの日付{
    background-color: #0071BC; 🟥背景色を青に設定
    color: #eeeeee; 🟥文字色を白に設定
    border-radius: 16px; 🟥角を16px丸める
    margin: auto;
    margin-top: 20px;
    width: 40%;
}
