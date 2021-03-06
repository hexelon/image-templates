---

copyright:
  years: 2014, 2018
lastupdated: "2018-04-04"

subcollection: image-templates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:tip: .tip}


# ユーザー自身の OS ライセンスまたはサブスクリプションの使用

VHD イメージを使用してイメージ・テンプレートを作成するとき、[Red Hat Cloud Access ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://www.redhat.com/en/technologies/cloud-computing/cloud-access) サブスクリプションからユーザー自身の RHEL オペレーティング・システムのライセンスを指定したり、Microsoft エンタープライズ契約から Windows ライセンスを指定したりすることを選択できます。
{:shortdesc}

ユーザー自身のライセンスを使用していることを示す {{site.data.keyword.BluSoftlayer_full}} のイメージをデプロイする場合、以下のサポート条件があります。
* {{site.data.keyword.IBM_notm}} は、ハイパーバイザー、インスタンスのプロビジョニング、イメージのインポート、イメージのリブート、OS の再ロード、イメージの取り込みに関するサポートを提供します。
* イメージ自体のサポートは、オペレーティング・システム・ライセンスの購入元の企業が提供します。 {{site.data.keyword.IBM_notm}} は、イメージに関するサポートは提供しません。

ユーザー自身のライセンスをイメージに提供する場合、イメージには以下の制約事項が適用されます。
* イメージはプライベート・イメージです。 公開して共有することはできません。
* イメージに、ソフトウェアのアドオンを組み込むことはできません。 イメージをプロビジョンした後に追加のソフトウェアを追加する必要があります。

## Red Hat Cloud Access の使用
Red Hat Enterprise Linux クラウド・プロバイダーとしての弊社の認定について詳しくは、[Infrastructure as a Service (Iaas) ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://access.redhat.com/ecosystem/cloud-provider/2262101) を参照してください。

## ユーザー自身の Windows ライセンスの使用
以下のオペレーティング・システムがサポートされています。
* Windows Server 2016
* Windows Server 2012
* Windows Server 2012 R2

既存の Windows ライセンスの資格、または報告書条件の理解について質問がある場合は、Microsoft の担当者に連絡してください。 ユーザー自身の Windows ライセンスを使用していることを指定するイメージ・テンプレートを作成するときは、専用ホストにそのイメージをプロビジョンする必要があります。 ユーザー自身の Windows ライセンスを使用していることを示すイメージを使用するときは、ホストに自動的に割り当てられるパブリック・インスタンスや専用インスタンスをプロビジョンすることはできません。 さらに、ユーザー自身のライセンスを使用していることを指定する Windows イメージ・テンプレートを作成または更新するときは、Windows イメージを cloud-init イメージにすることはできません。

## ユーザー自身のライセンスを指定するイメージのインポート

VHD イメージをインポートし、オペレーティング・システムに関してユーザー自身のライセンスまたはサブスクリプションを提供することを指定できます。

イメージ・テンプレートの「イメージのインポート」ページにアクセスし、ユーザー自身のライセンスまたはサブスクリプションを使用するように VHD イメージにマークを付けるには、以下の手順を実行します。
1. **「デバイス」**メニューから、**「管理」>「イメージ」**を選択します。
2. **「イメージのインポート」**タブをクリックします。
3. VHD イメージをインポートするために必要な情報を入力し、**「オペレーティング・システム」**ドロップダウン・ボックスの近くに表示されている**「自分のライセンス (Your License)」**チェック・ボックスを選択します。イメージのインポートについて詳しくは、[イメージの準備およびインポート](/docs/infrastructure/image-templates?topic=image-templates-preparing-and-importing-images)を参照してください。

## ユーザー提供の OS ライセンスを指定するようイメージ・テンプレートを更新

既存の VHD イメージ・テンプレートがある場合、オペレーティング・システムに関してユーザー自身のライセンスまたはサブスクリプションを提供することを指定できます。

イメージ・テンプレートにアクセスし、そのテンプレートでユーザー自身のライセンスまたはサブスクリプションを使用することを指定するには、以下の手順を実行します。
1. **「デバイス」**メニューから、**「管理」>「イメージ」**を選択します。
2. テンプレートのリストから、更新するイメージ・テンプレート名をクリックします。
3. 「イメージ・テンプレートの詳細」ページで、**「OS ライセンス」**ヘッダーの下の**「ユーザー提供 (User Provided)」**チェック・ボックスを選択し、**「更新」**をクリックします。
