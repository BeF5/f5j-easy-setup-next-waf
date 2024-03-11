.. F5 BIG-IP Next WAF セットアップガイド documentation master file, created by F5 Japan in 2024.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


F5 BIG-IP Next WAF v20.0 簡単セットアップガイド
==============================================
最終更新日: 2024年x月xx日


はじめに
==============================================
このページでは、これらのオフィシャルなドキュメントの補足となる資料や、複数の機能を組合せてソリューションを実現する方法をご紹介いたします。
F5のオフィシャルなドキュメントはこちらにございます。

- MyF5: https://my.f5.com/manage/s/
- F5 Cloud Docs: https://clouddocs.f5.com/
- F5 DevCentral（コミュニティ）: https://community.f5.com/

コンテンツ
==============================================
こちらのページでは、以下の内容をご紹介しております。

- 本セットアップガイドにて、F5 BIG-IP Next WAF（以下、Next WAF）のポリシーの設定方法についてご案内します。
- Next WAFは、Webアプリケーションファイアウォールです。
- Next WAF によって、Web アプリケーション特有の攻撃に対する防御が可能となります。
- Bot対策機能、L7レベルのDoS攻撃に対する防御機能も兼ね備えています。
- 本ガイドでは、Next WAFをご購入いただいてすぐにWAFを導入頂けるように、必要となる典型的なセットアップ手法を、豊富なスクリーンショットを交えて解説します。（実際は環境構成にあった設定値を設定して下さい。）
- 本ガイドでは、F5 Japanにおけるハンズオントレーニングのコースでも利用しております。




.. important:: View the agile course on scrum basics

- View `these slides to dive deeper into Agile Basics <_static/sample.pdf>`_. 


.. note::
   本ドキュメントの手順は、F5 UDF (Universal Demonstration Framework)というラボ環境での実施を前提に書かれています。
   UDF以外での環境で利用される場合は、IPアドレス等は環境に合わせて読み替えてください。


.. toctree::
   :numbered:
   :titlesonly:
   :caption: 目次:
   :glob:

   content*/content*
