# Azure OpenAI Responses API Sample

## 初期設定

### git clone を実行
```
git clone https://github.com/tsukashusan/aoai-responses-api-sample.git
```
### Python 仮想環境をアクティベート
virtualenv -p 3.11 .venv

1. `_env`ファイルにある、`AZURE_OPENAI_ENDPOINT`と`TARGET_FILE_PATH`と`MODEL_NAME`を設定</br>
![CREATE_ENV](./docs/images/create-env-file.png "サンプル")

1. `_env`ファイルのコピーし、`.env`ファイルとする</br>
![RENAME_ENV](./docs/images/copy-dot-env-file.png "サンプル")

![RENAME_ENV](./docs/images/dot-env.png "サンプル")

1. コマンドプロンプトで以下のコマンドを実行</br>
```posershell
pip install -r requirements.txt
```

## プログラムの実行

`aoai-responses-sample.ipynb`をバッチ実行する

```
papermill aoai-responses-sample.ipynb execute.ipynb --request-save-on-cell-execute --prepare-execute 
```