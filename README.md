# JHipster-Ionic (Work in Progress)

Example showing how to build an [Ionic](http://ionicframework.com/) app using [JHipster](http://jhipster.github.io/) as backend

The project is structured in 2 modules:
- server: the JHipster backend
- mobile: the Ionic app

## Environment

- Ubuntu
- java 8
- node 0.12.4
- Android SDK

## Generating modules

### Server

    mkdir server
    cd server
    yo jhipster

I chose the default options except for:

- gradle to be consistent with Android and [Apache Cordova](https://cordova.apache.org/)
- gulp to be consistent with [M-generator](https://github.com/mwaylabs/generator-m) and Ionic
- no translation

Test that app works:

    ./gradlew bootRun

Open http://127.0.0.1:8080

### Mobile App

The Ionic app was generated by Yeoman [M-generator]

    mkdir mobile
    cd mobile
    yo m

I chose the default options except for:

- appName: "jhipsterApp" to be consistent with JHipster angular module
- appId: "com.mycompany.myapp" to be consistent with JHipster
- no i18n/l10n
- no iOS

Test that app works in browser:

    gulp watch

Open http://127.0.0.1:9000

