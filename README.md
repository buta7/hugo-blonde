# README

## セットアップ

サイト作成

```shell
hugo new site hugo-blonde
```

レポジトリ初期化

```shell
cd hugo-blonde
git init
echo '*~' >> .gitignore
echo '*.bak' >> .gitignore
echo '*.orig' >> .gitignore
echo '.env' >> .gitignore
echo 'public' >> .gitignore
echo 'resources' >> .gitignore
```

テーマ設定(submoduleはhttpsプロトコルで追加)

```shell
git submodule add https://github.com/opera7133/Blonde.git themes/blonde
```

(参考)submoduleの削除

```shell
git submodule deinit -f themes/blonde
git rm themes/blonde
rm -fr .git/modules/blonde
```

サイト設定

```shell
cp -p themes/blonde/exampleSite/{config.toml .
cp -pr themes/blonde/exampleSite/{content,data} .
```

Node.jsパッケージのインストール

```shell
npm i
```

## Link

* [Blonde \| Hugo Themes](https://themes.gohugo.io/blonde/)
