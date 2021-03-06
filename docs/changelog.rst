Change logs
===========

`Version 0.3.2 <https://github.com/e9t/konlpy/releases/tag/v0.3.1>`_
----------------------------------------------------------------

Released on Sep 4, 2014.

- Fixed JPype class loading error for Mac OS X
    - Contributed by `combacsa <https://github.com/combacsa>`_
    - JPype is not compatible with JDK >= 1.7 in Mac OS X
- Fixed Kkma memory error for Mac OS X
    - Contributed by `combacsa <https://github.com/combacsa>`_
    - `java.lang.OutOfMemoryError` in Mac OS X if heap memory is to small

`Version 0.3.1 <https://github.com/e9t/konlpy/releases/tag/v0.3.1>`_
----------------------------------------------------------------

Released on Sep 4, 2014.

- Added MeCab installer script
- Fixed Morph modules to handle strings with whitespaces only
- Fixed data inclusion error for Hannanum
- Modified tagger filenames with underscore prefixes
- Modified concordance function not to print results by default
- Modified Hannanum `morph` method to `analyze`
- Uploaded `KoNLPy to PyPI <https://pypi.python.org/pypi/konlpy>`_

`Version 0.3.0 <https://github.com/e9t/konlpy/releases/tag/v0.3.0>`_
----------------------------------------------------------------

Released on Aug 25, 2014.

- Changed API by automatically initializing JVM for Hannanum, Kkma
- Added Kkma module with Kkma 2.0
- Added documents using Sphinx and Read the Docs
- Added license: GPL v3 or above
- Added pretty print function for Unicode
- Added noun extractor to Mecab
- Fixed Hannanum, Kkma module bug where it couldn't handle empty input strings

.. warning::

    The versions below do not have documents available, and are not backwards-compatible.

`Version 0.2 <https://github.com/e9t/konlpy/releases/tag/v0.2>`_
----------------------------------------------------------------

Released on Aug 1, 2014.

- Changed API by explicitly initializing JVM for Hannanum
- Added Mecab module with MeCab-0.996-ko-0.9.1
- Added unit tests
- Added test automation with Travis CI 
- Fixed Hannanum module parsing error when '/', '+' are in text
- Fixed Hannanum module text indexing error (where results get truncated)

`Version 0.1 <https://github.com/e9t/konlpy/releases/tag/v0.1>`_
----------------------------------------------------------------

Released on Jun 15, 2014.
Initial release of KoNLPy.

- Inspired by Heewon Jeon's `KoNLP <https://github.com/haven-jeon/KoNLP>`_ project, a wrapper of the Hannanum analyzer for R. The name KoNLPy, comes from this project.
- Added Hannanum module with JHannanum 0.8.3
