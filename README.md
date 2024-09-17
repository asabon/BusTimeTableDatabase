[![Release](https://github.com/asabon/BusTimeTableDatabase/actions/workflows/release.yml/badge.svg?branch=main)](https://github.com/asabon/BusTimeTableDatabase/actions/workflows/release.yml)

# BusTimeTableDatabase

## 概要

* json 形式で作成した、バスの時刻表データベース。
* 手作業での入力のため、自分が必要な部分しか入力してない。

## 目的

* バスの時刻表を扱うアプリから参照する。

## ディレクトリ構成

```text
+ database/       : 時刻表データ本体
+ release/        : 最新の成果物
  + hash.txt      : json データの hash 。前回取得時から値が変わっていたら database に変更が入っている。
  + timetable.zip : database 以下を zip で固めたもの。
```

### 第一階層 (database/*)

```text
+ kanachu/       : 会社「kanachu」のディレクトリ
+ companies.json : この階層にある「会社」ディレクトリの説明
```

### 第二階層 (database/*/*)

```text
+ m12/         : 系統「m12」のディレクトリ
+ ...
+ systems.json : この階層にある「系統」ディレクトリの説明
```

## LICENSE

MIT License.

