:class:`pysharty.File` – soyjak.party File
=======================================

:class:`pysharty.Post` allows for standard access to a soyjak.party file. This provides programs with a complete File object that contains all metadata about the soyjak.party file, and makes migration easy if soyjak.party ever makes multiple files in one Post possible (as 8chan does).

Basic Usage
-----------

.. autoclass:: pysharty.File

    File objects are not instantiated directly, but through a :class:`pysharty.File` object with an attribute like :attr:`pysharty.Post.first_file`.