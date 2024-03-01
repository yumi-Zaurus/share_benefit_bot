# share_benefit_bot

## 仮想環境の作成
作業ディレクトリで
``` python
python -m venv .venv
```

## 仮想環境への切り替え
### windows
#### PowerShell
```
.venv\Scripts\activate.ps1

deactivate
```
エラーが出たときは以下を実行
```
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser -Force
```
#### コマンドプロンプト
```
.venv\Scripts\activate.bat

deactivate
```
### Mac
```
未作成
```

## 仮想環境の共通化
### 一覧を作成
仮想環境内で
```
python -m pip freeze > requirements.txt
```
### 一覧を自分の仮想環境の取り入れる
仮想環境内で
```
python -m pip install -r requirements.txt
```