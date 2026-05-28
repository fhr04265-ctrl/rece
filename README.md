# 訪問看護レセプト ローカル診断MVP

iBow から出力した訪問看護レセプトデータを、ローカルPC上で提出前チェック・売上/基本報酬ダッシュボード確認するための試作ツールです。

## 格納物

- `release/ibow-receipt-precheck-phase2-transfer.zip`
  - 単体HTMLアプリ
  - 転送用README
  - 個人情報を含まない合成サンプルCSV/UKE

## 使い方

1. `release/ibow-receipt-precheck-phase2-transfer.zip` をダウンロードします。
2. ZIPを展開します。
3. `ibow-receipt-precheck-phase2.html` をブラウザで開きます。
4. iBowから出力した介護CSVと医療訪問看護UKEを読み込ませます。

## 注意

- 実データや個人情報はこのリポジトリへアップロードしないでください。
- 本ツールはローカルブラウザ内で動作する前提です。
- MVP段階のため、判定結果は最終請求前の確認補助として使ってください。

## 現在の主な対応

- 介護保険CSV: `7131` / `7132` 系レコードの基本解析
- 医療保険訪問看護UKE: `RECEIPTH.UKE` の `RE` / `HJ` / `KA` など主要レコード解析
- 提出前リスクチェック
- 売上・基本報酬ダッシュボード
- 利用者名/IDのマスキング前提レポート出力
