---
idx: selenium
bid: selenium
srcpath: selenium/index.md
title: Selenium
rids:
  - install
heroimgpath:
date: 2017.6.8
layout: binder.jade
---

selenium-standalone
: [vvo/selenium\-standalone ](https://github.com/vvo/selenium-standalone)

[SeleniumHQ/docker-selenium](https://github.com/SeleniumHQ/docker-selenium)
: Docker images for Selenium Standalone Server


## articles

- [selenium\-webdriverの紹介とAPI翻訳 \- Qiita](http://qiita.com/nazomikan/items/40b86dc5619bb1795aaa)
- __[Seleniumアレルギーのための処方箋 \- Qiita](http://qiita.com/cognitom/items/27b7375bea653b414c8f)__
- [\[Selenium 3\-beta\] Server fails to start when launched with chromedriver v2\.22 · Issue \#2566 · SeleniumHQ/selenium](https://github.com/SeleniumHQ/selenium/issues/2566)
> -D arguments in the command line should come before the '-jar's
- [Selenium WebDriver でMacとWindows共通に動く環境を作る（ChromeDriverをServerで） \- Qiita](http://qiita.com/kochizufan/items/905165b92c7e70986f60)
- [【Selenium】色んなブラウザを動かす（PC編） \- ネーミングセンスがない！](http://unagi-tabetai.hatenablog.com/entry/2015/05/25/125030) Java実装


## [Selenide](http://selenide.org/)
http://selenide.org/documentation.html

- [Selenide Java Library：簡単なことは簡単に，Web UI テスト自動化の敷居を下げ，生産性をあげる魔法の Wrapper \- Qiita](http://qiita.com/kazuki-ma/items/d6432fc41c82538a61bd)
- [Selenide～Javaで超簡単・簡潔にUIテストを書く～ \- Qiita](http://qiita.com/tatesuke/items/589e30ab9b3dc7037e26)
- [Java製SeleniumラッパーのSelenideを使ってみた \- Qiita](http://qiita.com/nyasba/items/6ab42fc73a912426ee5d)
- [Selenideでテストコードを書いてみた \- Qiita](http://qiita.com/nyakome/items/207daf3050809c269e8e)

### Configuration

```java
import static com.codeborne.selenide.Selenide.*;

System.setProperty( "webdriver.chrome.driver", "C:/path/to/chromedriver.exe" );
System.setProperty( "chromeoptions.args", "--headless --disable-gpu" );
Configuration.browser = WebDriverRunner.CHROME;
Configuration.browserSize = "1280x1024";
Configuration.timeout = 10000;
```

Chrome 起動オプション
: [List of Chromium Command Line Switches « Peter Beverloo](http://peter.sh/experiments/chromium-command-line-switches/)


### Frame
- [selenide/FramesTest\.java at master · codeborne/selenide](https://github.com/codeborne/selenide/blob/master/src/test/java/integration/FramesTest.java)

### `switchTo`
```
switchTo().defaultContent();

switchTo().innerFrame("parentFrame");

switchTo().innerFrame("parentFrame", "childFrame_2", "childFrame_2_1");

switchTo().frame("topFrame");

switchTo().frame(0);
```


## [WebdriverIO](http://webdriver.io/)
Selenium 2\.0 javascript bindings for nodejs  
※ __wdio__ == webdriverio

- [5 Minutes with WebdriverIO \- YouTube](https://www.youtube.com/watch?v=vPes7NKeYno)
- [WebdriverIO \- REPL interface](http://webdriver.io/guide/usage/repl.html) REPLがある
- [WebdriverIO \+ power\-assert でe2eテストをgeneratorで書いてみる \- Qiita](http://qiita.com/yoshi6jp@github/items/24d01dfc6712dbf112aa)
- [LIGブログの安全な開発のために 〜WebdriverIOでスクリーンショットを撮る編〜 \| それいけ！フロントエンド](https://liginc.co.jp/304470)
