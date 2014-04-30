pptable
=======

Prints data as a table assuming that data is a list of dictionaries

At the moment it assumes that dictionaries are flat (values are primitives, not a dictionary/list)


example usage
=============

install::

    pip install pptable


code::

    from pptable import pptable
    data = [{'slug': u'ams1', 'name': u'Amsterdam 1', 'region_id': 2},
    {'slug': u'sfo1', 'name': u'San Francisco 1', 'region_id': 3},
    {'slug': u'nyc2', 'name': u'New York 2', 'region_id': 4},
    {'slug': u'ams2', 'name': u'Amsterdam 2', 'region_id': 5},
    {'slug': u'sgp1', 'name': u'Singapore 1', 'region_id': 6}]

    pptable(data)

    ----------------------------------
    region_id  name             slug
    ----------------------------------
            2  Amsterdam 1      ams1
            3  San Francisco 1  sfo1
            4  New York 2       nyc2
            5  Amsterdam 2      ams2
            6  Singapore 1      sgp1


    headers = ['slug', 'name']
    pptable(data, headers=headers)

    -----------------------
    slug  name
    -----------------------
    ams1  Amsterdam 1
    sfo1  San Francisco 1
    nyc2  New York 2
    ams2  Amsterdam 2
    sgp1  Singapore 1
