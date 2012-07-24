=======================================
Sublime Text 2 Package memo
=======================================



.. code-block: php

  echo "hogehoge";

-----------------
私的分類
-----------------
.. toctree::
   :maxdepth: 1

   Program <st2_pkg_prg.rst>
   SCM <st2_pkg_scm.rst>
   Utility <st2_pkg_util.rst>
   未分類 <st2_pkg_unclassified.rst>


-----------------
Package Conrol
-----------------

- Sublime Package Control
	http://wbond.net/sublime_packages/package_control

Install
========

View - Show Console で、 ワンライナー

.. code-block:: python

   import urllib2,os; pf='Package Control.sublime-package'; ipp=sublime.installed_packages_path(); os.makedirs(ipp) if not os.path.exists(ipp) else None; urllib2.install_opener(urllib2.build_opener(urllib2.ProxyHandler())); open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read()); print 'Please restart Sublime Text to finish installation'

.. note:: 
	ワンライナーでインストールするものは、Githubのものより古い場合がある。
	Githubのを使ったほうがProxy周りは対応が入っている
