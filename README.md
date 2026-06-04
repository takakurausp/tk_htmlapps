# HTML Apps Collection

日常のちょっとした作業や野外調査、日々のタスクを便利にする、インストール不要・サーバー不要の軽量シングルファイルHTMLアプリのコレクションです。

すべてのアプリは **GitHub Pages** で公開されており、スマートフォンやPCのブラウザからすぐにアクセスして利用できます。

👉 [**公開ページ（GitHub Pages）でアプリ一覧を見る**](https://takakurausp.github.io/tk_htmlapps/ "null")

## 🚀 収録アプリ一覧

### 1. 🧭 野外調査メモ (Field Work Pad) [起動](https://takakurausp.github.io/tk_htmlapps/fw_pad.html)

野外調査やフィールドワークでの記録に特化した、スマートフォン用のデータロガーです。

*   **特徴**:
    
    *   メモを入力し始めるとバックグラウンドで高精度GPS（緯度・経度・高度・精度）を自動取得。
        
    *   電波の届かない山奥や僻地でも動作し、データは端末内（localStorage）に自動保存。
        
    *   記録した地点を即座に簡易マップ（Leaflet）にプロット。
        
    *   Excelでそのまま開ける「BOM付きUTF-8」のCSVエクスポート、およびJSONエクスポートに対応。
        
*   **ファイル名**: `fw_pad.html`
    
### 2. 🔎 野外調査メモのビューワー (Field Work Pad Viewer) [起動](https://takakurausp.github.io/tk_htmlapps/fwp-viewer.html)

上記野外調査メモアプリで作成したデータの簡易ビューワーです。

*   **特徴**:
    
    *   記録地点を地図上にピンで表示し、ピンのタップで詳細をバルーン表示します。
        
    *   数値に変換できるメモについては、色と数字であらわします。
        
*   **ファイル名**: `fwp-viewer.html`
  
### 3. 📷 電気泳動ゲル撮影システム (Electrophoresis Gel Document System) [起動](https://takakurausp.github.io/tk_htmlapps/optigelh.html)

電気泳動ゲルを美しく正しく撮影し、記録をとるためのシステムです。

*   **特徴**:
    
    *   染色液に応じてRまたはGのチャンネルを抜き出して記録することができます。
        
    *   バックグラウンドノイズを除去するデヘイズ処理を行います。具体的には一定以下の輝度を差し引いています。

    *   バンドの輝度をリニアに持ち上げるコントラスト処理も備えています。

    *   10枚までのスタッキング撮影に対応。これによりノイズを平均化し、美しいゲル画像を得ることができます。

    *   画像は、圧縮による劣化がないPNGで保存します。撮影パラメータはメタデータに書き込んでいますので、ビューアーなどで確認することができます。

*   **ファイル名**: `optigelh.html`
  
## 🛠 特徴と設計思想

*   **1ファイル完結 (Single File App)**: 全てのHTML、CSS (Tailwind CSS)、JavaScriptが1つのファイルに統合されています。ダウンロードしてダブルクリックするだけでローカル環境でも動きます。
    
*   **オフラインファースト (Offline Ready)**: インターネット接続が不安定な場所でも動作し、データはブラウザの `localStorage` に保存されるため、ページを閉じてもデータが消えません。
    
*   **レスポンシブデザイン (Mobile Friendly)**: スマートフォンによる片手での操作から、PCでの大画面操作までシームレスに対応します。
    
*   **安心のデータプライバシー**: データを外部のサーバーに送信せず、すべてお使いのブラウザ内部で処理・完結します。
    

## 💻 使い方（ローカル実行）

本リポジトリのアプリは、ローカル環境に保存して直接実行することも可能です。

1.  リポジトリをクローンするか、必要な `.html` ファイルをダウンロードします。
    
    ```
    git clone https://github.com/takakurausp/tk_htmlapps.git
    ```
    
2.  ダウンロードした `.html` ファイルをブラウザ（Chrome, Safari, Firefoxなど）でダブルクリックして開きます。
    

> **⚠️ 注意（GPSなどの位置情報機能について）** ブラウザのセキュリティ仕様により、位置情報（GPS）を使用するアプリは **HTTPS接続**（またはローカル開発環境の `localhost`）でのみ正常に動作します。スマートフォンでGPS機能を使用する場合は、GitHub Pages（https）経由でのアクセスを推奨します。

## 📄 ライセンス (License)

このプロジェクトは **MITライセンス** のもとで公開されています。商用利用、改変、配布、個人利用など、どなたでも自由にご利用いただけます。

```
Copyright (c) 2026 Koh-ichi Takakura

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 👤 開発者 (Author)

*   **Koh-ichi Takakura**
    
*   GitHub: [@takakurausp](https://github.com/takakurausp "null")
