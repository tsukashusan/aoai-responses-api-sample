# Azure OpenAI Responses API Sample

## 初期設定

### git clone を実行
```
git clone https://github.com/tsukashusan/aoai-responses-api-sample.git
```

### `_env`ファイルにある、`AZURE_OPENAI_ENDPOINT`と`TARGET_FILE_PATH`と`MODEL_NAME`を設定</br>
![CREATE_ENV](./docs/images/create-env-file.png "サンプル")

### `_env`ファイルのコピーし、`.env`ファイルとする</br>
![RENAME_ENV](./docs/images/copy-dot-env-file-1.png "サンプル")

![RENAME_ENV](./docs/images/copy-dot-env-file-2.png "サンプル")

### コマンドプロンプトで以下のコマンドを実行</br>
```posershell
pip install -r requirements.txt
```

## プログラムの実行

### az login の実行

> [!CAUTION]
> az cli が入っていない場合は次のサイトからダウンロード、インストール</br>
> https://learn.microsoft.com/ja-jp/cli/azure/install-azure-cli?view=azure-cli-latest

```
az login --tenant <tenant id>
```


### `aoai-responses-sample.ipynb`をバッチ実行する
```
papermill aoai-responses-sample.ipynb execute.ipynb --request-save-on-cell-execute --prepare-execute 
```

### Notebook 形式で インタラクティブに実行する
インタラクティブに実行する場合は、VSCodeなどで`aoai-responses-sample.ipynb`ファイルを開き適宜実行してください。
![RENAME_ENV](./docs/images/interactive.png "サンプル")


> [!CAUTION]
> 「`aoai-responses-sample.ipynb`をバッチ実行する」と「Notebook 形式で インタラクティブに実行する」はいずれかの実行です。両方実施する必要はありません。


### システムプロンプト、ユーザプロンプトの書き換え

`aoai-responses-sample.ipynb`の`10行目`, `14行目`の```の記号で括られたエリアを書き換えて実行してください。

![RENAME_ENV](./docs/images/copy-dot-env-file-2.png "サンプル")
