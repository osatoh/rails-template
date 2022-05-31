# devcontainer for Ruby on Rails 7.0 + tailwind + rspec

Ruby on Rails 7.0 の開発環境用の [devcontainer](https://code.visualstudio.com/docs/remote/containers)

## 構成

docker compose で構成

- app: [ruby:3.1.2](https://hub.docker.com/_/ruby)
- postgres: [postgres:14](https://hub.docker.com/_/postgres)

### 機能

- formatter:
  - Ruby: [rufo](https://github.com/ruby-formatter/rufo)
  - ERB: [erb-formatter](https://github.com/nebulab/erb-formatter)
  - HTML, CSS, JS: [Prettier](https://prettier.io/)
- Intellisense: [solargraph](https://github.com/castwide/solargraph)

## devcontainer の利用方法

※ devcontainer に必要なツールのインストールは[こちら](https://code.visualstudio.com/docs/remote/containers#_installation)

### このリポジトリを新規プロジェクトで利用する場合

1. VSCode を開き、 `Reopen in Container` を実行す

### 既存のプロジェクトで利用する場合

1. このリポジトリをダウンロードし、任意のプロジェクトに以下をコピーする

- [docker-compose.yml](docker-compose.yml)
- [docker/app/Dockerfile](docker/app/Dockerfile)
- [.devcontainer](.devcontainer)
- [.vscode](.vscode)

2. VSCode を開き、 `Reopen in Container` を実行する

## サーバーの立ち上げ方

#### devcontainer 上で、コマンドを実行する

```bash
$ dev
```

## docker compose のみで実行する場合

VSCode 以外の環境で開発する場合は、docker compose を利用することができる。 [Makefile](Makefile) コマンドが用意されている。各コマンドは Host OS 上で実行する。

#### 初回構築

```
$ make build
```

#### サーバーを起動する

```
$ make serve
```

## VSCode extensions

- [rebornix.Ruby](https://marketplace.visualstudio.com/items?itemName=rebornix.Ruby)
- [castwide.solargraph](https://marketplace.visualstudio.com/items?itemName=castwide.solargraph)
- [elia.erb-formatter](https://marketplace.visualstudio.com/items?itemName=elia.erb-formatter)
- [redhat.vscode-yaml](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml)
- [jemmyw.rails-fast-nav](https://marketplace.visualstudio.com/items?itemName=jemmyw.rails-fast-nav)
- [aki77.rails-db-schema](https://marketplace.visualstudio.com/items?itemName=aki77.rails-db-schema)
- [hridoy.rails-snippets](https://marketplace.visualstudio.com/items?itemName=hridoy.rails-snippets)
- [kaiwood.endwise](https://marketplace.visualstudio.com/items?itemName=kaiwood.endwise)
- [VisualStudioExptTeam.vscodeintellicode](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)
- [esbenp.prettier-vscode](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

## リファレンス

- [Visual Studio Code Doc - Developing inside a Container](https://code.visualstudio.com/docs/remote/containers)
- [VS Code Solargraph Extension](https://github.com/castwide/vscode-solargraph)
- [vscode-ruby debugger](https://github.com/rubyide/vscode-ruby/blob/main/docs/debugger.md)
- [saboyutaka/rails\-devcontainer](https://github.com/saboyutaka/rails-devcontainer)
