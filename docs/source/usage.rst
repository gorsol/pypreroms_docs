Usage
=====

.. _installation:

Installation
------------

To use PYpreROMS, first install it using conda:

.. code-block:: console

   (.venv) $ conda install -c conda-forge pypreroms

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import pypreroms
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

