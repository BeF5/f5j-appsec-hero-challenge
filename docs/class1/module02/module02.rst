F5 AppSec Hero Challenge 日本語訳
####

1. Give Away - This CTF is brought to you by
====

英文::

   This CTF is brought to you by
   5


Hints::

   Its the tornado category on a red dot 

和訳::

   このCTFイベントを提要している会社の略称を入力してください。
   5点

ヒント::

   赤いロゴに記載されている文字。トルネードのカテゴリを意味する。


1. Quizzes - Understanding Inventory
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
    - ゾンビ API
    - ローグ API
    - シャドー API
    - ディスカバード API

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
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

   Dashboard has the list of all applications exposed and status of WAF

和訳::

   セキュアでないWebアプリケーション
   10点

   F5 Distributed Cloudのアプリケーションインベントリにおいて、Webに公開されているがWAFによる保護がされていないアプリケーション（ロードバランサー名）を特定してください。

   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   ダッシュボードでは、公開されているすべてのWebアプリケーションのリストとWAFのステータスが表示されます。

7. Flags - GraphQL Violations
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
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

   Look for top attacks by violations in dashboard 

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
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   ダッシュボードで当該違反によるトップの攻撃を探す

1. Flags - Shadow API
====


英文::

   Shadow API
   15

   You are performing a security audit for all the Arcadia APIGW Backend APIs on F5 Distributed Cloud dashboard.
   Can you determine the total count of undocumented API detected by the system in past 24 hours

   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

   Look for the "api-gw-backend" loadlabcer and study its 'API Endpoints'


和訳::

   シャドーAPI
   15点

   あなたは、F5 Distributed Cloud dashboardで確認できる全てのArcadia APIGW Backend APIのセキュリティ監査を実施しています。
   過去24時間以内に検出された文書化されていないAPIの総数を入力してください。
  
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   api-gw-backend "ロードラバーサーを探し、その "API Endpoints "を調べる。


1. Flags - High Risk API
====


英文::

   High Risk API
   15

   While conducting the security audit of all Arcadia APIGW Backend APIs on the F5 Distributed Cloud security dashboard,you come across several high-risk APIs.
   Can you specifically identify the high-risk undocumented API that exposes Credentials identified over past 24 hours?
    - /api/v2/changeOrderById
    - /api/v2/placeOrder
    - /api/v2/moveOrder
    - /api/v2/updatePaymentInfoById/{DYN}
    - /api/v2/changeOrderById

   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/


Hints::

   - Go to "apigw-backend-lb" 
   - Go to "API Endpoints" 
   - Study the Apiendpoints in "table view"  

和訳::

   ハイリスクなAPI
   15点

   F5 Distributed Cloudのセキュリティダッシュボードで、すべての Arcadia APIGW Backend API のセキュリティ監査を実施しているときに、
   いくつかのハイリスクなAPI に遭遇しました。過去 24 時間に確認されたクレデンシャルを公開している文書化されていないハイリスクなAPIを選択してください。
    - /api/v2/changeOrderById
    - /api/v2/placeOrder
    - /api/v2/moveOrder
    - /api/v2/updatePaymentInfoById/{DYN}
    - /api/v2/changeOrderById 
  
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   - "apigw-backend-lb "に移動する。
   - "API Endpoints"タブを選択
   - "table view"で、APIエンドポイントを調べる

1.  Flags - Automated Traffic
====


英文::

   Automated Traffic
   15

   Due to the upcoming IPO, your organization's public website in the Asia Region has experienced a surge in popularity and, consequently, has become a frequent target of bots. 
   Using F5 Distributed Cloud dashboard can you determine which category of pages is receiving the highest volume of bot traffic?
    - Authentication
    - Account Management
    - Profile Management
    - Unknown

   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

   Switch to "Bot Defense View" from Select Service  and Filter traffic for region "Asia" 

和訳::

   自動化されたトラフィック
   15点

   近々予定されているIPOのため、アジア地域にある組織の公開ウェブサイトは人気が急上昇し、その結果、ボットの頻繁な標的となっています。
   F5 Distributed Cloudのダッシュボードを使用して、ボットのトラフィック量が最も多いページのカテゴリを特定してください。
    - Authentication
    - Account Management
    - Profile Management
    - Unknown
  
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   "Select Service"から"Bot Defense View"に切り替え、"Asia"リージョンでフィルタリングする。

1.   Flags - Bot Detection
====


英文::

   Bot Detection
   15

   During the assessment of the Arcadia frontend application traffic, you observe numerous blocked automation attempts by the system.
   Could you identify the primary reason code for the requests being blocked over the last 7 days?
    - Token Missing
    - Token Expired
    - Interstitial Served
    - Javascript Failure

   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

和訳::

   Botの検出
   15点

   "Arcadia frontend"アプリケーションの評価中に、システムによってブロックされた自動化されたリクエストが多数あることを確認しました。
   過去7日間にブロックされたリクエストのうち、最も主要なものを選択してください。
    - Authentication
    - Account Management
    - Profile Management
    - Unknown
  
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/

1.  Flags - Malicious User
====


英文::

   Malicious User
   15

   Amidst the ongoing targeting of your public-facing website Arcadia Frontend by different threat actors, 
   there has been one particular threat actor making multiple forbidden access attempts and triggering several WAF events over the past 24 hours.
   Using F5 Distributed Cloud can you identify the TLS fingerprint associated with this specific threat actor?

   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

   - Goto to "arcadia-front-end-lb"  from the Security Dashboard 
   - Click on Malicious User 
   - Study the High risk user 

和訳::

   悪意のあるユーザ
   15点

   さまざまな攻撃者によって貴社の公開Webサイト"Arcadia Frontend"が標的とされ続けている中、
   ある特定の攻撃者が過去24時間の間に何度も禁止されたアクセスを試み、複数のWAFイベントをトリガーしています。
   F5 Distributed Cloudを使用して、この特定の攻撃者に関連するTLSフィンガープリントをしてください。
  
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   - "Securiry Dashboard"から "arcadia-front-end-lb "に移動する。
   - "Malicious User"をクリック
   - ”High risk”と判断されているユーザを調べる

1.  Flags - Unrestricted Resource Consumption
====


英文::

   Unrestricted Resource Consumption
   15

   In accordance with the OWASP API Top 10 compliance, your organization has implemented resource consumption restrictions. 
   Using F5 Distributed Cloud console, can you identify the request path where users, whether malicious or otherwise, are encountering these restrictions over the past 24 hours?
   
   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

   - Under REquests Tab Look for Resp code 429   in last 24 hours 
   Alternatively 
   - Under Security Analytics looks for API events 
   - Look for Resp Code  429 


和訳::

   制限されていないリソース消費
   15点

   OWASP API Top 10 コンプライアンスに従って、あなたの組織はリソースの消費制限を実装しました。
   F5 Distributed Cloudコンソールを使用して、悪意があるかどうかにかかわらず、過去24時間にユーザーがこれらの制限に遭遇しているリクエストパスを特定してください。
  
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   - Requestタブで、過去24時間以内のレスポンスコード 429のログを探す
   または、
   - Security AnalyticsのAPI eventsを探す
   - レスポンスコード 429のログを探す













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
