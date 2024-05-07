脆弱なウェブサーバーをデプロイ
=========================================================

UDF画面上部タブの"DEPLOYMENT"をクリックし、BIG-IP Next Central Managerインスタンスの"ACCESS" > "GUI" を選択します。

   .. image:: images/Picture01.png
      :scale: 60%
      :align: center
   |

BIG-IP Next CM GUIへのログイン、ログインプロンプトが表示されたら、ユーザ名/パスワードを入力してログインします。
   - ユーザー名/パスワード:
   - **admin/Welcome123!**

   .. image:: images/Picture2.png
      :scale: 60%
      :align: center
   |       

ログインすると次のようなホーム画面から"Manage Applications"をクリックします。

   .. image:: images/Picture3.png
      :scale: 40%
      :align: center
   |       

“Add Application”をクリックして、新規アプリケーション作成します。

   .. image:: images/Picture4.png
      :scale: 40%
      :align: center
   |       

- Application Service Name:
   - **HTTP-DVWA**　（任意の名前）
- What kind of Application:
   - **Standard**　を選択
- **“Start Creating”** を二回クリック


   .. image:: images/Picture5.png
      :scale: 40%
      :align: center
   |       

“Pools”を選択し、“Create”をクリックしてpoolの名前とポート番号を入力します。

- Pool Name:
   - **dvwa_pool**
- Server Port:
   - **80**
- Load-Balancing Mode:
   - **round-robin**
- Monitor Type:
   - **http**

   .. image:: images/Picture6.png
      :scale: 40%
      :align: center
   |       

"Virtual Servers"のtabに戻り、以下内容を入力します。

- Virtual Server Name:
   - **DVWA-VS**
- Pool:
   - **dvwa_pool**　(先ほど作成されましたpoolを選択)
- **“Review & Deploy”** をクリック

   .. image:: images/Picture7.png
      :scale: 40%
      :align: center
   |       

次の画面から"Start Adding"をクリック、“big01.f5lab.local” のチェックボックスをチェックしてから"Add to List"をクリックします。

   .. image:: images/Picture8.png
      :scale: 40%
      :align: center
   |       

次のDeploy画面で、Virtual ServerのIPとPool memberを設定します。

- Virtual Address:
   - **10.1.10.100**
- Membersの下矢印を展開し、 “+Pool Members” をクリック

   .. image:: images/Picture9.png
      :scale: 40%
      :align: center
   |       

“+Add Row” を２回クリックpool memberを作成します。

- Name:
   - **dvwa_server **
- IP Address:
   - **10.1.20.101**
- 入力後、 ”Save” をクリック

   .. image:: images/Picture10.png
      :scale: 40%
      :align: center
   |       

ログインすると次のようなホーム画面から"Manage Applications"をクリックします。

   .. image:: images/Picture11.png
      :scale: 40%
      :align: center
   |       

ログインすると次のようなホーム画面から"Manage Applications"をクリックします。

   .. image:: images/Picture12.png
      :scale: 40%
      :align: center
   |       

ログインすると次のようなホーム画面から"Manage Applications"をクリックします。

   .. image:: images/Picture13.png
      :scale: 40%
      :align: center
   |       





