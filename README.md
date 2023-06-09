# SmartPDF
このプログラムは、OpenAIのChatGPTを使用してPDFファイルのファイル名を自動的にリネームします。指定された入力フォルダ内のPDFファイルを読み込み、その内容に基づいて適切な題名を生成し、出力フォルダにリネームされたファイルを保存します。

## 初期設定
1. Pythonパッケージをインストールします。
```
pip install -r requirements.txt
```
2. [こちら](https://github.com/tesseract-ocr/tesseract)からTesseract OCRをインストールします。
C:\Program Files\Tesseract-OCRをデフォルトで読み込みます。もし別の場所にインストールした場合は、settings.iniのtesseract_pathのパスを変更してください。
3. [こちら](https://blog.alivate.com.au/poppler-windows/)からPopplerをダウンロードし、解凍したうえでsmartPDF.pyと同一のディレクトリ直下に配置してください。もし別の場所に配置した場合は、settings.iniのpoppler_pathのパスを変更してください。
3. smartPDF.pyを実行すると「OpenAI APIキーが設定されていません。settings.iniにAPIキーを設定してください。」と表示され、settings.iniが開きます。ここでOpenAIのAPIキーを追記してください。
4. もう一度プログラムを実行すると、メインウィンドウが表示されます。ここで入力フォルダと出力フォルダを選択してください。<br>
※venvによる仮想環境を作成した場合は、smartPDF.batを実行することで仮想環境が自動的に有効化され、プログラムが実行されます。仮想環境の名前はvenvとしています。もし別の名前にした場合は、smartPDF.batを編集してください。<br>
※入力フォルダと出力フォルダは保存され、次回以降は自動的に読み込まれます。
5. 選択が完了したら、「開始」ボタンをクリックしてプロセスを開始します。入力フォルダ内のPDFファイルが読み込まれ、それぞれのファイルの内容に基づいて題名が生成され、出力フォルダにリネームされたファイルが保存されます。
6. プログラムが完了すると、リネームされたファイルのサマリがポップアップウィンドウで表示されます。

※このプログラムはWindows10でのみ動作確認を行っています。<br>
※このプログラムはChatGPTを利用して作成いたしました。