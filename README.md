# -test-codespace-storybook

## アプリプロジェクトの概要

このプロジェクトは、ReactとTypeScriptを使用して構築されたフロントエンドアプリケーションです。以下の主要な技術とツールが使用されています。

- **React**: ユーザーインターフェースを構築するためのJavaScriptライブラリ。
- **TypeScript**: 型安全なJavaScript。
- **Vite**: 高速なビルドツールと開発サーバー。
- **Tailwind CSS**: ユーティリティファーストのCSSフレームワーク。
- **Storybook**: UIコンポーネントの開発とドキュメント化を支援するツール。

## Reactの起動方法

### 起動手順

1. 必要な依存関係はdevcontainerの設定で自動的にインストールされています。

2. プロジェクトディレクトリに移動します。
   ```bash
   cd react-ts-project
   ```

3. Reactアプリケーションを起動します。
   ```bash
   npm run dev
   ```

4. ターミナルに出力されたURLからブラウザで `http://localhost:5173` を開き、アプリケーションを確認します。

### ポイント

- 開発サーバーはホットリロードをサポートしており、コードを変更すると自動的にブラウザが更新されます。
- 必要に応じて、`vite.config.ts` ファイルを編集してポートや設定を変更できるが、基本的にはDocker側でコントロールする方が良い

## Storybookの起動方法

### 起動手順

1. 必要な依存関係はdevcontainerの設定で自動的にインストールされています。

2. プロジェクトディレクトリに移動します。
   ```bash
   cd react-ts-project
   ```

3. Storybookを起動します。
   ```bash
   npm run storybook
   ```

4. ターミナルに出力されたURLからブラウザで `http://localhost:6006` を開き、Storybookのインターフェースを確認します。

### ポイント

- Storybookはコンポーネントのプレビューやドキュメント化に役立ちます。
- 必要に応じて、`package.json` ファイルを編集してスクリプトや設定を変更できます。

## VS Code Debugger 設定について

現代会では、VS Code Debugger の設定において最新の `pwa-msedge` タイプを採用しなかった。その理由として、`pwa-msedge` を使用しようとした際に、Codespace 環境での互換性に関する注意が表示された。このため、安定性を優先し、従来の `msedge` タイプを使用。
CodespaceをVScodeを使って行うことを考えると問題はなさそうだが、未検証のため、一旦msedgeにしておく。