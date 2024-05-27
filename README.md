> 以下の内容はあくまで参考です。ここまでのものを作るという意味ではないので、注意ください。内容的にもでっち上げに近いです（提案内容に影響を与えないためです）。ただし、作成する内容や筋を通すことは重要です。
> また、例として記載しているのは、1章以降は全て「こういうことを書くと良い」というもので、同じように書くだけでは、説明が不足していますので注意して下さい（このエリアは削除してください）

# 0. タイトル
**説明:** 企画名や班番号、チームメンバーの列挙（学籍番号、名前）をしてください。企画名は、プロジェクトの目的や内容を端的に示すと良いでしょう。また、副題でアプリ名を追加することも考えられます

- **例:**
  - **企画名:** スマートホーム環境の実現に向けたM5Stackユビキタス環境の開発
  - **班番号:** RWC24-group00
  - **チーム名:** あればぜひ書きましょう
  - **チームメンバー:**
    - 2312110000：近大 マグロ
    - 2312119999：近大 タイ
    - 2312111111：近大 ナマズ
    - 2312112222：近大 クエ
    - 2312113333：近大 マンゴー
  
# 1. システム化の背景
**説明:** 
ここでは、なぜこのシステムが必要かを説明します。現在の課題や問題点を明確にし、それを解決するためにIoT技術をどう活用するかを述べます。この背景説明は、システムの目的（次章）が妥当なもの（確かにそのアプリがいる）ということを示す基礎となります。
また、M5Stackの技術調査も含めてください。M5Stackの利用は課題上必須です。

- **例:**
  - スマートホーム技術の普及とその重要性
  - 現在の家庭環境における課題（エネルギー効率、セキュリティ、利便性の向上）
  - M5Stackの特性と利点（例：低コスト、高拡張性）

# 2. システムの目的
**説明:** 
このセクションでは、このシステムを開発する具体的な目的やゴールを述べます。誰に、いつ、どこで、どのような価値を提供するのかを明確にし、M5Stackと各種情報技術に基づいて解決可能な課題であることを記載します。

### 顧客

**説明:** 
ここでは、システムを利用するターゲットユーザーを明確にします。顧客の特性やニーズを具体的に記載し、システムの価値を伝える対象を明示します。

- **例:**
  - **家庭の主婦:** 日常の家事や家庭管理を効率化し、家族全体の生活品質を向上させることを求めている。そのため、朝、設定された時間にカーテンが自動で開き、エアコンが快適な温度に調整される。また、外出時に消し忘れた家電をスマートフォンで確認し、遠隔操作で電源を切ることができるような機能を提供する
  - **シニア層:** 高齢者の安全性と利便性を確保し、独立した生活を支援するためのツールを必要としている。そのため、転倒を検知するセンサーを設置し、転倒時には即座に家族に通知が行く。また、音声操作により簡単に家電を操作できるようにする。


### 課題

**説明:** 
顧客が抱える具体的な問題やニーズを明確にします。これらの課題を解決するために、システムがどのように貢献するかを説明します。

- **例:**
  - **家庭の主婦:** 家事の自動化とエネルギー管理の効率化が求められている。例えば、エアコンや照明の自動制御、家電の使用状況のモニタリング。
  - **シニア層:** 安全性の確保が重要。緊急時のアラートシステムや、リモートでの家族による見守り機能が必要。

### 提供内容

**説明:** 
システムが提供する具体的な解決策や機能を記載します。これにより、顧客の課題をどのように解決するかを具体的に示します。

- **例:**
  - **スマートデバイスの統合:** M5Stackを中心としたスマートデバイスの統合プラットフォームを提供し、家庭内のすべてのデバイスを一元管理。
  - **自動制御とモニタリング:** エネルギー効率を高めるための自動制御システム。温度センサーや光センサーを利用して、エアコンや照明を自動的に調整。
  - **安全管理:** 緊急時に家族や医療サービスに通知するアラートシステム。動きセンサーを使用して、異常な活動を検出し、リモートで通知。
  - **ユーザーフレンドリーなインターフェース:** 直感的な操作が可能なアプリケーションを提供し、技術に詳しくないユーザーでも簡単に利用可能。


# 3. システムの概念設計
**説明:** システムの全体像や各コンポーネントの設計について説明します。具体的なIoTデバイスの種類やその機能、アプリケーションの動作概要を記載します。

## システム構成図
**説明:** システムのそれぞれのセンサーやM5Stack、サーバーシステムなどの要素が、他とどういう関係性にあるかを図で示してください。今回は簡易的で良いので、以下のサイトのような記載を検討してください
https://blog.soracom.com/ja-jp/wp-content/uploads/2021/02/fig01.png

## コンポーネントと機能
**説明:** 構成図にあるコンポーネントと機能を記載して下さい

- **センサー類:** 温度センサー、湿度センサー、光センサー、動きセンサー。データ収集とモニタリングを行う
- **アクチュエーター類:** スマートライト、スマートサーモスタット、ドアロック、カメラ。機器の自動制御を行う
- **ゲートウェイ:** Raspberry PiやArduinoなどのIoTデバイスを統括するハブ。機器の自動制御、およびユーザへの通知機能を提供する
- **クラウドプラットフォーム:** AWS IoTやGoogle Cloud IoT Core。デバイスを統合

# 4. 役割分担
**説明:** プロジェクトチーム内での各メンバーの役割や担当分野を明確にします。誰が何を担当するのかを具体的に記載します。

- **例:**
  - **プロジェクトマネージャー: 近大太マグロ** プロジェクト全体の進行管理、スケジュール作成、進捗確認
  - **ハードウェア担当: 近大タイ** センサーやアクチュエーターの選定、接続、設定
  - **プログラマ: 近大ナマズ** ユーザーインターフェースの設計・開発、データの視覚化
  - **プログラマ: 近大クエ** サーバーサイドの設計・開発、データベース管理、APIの実装
  - **プログラマ: 近大マンゴー** 収集データの分析、アルゴリズムの設計・実装

# 5. 今後の計画
**説明:** プロジェクトの今後（前期中）のスケジュールやステップを明確にします。各段階での具体的な活動内容や目標を記載します。

- **例:**
  1. **4月**:
     - プロジェクトチームの編成、役割分担の確認
     - ユーザー調査と要件収集を実施
  2. **5月**:
     - IoTデバイスとアプリケーションフレームワークの評価
     - システムの概念設計とアーキテクチャの詳細設計
  3. **6月**:
     - 各コンポーネントの開発を開始
     - プロトタイプの開発に向けて、モックアップの作成を開始
     - コンポーネントの実装
  4. **7月**:
     - プロトタイプのテストと修正
     - ユーザーインターフェースのデザインと実装
     - 最終的なプロトタイプの完成とテスト
