#### [prev](./welcome.md) | [home](./welcome.md)  | [next](./findings.md)

# はじめに

クラウド環境に移行すると、展開されたワークロードを適切にコントロールすることが大きな課題になります。様々な調査では CEO や CIO などは、クラウドの全体を把握できるかどうかという可視性について懸念を抱いていることがわかっています。

Microsoft Defender for Cloud を活用することでクラウド環境の把握とコントロールが可能になります。

![Cyber Security Framework](./images/csf.png)
[NIST Cyber Security Framework](https://www.nist.gov/cyberframework)

## クラウド セキュリティ態勢管理 (CSPM)

CSPM の機能は無償の「基本的な CSPM」と有償の「Defender クラウド セキュリティ態勢管理 (CSPM)」の２つのプランが用意されており、サーバー、ストレージ、SQL、ネットワーク、アプリケーション、ワークロードなど、Azureで稼働しているクラウド リソースのセキュリティ状態を確認することができます。

[Microsoft Docs](https://docs.microsoft.com/ja-jp/azure/security-center/security-center-introduction) からの引用 - Microsoft Defender for Cloud は、3 つの緊急性が高いセキュリティの課題を対処します:

* **急速に変化するワークロード** – これはクラウドの強みであり、課題でもあります。 一方、エンド ユーザーはより多くの処理を実行できます。 さらに、使用および作成されている常に変化するサービスが、お客様のセキュリティ基準に準拠し、セキュリティのベスト プラクティスに従っていることを確認するにはどうすればよいでしょうか。

* **ますます高度になる攻撃** - ワークロードをどこで実行する場合でも、攻撃はますます高度になっています。 パブリック クラウドのワークロードを保護する必要があります。これは実質的にインターネットに接続しているワークロードであり、セキュリティのベスト プラクティスに従わないと、さらに脆弱になる可能性があります。

* **セキュリティ スキルの不足** - セキュリティ アラートとアラート システムの数は、環境が保護されているかどうかを確認するために必要な経歴と経験を持つ管理者の数を上回っています。 最近の攻撃の最新情報を把握し続けることは常に課題であり、セキュリティの世界が絶え間なく変化する最前線に立ち続けることは不可能です。

Microsoft Defender for Cloud の最大のメリットは、['Secure Score'](https://docs.microsoft.com/en-us/azure/security-center/secure-score-security-controls#security-controls-and-their-recommendations)です。セキュアスコアは、現状を把握し、効果的かつ効率的にセキュリティを向上させることを目的としています。セキュアスコアは、リソースのセキュリティ問題を継続的に評価し、それらを1つのスコアに集約することで、現在のセキュリティ態勢を確認することができます。スコアが高ければ高いほど、特定されたリスクレベルは低くなります。これは、[Microsoft Cloud Security Benchmark](https://docs.microsoft.com/en-us/security/benchmark/azure/baselines/security-center-security-baseline?toc=/azure/security-center/TOC.json)と呼ばれるポリシーによって制御されます。このポリシーは、推奨されるベストプラクティスに基づいて構築され、Center for Internet Security Benchmark の内容も考慮しています。

この機能は 「基本的な CSPM」に含まれており、無償で使用することができます。

「Defender クラウド セキュリティ態勢管理 (CSPM)」はこの機能に加えて規制コンプライアンス（ISO 27001 や PCI-DSS などの標準に基づいてリソースの評価を行う機能）や、攻撃パスの分析などさらなる可視性を得るための機能を利用することができます。

### 基本的な CSPM 機能
- クラウド リソースのセキュリティ構成の継続的な評価
- 構成の誤りと弱点を修正するためのセキュリティに関するレコメンデーション
- セキュリティ スコア

### Defender CSPM 
有償の CSPM プランです。現在はプレビューのステータスで、無償で利用することができます。
基本的な CSPM 機能に加えて、以下の機能を利用することができます。
- [クラウド セキュリティ エクスプローラー](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/how-to-manage-cloud-security-explorer)
- [攻撃パス分析](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/how-to-manage-attack-path)
- [マシンのエージェントレス スキャン](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/enable-vulnerability-assessment-agentless)
- [規制コンプライアンス](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/regulatory-compliance-dashboard)
- [ガバナンス ルール](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/governance-rules)


CSPM 機能の一覧：[基本的な CSPM と クラウド セキュリティ態勢管理 (CSPM) の機能比較](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/concept-cloud-security-posture-management)

## クラウド ワークロード保護 (CWP)

Microsoft Defender for Cloud を構成する2 つめの要素は "強化されたセキュリティ" で 「クラウド ワークロード 保護 (Cloud Workload Protection)」 ツールと呼ばれるものです。

これは様々なものを指しています。"強化されたセキュリティ" は単一の機能ではなく、異なった種類のリソースを保護するために設計された複数の高度なツールを含んでいます。Microsoft Defender for Endpoint による脅威対策と、Just In Time 管理や Adaptive Application Control などの高度なクラウド保護機能が統合されています。複数の異なるセキュリティ機能を統一的に管理する場所を提供し、ハイブリッドクラウドのワークロードに対応する機能を提供します。

- [Defender for Servers](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-servers-introduction)
- [Defender for Containers](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-containers-introduction)
- [データベースの保護](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/quickstart-enable-database-protections)
- [Defender for App Service](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-app-service-introduction)
- [Defender for Storage](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-storage-introduction)
- [Defender for Key Vault](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-key-vault-introduction)
- [Defender for Resource Manager](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-resource-manager-introduction)
- [Defender for DNS](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-dns-introduction)
- [Defender for DevOps](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-devops-introduction)


アラートの一覧：[セキュリティ アラート - リファレンス ガイド](https://learn.microsoft.com/ja-jp/azure/defender-for-cloud/alerts-reference)

## Azure Policy とは?
Azure Policy は、セキュリティ標準による評価を実施し、大規模な環境でもコンプライアンス評価を自動的に行うことができる。ビジネスルールを Azure Policy として定義すると、Azure Policy がリソースのプロパティを定義されたビジネスルールと比較して、全体の状態を把握することができると考えてください。様々なリソースに対して許可する構成、許可しない構成、自動的な監査、許可しない構成のブロックなどを行うことができます。


## コンピューティングに関連する Microsoft Defender XXX
### Microsoft Defender for Cloud
上記の通り Azure が提供する CSPM と CWP の機能です。
過去には Azure Security Center や、Azure Defender (CWP 機能) と呼ばれていました。

### Microsoft Defender for Server
Microsoft Defender for Cloud のサーバー向け CWP 機能です。
2022 年 4 月から Plan 1 と Plan 2 の２つの価格体系で提供されるようになりました。従来の Microsoft Defender for Servers はプラン 2 に該当します。
- Microsoft Defender for Servers プラン 1
    - Microsoft Defender for Endpoint の自動展開、時間単位の課金
- Microsoft Defender for Servers プラン 2
    - (Plan 1 に加えて)
    - 500 MB / 日のログ分析が含まれる (全ノードの平均、テーブルの種類に制限がある)
    - 規制コンプライアンス
    - Just-In-Time VM アクセス
    - Adaptive Application Control 
    - ファイル整合性の監視  
    など

プランの違いの詳細：  
[Microsoft Defender for Servers の概要](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/defender-for-servers-introduction)

[Microsoft Defender for Servers の価格](https://azure.microsoft.com/ja-jp/pricing/details/defender-for-cloud/)


>Microsoft Defender for Endpoint をサーバー OS で動かすことだけを Microsoft Defender for Server と呼ぶわけではありません。

### Microsoft Defender for Endpoint
EDR 機能です。エンタープライズネットワークによる高度な脅威の防止、検出、調査、および応答を支援します。
アンチマルウェア機能は次の項目の Microsoft Defender ウイルス対策 を使用しますが、サードパーティのアンチ マルウェアと組み合わせることもできます。

[Microsoft Defender for Endpoint Plan 1 and Plan 2](https://docs.microsoft.com/ja-jp/microsoft-365/security/defender-endpoint/defender-endpoint-plan-1-2?view=o365-worldwide)

> Microsoft Defender for Endpoint は Microsoft Defender for Cloud に統合されていて、 Microsoft Defender for Server の機能の一部として使われます。既に Defender for Ednpoint のライセンスをお持ちの場合には割引を受けることができます。  

[FAQ : Microsoft Defender for Endpoint のライセンスが既にある場合、Defender for Servers の割引を受けることはできますか?](https://docs.microsoft.com/ja-jp/azure/defender-for-cloud/enhanced-security-features-overview#if-i-already-have-a-license-for-microsoft-defender-for-endpoint-can-i-get-a-discount-for-defender-for-servers)

### Microsoft Defender ウイルス対策
Windows にビルトインされているアンチマルウェア機能です。 定義ファイルに基づいたマルウェアの検出や、一部挙動検知などの機能を備えています。
Azure の標準イメージから作成された Windows OS では既定で有効化されています。Defender for Endpoint を使わずに集中管理を行うためには Microsoft Endpoint Manager (MEM : クライアント OSの管理) や Microsoft Endpoint Configuration Manager (MECM) を使用することができます。

[Windows の Microsoft Defender ウイルス対策](https://docs.microsoft.com/ja-jp/microsoft-365/security/defender-endpoint/microsoft-defender-antivirus-windows?view=o365-worldwide)  
[MEM : Microsoft エンドポイント マネージャーの概要](https://docs.microsoft.com/ja-jp/mem/endpoint-manager-overview)  
[MECM : Configuration Manager とは](https://docs.microsoft.com/ja-jp/mem/configmgr/core/understand/introduction)

> Windows OS でウィルス対策だけを使用したい場合、Microsoft Defender for Server や Defender for Endpoint を有効化する必要はありません。



#### [prev](./welcome.md) | [home](./welcome.md)  | [next](./findings.md)