:class:`pysharty.Thread` – soyjak.party Threads
============================================

:class:`pysharty.Thread` allows for standard access to a soyjak.party thread, including listing all the posts in the thread, information such as whether the thread is locked and stickied, and lists of attached file URLs or thumbnails.

Basic Usage
-----------

.. autoclass:: pysharty.Thread

Methods
-------

    Thread objects are not instantiated directly, but instead through the appropriate :class:`pysharty.Board` methods such as :meth:`pysharty.Board.get_thread`.

    .. automethod:: pysharty.Thread.files

    .. automethod:: pysharty.Thread.thumbs

    .. automethod:: pysharty.Thread.filenames

    .. automethod:: pysharty.Thread.thumbnames

    .. automethod:: pysharty.Thread.update

    .. automethod:: pysharty.Thread.expand
