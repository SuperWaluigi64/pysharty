:class:`pysharty.Board` – soyjak.party Boards
==========================================

:class:`pysharty.Board` provides access to a soyjak.party board including checking if threads exist, retrieving appropriate :class:`pysharty.Thread` objects, and returning lists of all the threads that exist on the given board.

Example
-------

Here is a sample application that grabs and uses Board information::

    from __future__ import print_function
    import pysharty

    board = pysharty.Board('soy')
    thread_ids = board.get_all_thread_ids()
    str_thread_ids = [str(id) for id in thread_ids]  # need to do this so str.join below works
    print('There are', len(all_ids), 'active threads on /soy/:', ', '.join(str_thread_ids))

Basic Usage
-----------

.. autoclass:: pysharty.Board

Methods
-------

    .. automethod:: pysharty.Board.__init__

    .. automethod:: pysharty.Board.thread_exists

    .. automethod:: pysharty.Board.get_thread

    .. automethod:: pysharty.Board.get_threads

    .. automethod:: pysharty.Board.get_all_threads

    .. automethod:: pysharty.Board.get_all_thread_ids

    .. automethod:: pysharty.Board.refresh_cache

    .. automethod:: pysharty.Board.clear_cache
