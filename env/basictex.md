# MacでBasicTeX使うやつ

なんかMacTeX無駄じゃねって人へ

## homebrew入れよう

```sh
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew update
$ brew upgrade
```

## 必要なものを入れよう

なんだかんだ使うやつ

```sh
brew install ghostscript
brew install imagemagick
```

モノ

```sh
brew tap caskroom/cask
brew install brew-cask
brew cask install basictex
brew cask cleanup
```

## 日本語使うでしょ？

この文章を読んでいる人は多分日本語使うので日本語を使う。

```sh
sudo tlmgr update --self --all
sudo tlmgr install collection-langjapanese
```

フォント設定する

これを見るのだポッター！

- [すごいサイト](http://qiita.com/yyamnk/items/2da2791bcee82643984f#%E6%97%A5%E6%9C%AC%E8%AA%9E%E7%92%B0%E5%A2%83%E3%82%92%E6%95%B4%E3%81%88%E3%82%8B)


## 入れとけってやつ

もひひ

```sh
sudo tlmgr install latexmk
```

## パッケージがねえってなる

`tlmgr`を使うのじゃ
