pptable
=======

Prints data as a table assuming that data is a list of dictionaries

At the moment it assumes that dictionaries are flat (values are primitives, not a dictionary/list)


example usage
=============

pip install pptable


code::

    from pptable import pptable
    data = [{'slug': u'ams1', 'name': u'Amsterdam 1', 'region_id': 2},
    {'slug': u'sfo1', 'name': u'San Francisco 1', 'region_id': 3},
    {'slug': u'nyc2', 'name': u'New York 2', 'region_id': 4},
    {'slug': u'ams2', 'name': u'Amsterdam 2', 'region_id': 5},
    {'slug': u'sgp1', 'name': u'Singapore 1', 'region_id': 6}]

    pptable(data)

    headers = ['slug', 'name']
    pptable(data, headers=headers)

