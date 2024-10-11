<div id="top"></div>

## 使用技術一覧

<!-- シールド一覧 -->
<!-- 該当するプロジェクトの中から任意のものを選ぶ-->
<p style="display: inline">
  <!-- バックエンドの言語一覧 -->
  <img src="https://img.shields.io/badge/-Python-F2C63C.svg?logo=python&style=for-the-badge">
</p>

## 目次

1. [プロジェクトについて](#プロジェクトについて)
2. [環境](#環境)
3. [ディレクトリ構成](#ディレクトリ構成)
4. [開発環境構築](#開発環境構築)
5. [トラブルシューティング](#トラブルシューティング)

<p align="right">(<a href="#top">トップへ</a>)</p>

## プロジェクト名

LSTMによる株価予測モデルの構築

<!-- プロジェクトについて -->

## プロジェクトについて

LSTMリカレントニューラルネットワークを用いてNTTの株価を予測

<p align="right">(<a href="#top">トップへ</a>)</p>

## 環境

<!-- 言語、フレームワーク、ミドルウェア、インフラの一覧とバージョンを記載 -->

| 言語  | バージョン |
| --------------------- | ---------- |
| Python                | 3.10.12     |
Google Colaboratory

<p align="right">(<a href="#top">トップへ</a>)</p>

## 実行方法

### 1. Colab へのアクセス
- まず、Google Colaboratory にアクセスします。以下のリンクからアクセスできます:
  [Google Colaboratory](https://colab.research.google.com)

### 2. ノートブックを開く
- Google Colab の「ファイル」で、右下の「ノートブックを開く」をクリックします。

### 3. Driveにファイルをアップロード
- Google Driveを開きます。以下のリンクにアクセスし、「新規」→「ファイルをアップロード」からCSVファイルをドライブにアップロードします:
  [Google Drive](https://drive.google.com/drive)

### 4. ドライブをマウント
- Google Colaboratoryに戻り、左のファイルアイコンをクリックし、ドライブをマウントするアイコンをクリックします。

### 5. ファイルパスの書き換え
- Colab画面の左のファイルアイコンをクリックし、CSVファイルのパスをコピーします。そのパスに、セクション「０．準備」の3つ目のセルの中にあるパスを書き換えます。

### 6. コードの実行
- 「ランタイム」→「すべてのセルを実行」をクリックします。

<p align="right">(<a href="#top">トップへ</a>)</p>

## プログラムの概要

このプログラムは、株価の時系列データを用いて、将来の株価を予測するモデルを構築することを目的としています。

処理の流れは以下のとおりです。

### 1. データの読み込みと準備
- CSVファイルから株価データを読み込みます。
- データの型を確認し、欠損値を処理します。
- 列名を英語に変換します。
- 日付データを適切な形式に変換します。

### 2. 特徴量エンジニアリング
- 過去の株価や出来高、変化率などの情報を用いて、新しい特徴量を作成します。
- 年、月、週などの周期性を表現する特徴量も作成します。
- 不要な特徴量を削除します。

### 3. でー
