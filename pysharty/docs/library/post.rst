:class:`pysharty.Post` – soyjak.party Post
=======================================

:class:`pysharty.Post` allows for standard access to a soyjak.party post.

Example
-------

Here is a sample application that grabs and prints :class:`pysharty.Thread` and :class:`pysharty.Post` information:

.. code-block:: python

    # credits to Anarov for improved example
    from __future__ import print_function
    import pysharty

    # get the board we want
    board = pysharty.Board('soy')

    # select the first thread on the board
    all_thread_ids = board.get_all_thread_ids()
    first_thread_id = all_thread_ids[0]
    thread = board.get_thread(first_thread_id)

    # print thread information
    print(thread)
    print('Sticky?', thread.sticky)
    print('Closed?', thread.closed)
    print('Replies:', len(thread.replies))

    # print topic post information
    topic = thread.topic
    print('Topic Repr', topic)
    print('Postnumber', topic.post_number)
    print('Timestamp', topic.timestamp)
    print('Datetime', repr(topic.datetime))
    print('Subject', topic.subject)
    print('Comment', topic.comment)
    
    # file information
    for f in first_thread.file_objects():
        print('Filename', f.filename)
        print('  Filemd5hex', f.file_md5_hex)
        print('  Fileurl', f.file_url)
        print('  Thumbnailurl', f.thumbnail_url)
        print()

Basic Usage
-----------

.. autoclass:: pysharty.Post

    Post objects are not instantiated directly, but through a :class:`pysharty.Thread` object with an attribute like :attr:`pysharty.Thread.all_posts`.
