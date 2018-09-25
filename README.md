# Brave Browser
> 개인 정보를 보호하고 및 열린 웹 생태계를 강조하는 유명한 웹브라우저는 모질라재단이 만든 ‘파이어폭스’다. 브랜든 아이크는 모질라재단의 자회사 모질라 코퍼레이션을 설립했으며, 모질라 코퍼레이션에서 약 10년간 최고 기술관리자(CTO)를 역임했던 인물이다. 1995년에 넷스케이프에 근무하던 당시는 자바스크립트를 만들기도 하였다. 하지만 브랜든 아이크 CEO는 동성결혼을 금지하는 ‘동성결혼금지 법안(California’s Proposition 8)’에 1천달러를 기부했고, 내부 직원들의 반발로 2014년 모질라재단을 떠났다. 브레이브는 여전히 모질라재단과 많은 연결고리를 가진다. 브레이브 iOS 버전은 파이어폭스 iOS를 기술 ‘포크(오픈소스 기술을 복사해 일부 수정하는 것)’해 개발한 기술이다. 브레이브 PC버전 초창기 버전은 모질라재단이 만든 ‘게코’엔진을 이용해 만들었다. 지금은 깃허브가 만든 ‘일렉트론’ 프레임워크로 교체했다. 브레이브소프트웨어 공동설립자 브레인 본디 개발자도 2011년부터 3년 동안 파이어폭스 기술 개발에 참여했다.

## Overview 

This repository holds the build tools needed to build the next generation Brave desktop browser for macOS, Windows, and Linux.  In particular, it fetches and syncs code from the projects we define in `package.json` and `src/brave/DEPS`:

  - [Chromium](https://chromium.googlesource.com/chromium/src.git)
    - Fetches code via `depot_tools`.
    - sets the branch for Chromium (ex: 65.0.3325.181).
  - [brave-core](https://github.com/brave/brave-core)
    - Mounted at `src/brave`.
    - Maintains patches for 3rd party Chromium code.
  - [brave-extension](https://github.com/brave/brave-extension)
    - Mounted at `src/brave/vendor/brave-extension`.
    - Browser action extension which implements the UI for the shields panel.
  - [ad-block](https://github.com/brave/ad-block)
    - Mounted at `src/brave/vendor/ad-block`.
    - Implements Brave's ad-block engine.
  - [tracking-protection](https://github.com/brave/tracking-protection)
    - Mounted at `src/brave/vendor/tracking-protection`.
    - Implements Brave's tracking-protection engine.
    
## Build instructions

See the [Brave Wiki](https://github.com/brave/brave-browser/wiki).

## Downloads

We're not offering downloads yet for this next generation desktop browser.

You can [visit our website](https://brave.com/downloads.html) to get the latest stable release of our existing browser which is still in active development.

## Other repositories

For other versions of our browser which are shipping already, please see:

* macOS, Windows, Linux - [brave/browser-laptop](https://github.com/brave/browser-laptop)
* iPhone - [brave/browser-ios](https://github.com/brave/browser-ios)
* Android - [brave/browser-android-tabs](https://github.com/brave/browser-android-tabs)

## Community

[Join the Q&A community](https://community.brave.com/) if you'd like to get more involved with Brave. You can [ask for help](https://community.brave.com/c/help-me),
[discuss features you'd like to see](https://community.brave.com/c/feature-requests), and a lot more. We'd love to have your help so that we can continue improving Brave.

Join our [Discord community chat](https://discordapp.com/invite/k57tYrS) for higher bandwidth discussions.

Follow [@brave](https://twitter.com/brave) on Twitter for important news and announcements.
