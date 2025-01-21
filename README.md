<h1>Wetube Reloaded プロジェクト</h1>

Wetube Reloaded は、Node.js を使用した 動画共有ウェブアプリケーション であり、YouTube のような機能を提供するクローンプロジェクトです。

このプロジェクトは Express.js、MongoDB、Pug、Webpack、ES6+、などの技術を活用して開発されています。


---------------------------------------------------

🔹 プロジェクト概要

Wetube Reloaded は、ユーザー登録およびログイン機能を備えており、ユーザーが 動画をアップロード、視聴、コメント投稿 できるウェブアプリです。

主な機能として、ユーザー認証、動画のアップロード・管理、コメントシステム、ソーシャルログイン (GitHub 連携) などがあります。


---------------------------------------------------


🔹 技術スタック

✅ バックエンド (Backend)

  Node.js: サーバーサイド JavaScript 実行環境

  Express.js: ウェブアプリケーションフレームワーク

  MongoDB & Mongoose: NoSQL データベースおよび ODM (Object-Document Mapping) ライブラリ

  Bcrypt: パスワードの暗号化とセキュリティ処理


✅ フロントエンド (Frontend)

  Pug: テンプレートエンジンを使用した HTML レンダリング

  Webpack: バンドルおよびコードの最適化

  SCSS: スタイリングとレスポンシブデザイン


✅ その他 (DevOps & Deployment)

  ES6+ (Modern JavaScript): 最新の JavaScript 構文を使用

  Multer: ファイルアップロード処理 (動画アップロード)

  Fly.io: PaaS (Platform as a Service) を利用したデプロイ


  ----------------------


🔹 主な機能説明

🔸 1. ユーザー登録およびログイン (User Authentication)

    メール/パスワードによるアカウント登録・ログイン
    
    GitHub ソーシャルログイン対応 (OAuth 2.0)
    
    Bcrypt によるパスワードの暗号化
    
    Session & Cookie を利用したログイン状態の維持
    
🔸 2. 動画のアップロードおよび管理 (Video Upload & Management)

    ユーザーは 動画をアップロード し、管理可能
    
    タイトル、説明、ハッシュタグ の追加が可能
    
    Multer ミドルウェア を利用したファイルアップロード処理
    
🔸 3. 動画視聴およびコメント機能 (Video Watching & Comments)

    アップロードされた動画を ストリーミング再生 可能
    ユーザーは 動画にコメントを投稿・削除 可能
    AJAX を利用した非同期コメント処理

    
🔸 4. 検索機能 (Search)

    タイトルまたはハッシュタグ を使用した動画検索
    MongoDB の $regex クエリを活用した検索機能
    
🔸 5. ユーザープロフィール管理 (User Profile)

    プロフィール写真のアップロード・変更
    ユーザー情報の編集 (名前、メールアドレスなど)
    アップロードした動画の一覧表示
    
🔸 6. ソーシャルログイン (GitHub OAuth)

    GitHub アカウントを使用したログイン
    OAuth 2.0 による GitHub API 連携
    GitHub のプロフィール情報 (メールアドレス、プロフィール写真) を取得
    
🔸 7. レスポンシブ UI およびデザイン

    Pug テンプレートエンジンを使用した UI 設計
    SCSS を利用したスタイリング
    レスポンシブデザイン に対応し、PC・モバイルの両方に最適化


-----------------

 プロジェクトフォルダ構成

 
wetube-reloaded/

│── src/

│   ├── controllers/   # ビジネスロジックを担当するコントローラー

│   ├── middlewares/   # ミドルウェア (セキュリティ、ファイルアップロードなど)

│   ├── models/        # MongoDB スキーマおよびモデルの定義

│   ├── routers/       # Express ルーティング定義

│   ├── views/         # Pug テンプレートファイル (フロントエンド)

│   ├── assets/        # SCSS およびフロントエンドファイル

│   ├── init.js        # サーバーの初期設定

│   ├── server.js      # Express サーバーの起動スクリプト

│── .gitignore         # Git に含めないファイルリスト

│── package.json       # プロジェクト情報および依存関係

│── webpack.config.js  # Webpack 設定ファイル



------------


🔹 動作フロー

ユーザーは 新規登録 または GitHub ログイン でアカウントを作成

ログインしたユーザーは 動画をアップロード し、タイトルや説明、ハッシュタグを追加

他のユーザーは 動画を検索・視聴・コメント投稿 可能

ユーザーは プロフィールの編集 や アップロード動画の管理 を実施


-------------

🔹 まとめ

このプロジェクトを通じて、Node.js と Express を活用したフルスタックアプリケーションの開発方法を学びました。

MongoDB を使用したデータ管理や、ファイルアップロード処理 の実装方法を習得しました。

Webpack を使用したフロントエンドリソースの最適化や、Pug テンプレートエンジンを利用したサーバーサイドレンダリング (SSR) の理解を深めることができました。




















