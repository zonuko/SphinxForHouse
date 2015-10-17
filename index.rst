
Sphinxの紹介
================

.. s6:: styles

    'h1': {position:'absolute',fontSize:'190%',padding:'1.1em'},

話すこと、話さないこと
-------------------------------
* 話すこと
   * Sphinxって何？
   * 特徴
   * Sphinxの利点/ダメな点
   * 自分の環境

* 話さないこと
   * 細かい環境設定
   * 具体的な文法
   * (Pythonのこと) 要望次第

.. s6:: styles

    'h2': {fontSize:'70%'},
    'ul/li[0]': {fontSize:'75%'},
    'ul/li[1]': {fontSize:'75%',marginTop:'1em'},


Sphinxって何？
--------------------------

* Python製ドキュメント生成ツール
* Pythonのドキュメントを書くために誕生

利用例
   * `OpenPNEのAPIリファレンス <http://www.openpne.jp/developer/webapi/ja/index.html>`_
   * `astah Plug-in開発チュートリアル <http://astah.change-vision.com/ja/plugin-tutorial/>`_
   * `OpenCVリファレンス <http://opencv.jp/opencv-2svn/c/>`_


.. s6:: styles

    'h2': {fontSize:'70%'},
    'ul/li': {fontSize:'90%',marginTop:'0.5em'},
    'dl/dt': {fontSize:'80%'},
    'dl/dd/ul/li/a': {fontSize:'80%',marginTop:'0.5em'},

特徴
-------------------------------

* **reStructuredText** と呼ばれるマークアップ言語(拡張子 ``*.rst`` )
* ビルドはPythonで制御(知識は必要ない)
* WikiやTexに近い文法
* 出力は主にHTML、PDF(そのままPDFで出てくるわけではない)
* TocTreeと呼ばれる木構造


.. s6:: styles

    'h2': {fontSize:'70%'},
    'ul/li': {fontSize:'75%',marginTop:'0.5em'},

利点
-------------------------------

* 検索やインデックス作成に優れている: `参考 <http://docs.sphinx-users.jp/>`_
* 拡張性:テーマや今使っているスライド(自分のも見せる)
* ソースの時点で文章の形がわかりやすい
* 木構造で制御するため文章が散らばりにくい(Wikiと違う部分)
* ↑かつソースはバイナリではないのでGitで管理しやすい

.. s6:: styles

    'h2': {fontSize:'70%'},
    'ul/li': {fontSize:'75%',marginTop:'0.5em'},

利点2
-------------------------------

豊富かつ協力なコードシンタックス

.. code-block:: c++

   class test {
   private:
      int a;
      int b;
   };

* ActionScript Ada ANTLR AppleScript Assembly (various) Asymptote Befunge Boo BrainFuck C, C++ C# Clojure CoffeeScript ColdFusion Common Lisp Cython D Delphi Dylan Erlang Fortran Gherkin (Cucumber) GL shaders Haskell (incl. Literate Haskell) Io Java JavaScript LLVM Logtalk Lua Matlab MiniD Modelica Modula-2 MuPad Objective-C Objective-J OCaml PHP Perl PovRay Prolog Python 2.x and 3.x (incl. console sessions and tracebacks) Rebol Redcode Ruby (incl. irb sessions) S, S-Plus, R Scala Scheme Smalltalk Tcl Vala Visual Basic.NET XQuery　`その他 <http://note.sicafe.net/sphinx_memo/codeBlockByPygments.html>`_

.. s6:: styles

    'h2': {fontSize:'70%'},
    'ul/li[0]': {fontSize:'30%',marginTop:'0.5em'}


ダメな点
-------------------------------

* ビルドが必要

.. code-block:: shell

   make html

* メインはHTMLでPDFには正直しにくい
* reST記法を覚える必要がある
*  ``*.docx`` や ``*.xlsx`` にはならない
   →仕事で使うのはこの二種類がメイン(残念ながら・・・)

.. s6:: styles

    'h2': {fontSize:'70%'},
    'ul/li': {fontSize:'75%',marginTop:'0.5em'},

個人的な野望
-------------------------------

* 日報これにしたい
   公開できるように出来たら見る方も簡単なはず。検索性も高い。
* **書く側は記法を覚えなくてはいけない**
   テンプレート用意とか？

* ビルド方法も考える必要あり
   | 書く人全員にビルドしてもらう訳にはいかない。
   | 自動ビルドの方法はいくらでもあるが、実際に置く場合の色々な面倒がありそう・・・

.. s6:: styles

    'h2': {fontSize:'70%'},
    'ul/li': {fontSize:'75%',marginTop:'0.5em'},

自分の環境
-------------------------------
リモートで・・・