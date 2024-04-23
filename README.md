## What is it about?

個人作業用のgitignore template

## Usage

任意のディレクトリにrespoitoryをcloneする

```zsh
% git clone https://github.com/RyoNakagami/ryonak_gitignore.git <arbitrary-path>
```

interactive shellに対して, `<arbitrary-path>/script` PATHを通す

```zsh
% export PATH="<arbitrary-path>/script:$PATH"' >> ~/.zshrc
```

templateに従った`.gitignore` fileを生成する

```zsh
% set_gitignore <template-name without .gitignore>
```


## 設定
### bfg

bfg-cleanerの利用を想定して以下の２つを`.gitignore`に記載している

- `..bfg-report`: bfg実行ログフォルダ
- `bfg_check_list/`: bfgの削除対象ないし置換文字列txt fileを格納する場所
