Nihonkoku Kenpo
===============

Github Page : http://esehara.github.com/NihonkokuKenpo/

What is this?
-------------

This is the THE CONSTITUTION OF JAPAN (Language : Japanese) Repository.


How do I this?
-------------- 

使い方は特に考えていません。Gitの練習にどうぞ。

About
-----

現在、フォルダは下の用に構成されています。

* src
* usr

srcは、元の日本国憲法が入っているデフェクトリです。
usrは他のGithubユーザーが作成した日本国憲法改正草案が入る予定です。


Git
---

使い方はGithubの使い方に準拠します。簡単な使い方としては、上のForkを使用して、自分のGitにCloneしましょう。

    $ git clone git@github.com:YOUR_USERNAME/NihonkokuKenpo.git
    $ git branch dev-YOURNAME-Kenpo
    $ git checkout dev-YOURNAME-kenpo

　上記のbranch、checkoutに関しては、 `checkout -b dev-YOURNAME-Kenpo` で代用が可能です。ここから改正案を作成していきます。もちろん、master配下でRewriteすることも可能ですが、できることならばあまりやらないほうがいいでしょう。Rewrite内容で、Branchを使用することを推奨します。ある程度、書き直しが進んだら、次のようにMergeします。

    $ git checkout master
    $ git merge dev-YOURNAME-Kenpo

　これで、masterに、dev-YOURNAME-Kenpoで作った内容が反映されます。このような形で、自分の日本国憲法に書き直していきましょう。

Pull Requestの方針について
--------------------------

　Masterに対する、Pull Requestに関しては、`usr/YOURNAME/` のみに変更があった場合に、Mergeされます。

　Master branchにおいて、srcは、記法及び表現において修正が認められるさいにおいてのみ、変更が行われます。srcを弄るような作りは想定していません。

　しかし、GitらしくBranchを作りたい人たちに関しては、それらを保管する新しいBranchを作り、そこにMergeします。
