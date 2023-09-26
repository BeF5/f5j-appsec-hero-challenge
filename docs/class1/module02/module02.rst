F5 AppSec Hero Challenge 日本語訳
####

1. Give Away - This CTF is brought to you by
====

英文::

   This CTF is brought to you by
   5

和訳::

   このCTFイベントを提要している会社の略称を入力してください。
   5点

ヒント::

   赤いロゴに記載されている。トルネードのカテゴリを意味する。


2. Quizzes - Understanding Inventory
====


英文::

   Understanding Inventory
   5

   What are APIs that lack documentation in Inventory or hidden commonly referred to as?
    - Zombie API
    - Rogue API
    - Shadow API
    - Discovered API

和訳::

   APIのインベントリ（資産化）の理解
   5点

   ドキュメント化されていない、あるいは、適切な管理がされていない状態で公開されているAPIは一般的に何と呼ばれるか？
   選択肢から選んでください。
    - Zombie API
    - Rogue API
    - Shadow API
    - Discovered API

3. Quizzes - Too many requests
====

英文::

   Too many requests
   5

   Which HTTP response code is generated when a user sends an excessive number of requests and gets rate-limited?

和訳::

   Too many requests
   5点

   ユーザが過剰な数のリクエストを送信した結果、
   レート制限を受けた際に応答として受けるHTTPレスポンスコードを入力してください

4. Quizzes - Fingerprint user
====

英文::

   Fingerprint user
   5

   What is the preferable choice for identifying a threat actor?
    - Client IP Address
    - Client ASN
    - TLS Fingerprint
    - User Agent
  
和訳::

   不正ユーザを識別する特徴
   5点

   脅威をもたらす不正ユーザを識別するための特徴として、
   最も適切な選択肢を選択してください。
    - Client IP Address
    - Client ASN
    - TLS Fingerprint
    - User Agent

5. Quizzes - Base64
====


英文::

   Base64
   5

   Can a base64 string be decoded without any key
    - Yes
    - No

和訳::

   Base64
   5点

   「Base64でエンコードされた文字列は、鍵を使わずにデコードできる」。この記述は正しいですか？
    - Yes
    - No

6. Flags - Unsecure App
====


英文::

   Unsecure App
   10

   While examining your application inventory on F5 Distributed Cloud, 
   can you identify the application（Load balancer name）that is exposed to the web but lacks WAF protection?

   Credentials have been emailed to you as part of registration & console is located here

和訳::

   セキュアでないWebアプリケーション
   10点

   F5 Distributed Cloudのアプリケーションインベントリにおいて、Webに公開されているがWAFによる保護がされていないアプリケーション（ロードバランサー名）を特定してください。

   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   `https://f5-xctestdrive.console.ves.volterra.io/ <https://f5-xctestdrive.console.ves.volterra.io/ >`_


ヒント::

   ダッシュボードでは、公開されているすべてのWebアプリケーションのリストとWAFのステータスが表示されます。

1. Flags - GraphQL Violations
====


英文::

   GraphQL Violations
   10

   From the F5 Distributed Cloud Dashboard, 
   can you identify the most significant GraphQL violation in the past 24 hours on the Arcadia Frontend messaging platform, 
   which operates on a modern API with GraphQL and has attracted the attention of attackers?
    - VIOL_GRAPHQL_FORMAT
    - VIOL_GRAPHQL_MALFORMED
    - VIOL_GRAPHQL_INTROSPECTION_QUERY
    - VIOL_GRAPHQL_BATCH_EXCEEDED

   Credentials have been emailed to you as part of registration & console is located here

和訳::

   GraphQL に関する違反
   10点

   GraphQLを使用したAPIサービスであるArcadia FrontendメッセージングプラットフォームをF5 Distributed Cloud Dashboardで保護しています。
   このアプリケーションで、過去24時間に発生した最も重大なGraphQLに関する違反は、次のうちどれですか？
    - VIOL_GRAPHQL_FORMAT
    - VIOL_GRAPHQL_MALFORMED
    - VIOL_GRAPHQL_INTROSPECTION_QUERY
    - VIOL_GRAPHQL_BATCH_EXCEEDED
  
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   `https://f5-xctestdrive.console.ves.volterra.io/ <https://f5-xctestdrive.console.ves.volterra.io/ >`_


ヒント::

   ダッシュボードで当該違反によるトップの攻撃を探す















1. F5 DCS WAAPの構成
====

F5 DCS WAAPの構成について紹介します。

   .. image:: ./media/dcs-waap-lab-diagram.JPG
       :width: 400

こちらに示している各種機能をF5 DCSのコンソール画面から設定します

| F5 DCSには ``Tenant`` と ``Namespace`` があり、その配下で各種設定オブジェクトを管理します。
| 契約者毎に ``Tenant`` が割り当てられます。あるTenantに所属するユーザは、そのTenanat内に ``Namespace`` を作成することが可能です
| また、ユーザが定義する Namespace の他に、いくつかの Namespace が存在します
| 詳細は、 `Core Concepts <https://docs.cloud.f5.com/docs/ves-concepts/core-concepts>`__ を参照してください。

   .. image:: ./media/dcs-waap-tenant-ns.JPG
       :width: 600

その他WAAPの設定に関連するオブジェクトを示します。
こちらの例ではユーザが定義した2つの Namespace にそれぞれHTTP Load Balancerを構成しています。
HTTP Load Balancerはその提供機能に応じた設定パラメータを持ちます。各機能は、HTTP Load Balancerの設定項目としてパラメータを指定します。
一部の設定については、Namespace 内で別の 設定オブジェクト として定義され、それらを参照する構成をとります。
HTTP Load Balancerの外部で定義された 設定オブジェクト は同一Namespace内の別のHTTP Load Balancerから参照可能です。

また、一部の設定オブジェクトについては、Shared Object として作成することが可能です。このオブジェクトは、複数のName Spaceから参照することができます。

   .. image:: ./media/dcs-waap-objects.JPG
       :width: 600

3. Namespaceの作成
====

本ラボで利用する ``Namespace`` を別に作成する場合、新規に作成頂くことが可能です。
すでに利用できる ``Namespace`` があり、新規に作成が不要である場合、こちらの手順をスキップしてください

F5 DCS のコンソールを開き、 ``Administration`` を開きます

   .. image:: ./media/dcs-console-administration.JPG
       :width: 400

Personal Management の ``My Namespaces`` を開き、上部に表示される ``Add namespaces`` をクリックしてください

   .. image:: ./media/dcs-waap-add-namespace.JPG
       :width: 400

表示される項目を入力し、 ``Save changes`` をクリックしてください

   .. image:: ./media/dcs-waap-add-namespace2.JPG
       :width: 400

4. Tenant ID等の確認
====

ご利用されるアカウントのテナントID等の情報は以下の手順でご確認いただけます。
それぞれの情報はTerraform/APIなどで利用いたします。利用の際にはこちらの項目をご確認ください。

F5 DCS のコンソールを開き、 ``Administration`` を開きます

   .. image:: ./media/dcs-console-administration.JPG
       :width: 400

画面左側 ``Tenant Settings`` の ``Tenant Overview`` を開き、画面に表示される内容を確認してください。

   .. image:: ./media/dcs-administration-tenant-information.jpg
       :width: 400
