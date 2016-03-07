# gitbook-starter-docker

[GitBook](https://www.gitbook.com/)の[スターターキット](https://github.com/azu/gitbook-starter-kit)を`Docker`で使えるようにしました。

## 前提条件/準備

* Docker + Docker Compose

[Docker Toolbox](https://www.docker.com/products/docker-toolbox)をインストールしておくのがオススメです。

## インストール

GitBookを使った書籍を以下のようにするだけで書き始めることができます。

```
git clone --recursive  https://github.com/yamamoto-febc/gitbook-starter-docker.git  your-book-name
cd your-book-name
```

## 使い方

    docker-compose up -d gitbook

GitBookのローカルサーバが立ち上がり、 http://DockerホストのIP:4000/ にアクセスすることでプレビューできます。

    docker-compose run build

単純にビルドだけをしたい場合は、`docker-compose run build`で行うことができます。
(`_book/`にHTMLファイルが生成されます。)

### 文章を追加する

詳細は[スターターキット](https://github.com/azu/gitbook-starter-kit)を参照ください。

## テスト


    docker-compose run test

詳細は[スターターキット](https://github.com/azu/gitbook-starter-kit)を参照ください。


## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

MIT
