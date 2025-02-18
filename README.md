# android-app-builder

下記の番号の内容に沿ってアンドロイド向けアプリを作成して欲しい

1.　最初のページに縦並びのボタンを、ディベロッパー情報、空き室状況、想定賃貸算出の項目で作成
2.　「ディベロッパー」画面では「追加」ボタンを追加
2.2.　「追加」ボタンをおしたら「名前」と「リンク」の入力欄と「確定」と「キャンセル」ボタンを表示
2.3.　「確定」ボタンを押したら「名前」の値をボタン名にする
2.4.　「キャンセル」ボタンを押したら「ディベロッパー」画面に戻る
2.5.　追加されたボタンは「リンク」に入力したWebsiteのページを表示
2.6.　画面左上に「戻る」ボタンを追加して押したらホーム画面に戻って
2.7.　追加されたボタンの隣に「×」ボタンを追加
2.8.　「×」ボタンを押したら隣のボタンを削除

3.　「空き室状況」の画面では下記の内容で構成して
3.1　「追加」ボタンを追加
3.2　「追加」ボタンをおしたら「名前」と「リンク」の入力欄と「確定」と「キャンセル」ボタンを表示
3.3　「確定」ボタンを押したら入力した「名前」の値をボタン名にする
3.4.　「キャンセル」ボタンを押したら空き室状況の画面に戻る
3.5.　追加されたボタンは「リンク」に入力したWebsiteのページを表示
3.6.　画面左上に「戻る」ボタンを追加して押したらホーム画面に戻って
3.7.　追加されたボタンの隣に「×」ボタンを追加
3.8.　「×」ボタンを押したら隣のボタンを削除

4.　「想定賃貸算出」画面は下記の内容で構成して
4.1　次の項目を追加
購入価格/竣工時価格
面積
平米単価	
竣工残り年数
竣工
周辺地価上昇率/年
想定竣工時価格
想定平米単価
周辺平均年間利回り
1br
2br
3br
想定年間総利益
純賃貸価格	
組合費/月
最低
最大
最終賃貸価格
4.2　「購入価格/竣工時価格」、「平米単価」、「想定竣工時価格」、「想定平米単価」、「想定平米単価」、「想定年間総利益」、「純賃貸価格」、「組合費/月」、「最低」、「最大」、「最終賃貸価格」の項目はPHP金額となるため入力された値には「₱」と3桁毎に「,」を追加
4.3　「平米単価」は「購入価格/竣工時価格」の値を「面積」の値で割った値
4.4　インターネット上からフィリピン首都圏の1年でのコンドミニアムの平均価格上昇率を取得。取得ができない場合は「6.45％」の値を表示
4.5　「想定竣工時価格」は「購入価格/竣工時価格」に「周辺地価上昇率/年」の値を掛け算した値で掛け算をする
4.6「周辺平均年間利回り」は「1br」、「2br」、「3br」の平均率を表示し、該当がなければ「5.04%」と表示する
4.7　「想定年間総利益」は「想定竣工時価格」に値があればその値で掛け算、空白の場合は「購入価格/竣工時価格」の値で掛け算
4.8　「想定年間総利益」の値を12で割る
4.9　「組合費/月」は「最低」と「最大」の平均値
4.10　「最終賃貸価格」は「想定年間総利益」と「組合費/月」を足した値
4.11　「竣工残り年数」に値が無い場合は「周辺地価上昇率/年」と「想定竣工時価格」と「想定平米単価」は入力できない状態にするが、「竣工残り年数」に値を入力すれば周辺地価上昇率/年」と「想定竣工時価格」と「想定平米単価」は入力できるようになる

## Collaborate with GPT Engineer

This is a [gptengineer.app](https://gptengineer.app)-synced repository 🌟🤖

Changes made via gptengineer.app will be committed to this repo.

If you clone this repo and push changes, you will have them reflected in the GPT Engineer UI.

## Tech stack

This project is built with React with shadcn-ui and Tailwind CSS.

- Vite
- React
- shadcn-ui
- Tailwind CSS

## Setup

```sh
git clone https://github.com/GPT-Engineer-App/android-app-builder.git
cd android-app-builder
npm i
```

```sh
npm run dev
```

This will run a dev server with auto reloading and an instant preview.

## Requirements

- Node.js & npm - [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)
