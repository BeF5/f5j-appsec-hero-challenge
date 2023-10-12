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

8. Flags - Shadow API
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


9. Flags - High Risk API
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

10.  Flags - Automated Traffic
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

11.   Flags - Bot Detection
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

    - Token Missing
    - Token Expired
    - Interstitial Served
    - Javascript Failure

   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/

12.   Flags - Malicious User
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

13.   Flags - Unrestricted Resource Consumption
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


14.   Flags - Top Attacker
====


英文::

   Top Attacker
   15

   Can you find TLS fingerprint of top attacker across all your applications over past 24 hours using F5 Distributed Cloud?

    - 8d9f7747675e24454cd9b7ed35c58707
    - d0ee3237a14bbd89ca4d2b5356ab20ba
    - 398430069e0a8ecfbc8db0778d658d77
    - f436b9416f37d134cadd04886327d3e8
  
   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

   - Under security dashboard look for top attacker source 
   - Switch from Source IP to TLS fingerprint


和訳::

   トップアタッカー
   15点

   F5 Distributed Cloudを使用して、過去24時間のすべてのアプリケーションでトップ攻撃者（最も多く攻撃を行っている攻撃者）のTLSフィンガープリントはどれですか？

    - 8d9f7747675e24454cd9b7ed35c58707
    - d0ee3237a14bbd89ca4d2b5356ab20ba
    - 398430069e0a8ecfbc8db0778d658d77
    - f436b9416f37d134cadd04886327d3e8
    
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   - "Securiry Dashboard"で "Top Attacker"のSourceを探す
   - Source IPからTLS fingerprintに切り替える


15.   Flags - Threat Campaigns
====


英文::

   Threat Campaigns
   15

   During the last 24 hours, your organization's internet-facing applications have been subjected to scanning and attacks.
   Using F5 Distributed Cloud can you identify the attack campaign specifically targeting your Apache server
   and determine the CVE ”Common Vulnerabilities and Exposures” being exploited in this attack?
  
   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

  Check "Threat Campaigns Tab"  Under "Threat Insights" 


和訳::

   スレットキャンペーン
   15点

   過去24時間の間に、あなたの組織のインターネットに面したアプリケーションは、スキャンと攻撃を受けています。
   F5 Distributed Cloudを使用して、Apacheサーバを標的とした攻撃キャンペーンを特定し、この攻撃で悪用されているCVE IDを入力してください。
    
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   "Threat Insights"の下にある "Threat Campaigns Tab" を確認する

16.   Flags - SSRF
====


英文::

   SSRF
   15

   The F5 Distributed Cloud security dashboard has alerted a SSRF attempt on your Arcadia apigw backend application over the past 24 hours.
   Can you identify the URL the attacker was trying to access?
  
   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

  Look for SSRF in Dashboard and find the corresponding event in "Security Analytics" tab by clicking on it. 


和訳::

   SSRF
   15点

   F5 Distributed Cloudのセキュリティダッシュボードで、過去24時間以内に"Arcadia apigw backend"アプリケーションに対するSSRF攻撃の試行が警告されました。
   攻撃者がアクセスしようとしたURLを特定してください。
    
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   ダッシュボードでSSRFを探し、"Security Analytics "タブで該当するイベントをクリックして見つける。

17.   Flags - Client Side Defense
====


英文::

   Client Side Defense
   20

   The developers of Arcadia Frontend application incorporated several open-source JS packages.
   The F5 Distributed Cloud console is now alerting you about potential malicious behavior exhibited by a script on users' browsers. 
   Can you identify the name of the script that has interacted with five or more high-risk sites in the past 30 days?
  
   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

  - From security dash board click on Arcadia frontned 
  - Goto client side defense widget 
  - Click Goto dashboard 
  - Click on script list and check last 30 days window 


和訳::

   Client Side Defense
   20点

   "Arcadia Frontend"アプリケーションの開発者は、クライアント側で動作するいくつかのオープンソースのJava Scriptパッケージを組み込みました。
   F5 Distributed Cloudコンソールは、ユーザーのブラウザ上でスクリプトが示す潜在的な悪意のある動作について警告しています。
   過去30日間に危険度5以上と判定されているサイトと通信したスクリプトの名前はなんですか？
    
   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

   - セキュリティ・ダッシュボードから Arcadia frontned をクリックする。
   - Client Side Defenseウィジェットに移動 
   - ダッシュボードに移動 
   - Script listをクリックし、過去30日間の期間をチェックする。

18.   Flags - Security Posture: Authentication
====


英文::

   Security Posture: Authentication
   25

   While conducting the audit on Arcadia APIGW backend on F5 Distributed Cloud console, 
   you discover a high-risk API /api/v2/moveOrder. 
   Can you investigate the authentication-related vulnerabilities associated with this API?
  
    - API key not rotated
    - Weak JWT
    - No Authentication
    - Alert is a false positive

   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

  1. Under "Dashboard" look for the API Gateway backend. 
  2. Inspect the API Endpoint for the stated API and look under "Security Posture 


和訳::

   セキュリティポスチャ: 認証
   25点

   F5 Distributed Cloudコンソールで"Arcadia APIGW backend"の監査を行っているときに、
   リスクの高いAPI /api/v2/moveOrderを発見しました。このAPIに関連する認証関連の脆弱性を次の中から選択してください。

    - API key not rotated
    - Weak JWT
    - No Authentication
    - Alert is a false positive

   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

  1. Dashboardで"API Gateway backend" を探す
  2. 指定されたAPIのAPIエンドポイントを調べて、"Security Posture"の下を確認する

19.  Flags - API Drift
====


英文::

   API Drift
   25

   According to your organizational policy and the Open API Specification/ Swagger, OAuth tokens are mandated for API authorization for Arcadia frontend APIs . 
   However, the developers recently made updates to the "Arcadia Frontend" application that deviated from this policy. 
   F5 Distributed Cloud security analytics dashboard has reported these API deviations within the past 24 hours. 
   Can you locate the value of the Violation related to these incidents?

   Credentials have been emailed to you as part of registration & console is located here
   https://f5-xctestdrive.console.ves.volterra.io/

Hints::

  Under security Anlaytics , Look for "API" events  with Mode as "Report" 
  Study any event and look for violations 
  The answer is base 64 encoded  


和訳::

   APIドリフト
   25点

   組織のポリシーとOpen API Specification/Swaggerによると、"Arcadia frontend"のAPI認証にはOAuthトークンが必須です。
   しかし、開発者は最近、"Arcadia Frontend"アプリケーションにこのポリシーから逸脱したアップデートを行いました。
   F5 Distributed Cloudのセキュリティ分析ダッシュボードは、過去24時間以内にこれらのAPIの逸脱を報告しています。
   これらのインシデントに関連する違反の値を入力してください。

   コンソールは、以下より利用可能です。ログイン情報は指定のものを使ってください。
   https://f5-xctestdrive.console.ves.volterra.io/


ヒント::

  Security Anlayticsの下で、Modeが"Report"の”API"イベントを探す。
  違反となっているイベントを探す。
  答えは、Base64でエンコードされている
