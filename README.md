# 緊急避難サポートアプリ

## 概要
このアプリは、災害時の避難をサポートするためのモバイルアプリケーションです。最寄りの避難所情報の表示、災害マップの確認、防災グッズの管理など、防災に必要な機能を提供します。

## 主な機能

### 1. 避難所情報
- 現在地から最寄りの避難所を検索
- 避難所までの距離と経路を表示
- オフラインでも閲覧可能

### 2. 災害マップ
- 避難所の位置をマップ上に表示
- 災害種別による避難所の色分け表示
- 現在地表示機能

### 3. 防災グッズ管理
- 防災グッズのチェックリスト
- 期限管理機能
- カテゴリー別の整理

### 4. 気象情報
- 気象警報・注意報の表示
- 天気予報の確認

## 技術スタック
- **フロントエンド**: React Native (Expo)
- **プログラミング言語**: TypeScript
- **ナビゲーション**: React Navigation
- **位置情報**: Expo Location
- **データストレージ**: AsyncStorage
- **地図表示**: React Native Maps

## 必要要件
- **Node.js**: 14.0以上
- **Expo CLI**: 最新版
- **iOS**: 13.0以上 または **Android**: 6.0以上

## インストール手順
1. リポジトリをクローンします。
   ```bash
   git clone https://github.com/manmaru-ai/pbl1-team4.git
   ```
2. プロジェクトディレクトリに移動します。
   ```bash
   cd <project-directory>
   ```
3. 依存関係をインストールします。
   ```bash
   npx expo install
   ```
4. アプリを起動します。
   ```bash
   npx expo start
   ```

## 使用方法
アプリを起動すると、ホーム画面が表示されます。メニューから避難所情報、災害マップ、防災グッズ管理、気象情報などの機能にアクセスできます。

## ExpoSDKのアップデート手順

ExpoSDKのアップデートが必要な場合は、以下の手順で対応してください。

1. package.jsonのexpoとexpo関連パッケージを更新
   ```bash
   npx expo-doctor
   ```

2. 依存関係のアップデート
   ```bash
   npx expo install --fix
   ```

3. プロジェクトのクリーンアップ
   ```bash
   npx expo prebuild --clean
   ```

4. キャッシュのクリア
   ```bash
   npx expo start --clear
   ```

注意点:
- アップデート前に必ずプロジェクトのバックアップを取ってください
- 破壊的変更がある可能性があるため、リリースノートを確認してください
- 依存関係のバージョンの整合性に注意してください

参考: [ExpoSDK50へのアップグレード方法](https://zenn.dev/ryuu/articles/upgrade-exposdk-50)