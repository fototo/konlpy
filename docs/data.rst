Data
====

.. _tags:

Tags
----

.. seealso::
    `Korean POS tags comparison chart <https://docs.google.com/spreadsheets/d/1OGAjUvalBuX-oZvZ_-9tEfYD2gQe7hTGsgUpiiBSXI8/edit#gid=0>`_

        Compare POS tags between several Korean analytic projects. (In Korean)


.. _dictionaries:

Dictionaries
------------

Dictionaries are used for :doc:`morph`,
and are built with :ref:`corpora`.

:py:mod:`.hannanum` *system dictionary*
'''''''''''''''''''''''''''''''''''''''

A dictionary created with the KAIST corpus. (4.7MB)

Located at ``./konlpy/java/data/kE/dic_system.txt``.
Part of this file is shown below.::

    ...
    나라경제        ncn
    나라기획        nqq
    나라기획회장    ncn
    나라꽃  ncn
    나라님  ncn
    나라도둑        ncn
    나라따르        pvg
    나라링링프로덕션        ncn
    나라말  ncn
    나라망신        ncn
    나라박물관      ncn
    나라발전        ncpa
    나라별  ncn
    나라부동산      nqq
    나라사랑        ncn
    나라살림        ncpa
    나라시  nqq
    나라시마        ncn
    ...

You can add your own terms, modify ``./konlpy/java/data/kE/dic_user.txt``.

:py:mod:`.kkma` *system dictionary*
'''''''''''''''''''''''''''''''''''

A dictionary created with the Sejong corpus. (32MB)

It is included within the Kkma ``.jar`` file,
so in order to see dictionary files, check out the `KKMA's mirror <https://github.com/e9t/kkma/tree/master/dic>`_.
Part of ``kcc.dic`` is shown below.::

    아니/IC
    후우/IC
    그래서/MAC
    그러나/MAC
    그러니까/MAC
    그러면/MAC
    그러므로/MAC
    그런데/MAC
    그리고/MAC
    따라서/MAC
    하지만/MAC
    ...

:py:mod:`.mecab` *system dictionary*
''''''''''''''''''''''''''''''''''''

A CSV formatted dictionary created with the Sejong corpus. (346MB)

The compiled version is located at ``/usr/local/lib/mecab/dic/mecab-ko-dic`` (or the path you assigned during installation),
and you can see the original files in the `source code <https://bitbucket.org/eunjeon/mecab-ko-dic/src/ce04f82ab0083fb24e4e542e69d9e88a672c3325/seed/?at=master>`_.
Part of ``CoinedWord.csv`` is shown below.::

    가오티,0,0,0,NNG,*,F,가오티,*,*,*,*,*
    갑툭튀,0,0,0,NNG,*,F,갑툭튀,*,*,*,*,*
    강퇴,0,0,0,NNG,*,F,강퇴,*,*,*,*,*
    개드립,0,0,0,NNG,*,T,개드립,*,*,*,*,*
    갠소,0,0,0,NNG,*,F,갠소,*,*,*,*,*
    고퀄,0,0,0,NNG,*,T,고퀄,*,*,*,*,*
    광삭,0,0,0,NNG,*,T,광삭,*,*,*,*,*
    광탈,0,0,0,NNG,*,T,광탈,*,*,*,*,*
    굉천,0,0,0,NNG,*,T,굉천,*,*,*,*,*
    국을,0,0,0,NNG,*,T,국을,*,*,*,*,*
    귀요미,0,0,0,NNG,*,F,귀요미,*,*,*,*,*
    ...

To add your own terms, see `here <https://bitbucket.org/eunjeon/mecab-ko-dic/src/ce04f82ab0083fb24e4e542e69d9e88a672c3325/final/user-dic/?at=master>`_.


.. note::

    You can add new words either to the system dictionaries or user dictionaries. However, there is a slight difference in the two choices.:

    - *Adding to the system dictionary*: When dictionary updates are not frequent, when you do not want to drop the analysis speed.
    - *Adding to the user dictionary*: When dictionary updates are not frequent, when you do not have ``root`` access.
