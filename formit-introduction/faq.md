# よくある質問(FAQ)

## FormIt について

**FormIt や FormIt Pro はどのような製品ですか?**

FormIt は、建築デザインのための 3D モデリング、ビジュアライゼーション、解析、計算環境です。

FormIt には次のような特徴があります。

* 堅牢なソリッド モデリング エンジンであり、強力なツールとワークフローが建築デザインに最適化されている
* 環境ビジュアライゼーションが強化され、シーンを使用した保存済みのモデル状態などのデザイン オプションを表示できる
* Bing マップを使用した位置、衛星画像、3D 地形
* Autodesk Material Library のマテリアル
* グループ、レイヤ、シーンなどのモデルの構成および表示ツール
* 解析ツールの例
   * ソリッド モデルの診断および修復のための密閉性および背面の検証
   * 太陽と日影
   * 日照解析
   * エネルギー分析
* 統合されているオートデスク製品
   * BIM 360 Docs
   * Insight (エネルギー解析)
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* サポートされるファイル形式
   * 開く/読み込む
      * AXM、DWG、FBX、SAT、STL、OBJ、WSM、SketchUp、Image
   * 書き出す
      * AXM、FBX、OBJ、STL、SAT、DAE、DXF

FormIt は、[iOS](https://itunes.apple.com/jp/app/autodesk-formit-360/id575282599?mt=8) および[ご使用のブラウザ](https://app.formit.autodesk.com/)で無償で使用できます。**FormIt Pro** のサブスクリプションは、[FormIt for Windows](https://formit.autodesk.com/page/download) を使用する場合に必要です。これは、FormIt の最も強力で機能が豊富なバージョンです。**FormIt Pro** のサブスクリプションでは、日照解析やエネルギー解析などの機能を、iOS や Web 上で行うこともできます。**FormIt Pro** は、[Autodesk AEC Collection](https://www.autodesk.co.jp/collections/architecture-engineering-construction/overview) に含まれています。

**FormIt for Android はどうなったのでしょうか?**

FormIt 製品の提供を合理化するために、Android アプリを廃止するという苦渋の決断を下す必要がありました。インストール済み場合は引き続きお使いいただけますが、Play ストアからは入手できなくなりました。

**FormIt の利用を開始する方法を教えてください**

Windows バージョンを実行するには、**FormIt Pro** へのアクセス権が必要です。これは [AEC Collection](https://www.autodesk.co.jp/collections/architecture-engineering-construction/overview) のサブスクリプションに含まれています。オフィスに Revit がある場合は、FormIt にアクセスできる可能性が高いです。[当社の Web サイトから直接 FormIt for Windows をダウンロード](https://formit.autodesk.com/page/download)できます。または Autodesk デスクトップ アプリからもダウンロードできます。

また、Web バージョンは、直接 Web サイト [http://formit.autodesk.com](http://formit.autodesk.com) から無料で実行できます。

iOS バージョンは、Apple App Store から無料でダウンロードできます(iPad のみを対象としています)。

**学生または教育機関の場合は、無償で FormIt Pro を利用できますか?**

はい。FormIt Pro のサブスクリプションは、[Autodesk Education Portal](https://www.autodesk.co.jp/education/edu-software/overview?sorting=featured&page=1) からアクセスできます。

**FormIt の学習方法を教えてください**

[FormIt Primer チュートリアル](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html)から始めることをお勧めします。

FormIt Primer には、現代的な家屋全体を作成する初心者向けのセクションから、Revit と Dynamo も利用する高度な内容のセクションまで用意されています。

また、FormIt Friday ウェビナー シリーズには 20 を超えるビデオもあり、[YouTube チャンネル](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH)からご視聴いただけます。

## Revit と連携する

**FormIt は Revit とどのように連携しますか?**

FormIt は単独で 3D スケッチおよびデザインが可能なアプリケーションですが、[Revit の FormIt アドインを使用](https://formit.autodesk.com/page/formit-revit)すると、簡単に Revit に変換できるデータを作成できます。

**Revit に読み込むと、どうなりますか?**

バージョン 2016 以降、Revit には FormIt データを使用して作業するためのアドインが付属しています。FormIt の AXM ファイルを Revit に読み込む際に、このアドインによってファイル内の各オブジェクトが検査され、API を使用して Revit で再作成されます。既定では、FormIt 内のすべての要素はマスとして分類されます。

FormIt コンバータは、[直接形状の API](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/JPN/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html) を使用して、Revit で各マス オブジェクトを取得してマス ファミリを作成します。

直接形状は、IFC ワークフローで使用される編集不可能なオブジェクトです。編集はできませんが、FormIt と Revit の間でマテリアル テクスチャをすべて転送できるという明確な利点があります。FormIt から Revit へのワークフローの詳細について説明する[チュートリアルはこちら](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html)にあります。

**FormIt で壁や床などの Revit システム ファミリを作成できますか?**

直接作成することはできません。上述のように、各オブジェクトは既定でマス カテゴリとなります。壁、床などを作成するには、コンバータ アドインを使用してモデルを Revit に読み込み、ネイティブの Revit ツールを使用して基礎となるマス モデルからシステム ファミリを作成する必要があります。

**Revit からデータを FormIt に戻すことはできますか?**

はい。データを FormIt に再度読み込むには、Revit ファイルのすべてまたは可能な場合は一部を SAT ファイル形式に書き出します。__通常、Revit データのすべてを FormIt に送信する必要はありません。代わりに、SAT に保存する前に、床と壁といった最小データ)のみを含むようにフィルタしたビューを Revit で作成します。

## 他のアプリケーションと連携する

**既定のファイル形式が「.AXM」であるのはなぜですか?**

FormIt の公式の名前が決まる前、社内で使われていたコードネームは XModeler でした。そのため、作成したファイル形式は Autodesk X Modeler、略して AXM となりました。

**FormIt ではどの種類の 3D 形式を読み込むことができますか?**

* Windows: AXM、DWG、FBX、OBJ、SAT、SKP、STL
* Web: OBJ、STL
* iOS: OBJ、STL、SAT

**FormIt ではどの種類の形式を書き出すことができますか?**

* Windows: FBX、OBJ、SAT、STL、DAE、DXF
* Web: OBJ、SAT、STL
* iOS: OBJ

**FormIt は Dynamo とどのように連携しますか?**

計算設計ワークフローを作成するための [FormIt と Dynamo の連携についてはこちら](https://formit.autodesk.com/page/formit-dynamo)をご覧ください。

**FormIt の SketchUp との違いは何ですか?**

* [**Revit との相互運用性**](../tool-library/revit.md)が向上
* 計算設計のための[**Dynamo との統合**](../tool-library/dynamo.md)
* [**日照解析**](../tool-library/solar-analysis.md)および Autodesk Insight による[**エネルギー解析**](../tool-library/energy-analysis.md)のネイティブ ツール
* 高度なモデリング操作を可能にする、より堅牢なソリッド モデリング カーネル
* [**スイープ、かぶり、ロフト**](../tool-library/cover-sweep-loft.md)、ソリッドをオフセット/シェル化、3D ブレンド/フィレット、[**面を平坦化**](../tool-library/flatten-face.md)などの、ネイティブの高度なモデリング ツール
* 複数の[**断面平面**](../tool-library/section-planes.md)を表示可能
* [**密閉性に関する問題を表示、および背面を表示**](../tool-library/visual-styles.md)などの診断ツール
* 選択または表示されている内容に基づいて[**モデルの一部を書き出す**](../tool-library/export-data.md)
* ネイティブの OBJ、SAT、STL の書き出し

**SketchUp のキーボード ショートカットを使用できますか?**

はい。FormIt for Windows には、完全に編集可能なキーボード マップがあります。多くの一般的な SketchUp のショートカットは既定で存在しますが、[編集] &gt; [基本設定]メニューで編集できます。

**DWG ファイルを使用できますか?**

はい。FormIt は 2D および 3D の DWG ファイルを読み込みます。

## 一般的なサポートの質問

**サポートを利用するにはどうすればよいですか?**

オートデスク認定販売パートナーにお問い合わせいただくか、[FormIt フォーラム](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=ja)をご覧ください。そこではまず質問を検索することをお勧めします。まだ回答がない場合は、新しいトピックを投稿すると、FormIt チームが回答します。

**ログインできない場合はどうすればよいですか?**

* この[フォーラムの投稿\(英語\)](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=ja)には、一般的なログインの問題が記載されています
* 切り替え可能なグラフィックス プロセッサ(GPU)を搭載した PC を使用する場合は、FormIt が常により高性能な GPU を使用するようにすることが重要です。[AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) および [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1) の場合の手順はこちらをご覧ください(英語)

**Insight のエネルギー解析が失敗した場合はどうすればよいですか?**

Insight のエネルギー解析でエラーが報告された場合や、結果が返されない場合は、[Insight のエネルギー解析のページ(英語)](https://formit.autodesk.com/page/formit-insight)で、一般的なトラブルシューティングのヒントを参照してください。

