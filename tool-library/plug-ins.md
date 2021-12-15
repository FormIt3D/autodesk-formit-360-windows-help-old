# プラグイン

Plugin Manager を使用して、FormIt チームから便利なプラグインをインストールするか、[**独自の FormIt プラグインを構築する**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**方法を学びます。**

#### FormIt Plugin Manager

FormIt Plugin Manager は、Formit のプラグインを見つけたり管理を行うためのハブとして機能します。

FormIt がインターネットにアクセスできる限り、Plugin Manager は FormIt の起動時に自動的にロードされます。

Plugin Manager にアクセスするには、アプリケーション ウィンドウの右側にあるプラグのアイコンをクリックします。

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### Plugin Manager は、各種プラグインをさまざまなタイプに分類しています。

* **インストール済みのプラグイン**
* **推奨プラグイン**
   * FormIt の主要機能を拡張し、新しいワークフローを実現するために FormIt チームが推奨するプラグイン。
   * コミュニティで開発されたプラグインは、FormIt チームによって承認された後に、ここに表示されます。今後、ここに詳細が記載されます。
* **パブリック プラグイン**
   * コミュニティによってビルドされたものの、FormIt チームがまだ確認や承認を行っていないプラグイン。

#### Plugin Manager は、展開/折りたたみ可能なインタフェースを使用して設計されているため、プラグインとそのリポジトリの管理が簡単にできます。

* **プラグインを管理する:**
   * プラグイン名をクリックすると、その説明が表示されます。
   * スイッチを切り替えて、インストールやアンインストールを行います。
      * プラグインは、そのタイプに応じて、アプリケーションの上部のツールバー、右側のパネル、または中央のダイアログとして表示されます。
* [独自のプラグインを開発する](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)場合は、下部のフィールドにプライベート URL を入力して、[+]ボタンをクリックします。

![The FormIt Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### プラグインの仕組み

* プラグインは Web ベースで、FormIt for Windows と FormIt for Web で利用できます。
* プラグインは一連のファイルとフォルダで構成され、GitHub、またはユーザ独自で構築した場合はローカル サーバにホストされています。
* ローカルにホストされていない外部のプラグインを最初にロードする際には、インターネット接続が必要です。次の点に注意してください。
   * FormIt の起動時にインターネット接続が検出されない場合、外部プラグインはロードされません。
   * ロードした後、一部の外部プラグインはそのセッションの間はオフライン モードで作業を続行できますが、接続が回復するまで中断するプラグインもあります。
   * 外部プラグインは実行のたびにサーバ上の最新のコードをロードするため、作成者が変更をプッシュするたびに機能が更新されます。
* プラグインは非同期的にロードされます。つまり、FormIt インタフェースのプラグインの順序は、セッションごとに変更される場合があります。
* Plugin Manager は、インストールされたリポジトリとプラグインを保存するために、Windows のレジストリ キーを使用します。
   * Plugin Manager を既定にリセットする必要がある場合は、次のレジストリ キーを削除します。
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * これにより、ユーザが追加したすべてのリポジトリとプラグインがアンインストールされ、Plugin Manager がリセットされて内蔵リポジトリとプラグインのみが含まれるようになります。

