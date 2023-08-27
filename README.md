### オーディオサンプリングレート変換ツール ユーザーガイド

---

#### 1. 事前準備

- このツールはPython 3で動作します。Python 3がインストールされていない場合は、公式サイトからダウンロードしてインストールしてください。[Python公式サイト](https://www.python.org/downloads/)

- また、このツールはオーディオファイルの読み取りと書き込みに`ffmpeg`を使用する場合があります。`ffmpeg`がインストールされていない場合は、[公式サイト](https://ffmpeg.org/download.html) からダウンロードしてインストールしてください。

---

#### 2. 必要ライブラリのインストール

- 次のコマンドを使用して、必要なPythonライブラリをインストールします。

  ```
  pip install gradio soundfile numpy resampy pydub
  ```

---

#### 3. オーディオサンプリングレート変換ツールの使用方法

1. ツールのPythonスクリプト(`exchange_sampling_rate.py`など)をダウンロードまたはクローンします。
   
2. コマンドプロンプトまたはターミナルを開き、スクリプトが保存されているディレクトリに移動します。

   例: 
   ```
   cd path/to/directory
   ```

3. 次のコマンドを実行して、ツールを起動します。

   ```
   python exchange_sampling_rate.py
   ```

4. ブラウザが自動的に開かず、`Running on local URL: http://127.0.0.1:xxxx` というメッセージが表示された場合、ブラウザを手動で開き、表示されたURLを入力してアクセスしてください。

5. インターフェース上で、変換したいオーディオファイルが保存されているディレクトリのパスを入力します。

6. ターゲットとなるサンプリングレートをドロップダウンメニューから選択します。

7. "送信" ボタンをクリックすると、指定したディレクトリ内のオーディオファイルのサンプリングレートが選択したレートに変換され、元のディレクトリに`resampled_`というプレフィックスを持つファイル名で保存されます。

---

#### 4. トラブルシューティング

- もし、MP3ファイルの読み取りや書き込みに問題が発生した場合は、`ffmpeg`が正しくインストールされているかを確認してください。

- 何らかのエラーメッセージが表示された場合は、そのエラーメッセージをメモして、サポートにお問い合わせください。


### Audio Sampling Rate Conversion Tool User Guide

---

#### 1. Prerequisites

- This tool operates on Python 3. If you haven't installed Python 3, download and install it from the official website: [Python Official Site](https://www.python.org/downloads/).

- The tool might utilize `ffmpeg` for reading and writing audio files. If you don't have `ffmpeg` installed, download and set it up from the [Official Site](https://ffmpeg.org/download.html).

---

#### 2. Installing Required Libraries

- Use the following command to install the necessary Python libraries:

  ```
  pip install gradio soundfile numpy resampy pydub
  ```

---

#### 3. How to Use the Audio Sampling Rate Conversion Tool

1. Download or clone the Python script for the tool (e.g., `exchange_sampling_rate.py`).
   
2. Open your command prompt or terminal and navigate to the directory where the script is saved.

   Example: 
   ```
   cd path/to/directory
   ```

3. Run the following command to launch the tool:

   ```
   python exchange_sampling_rate.py
   ```

4. If the browser doesn't open automatically and you see a message like `Running on local URL: http://127.0.0.1:xxxx`, manually open your browser and input the provided URL to access the tool.

5. On the interface, input the directory path where the audio files you wish to convert are stored.

6. Choose the desired target sampling rate from the dropdown menu.

7. Click on the "Submit" button. The audio files in the provided directory will be converted to the chosen sampling rate and saved back in the original directory with a `resampled_` prefix in their filename.

---

#### 4. Troubleshooting

- If you encounter issues with reading or writing MP3 files, ensure `ffmpeg` is correctly installed.

- If any error messages appear, take note of them and contact support for further assistance.
