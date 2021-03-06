.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the CubeMap.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_CubeMap:

CubeMap
=======

**Inherits:** :ref:`Resource<class_resource>` **<** :ref:`Reference<class_reference>` **<** :ref:`Object<class_object>`

**Category:** Core

Brief Description
-----------------

A CubeMap is a 6 sided 3D texture.

Member Functions
----------------

+----------------------------+-----------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`      | :ref:`get_height<class_CubeMap_get_height>` **(** **)** const                                                   |
+----------------------------+-----------------------------------------------------------------------------------------------------------------+
| :ref:`Image<class_image>`  | :ref:`get_side<class_CubeMap_get_side>` **(** :ref:`int<class_int>` side **)** const                            |
+----------------------------+-----------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`      | :ref:`get_width<class_CubeMap_get_width>` **(** **)** const                                                     |
+----------------------------+-----------------------------------------------------------------------------------------------------------------+
| void                       | :ref:`set_side<class_CubeMap_set_side>` **(** :ref:`int<class_int>` side, :ref:`Image<class_image>` image **)** |
+----------------------------+-----------------------------------------------------------------------------------------------------------------+

Member Variables
----------------

  .. _class_CubeMap_flags:

- :ref:`int<class_int>` **flags** - The render flags for the ``CubeMap``. See the ``FLAG\_\*`` constants for details.

  .. _class_CubeMap_lossy_storage_quality:

- :ref:`float<class_float>` **lossy_storage_quality** - The lossy storage quality of the ``CubeMap`` if the storage mode is set to STORAGE_COMPRESS_LOSSY.

  .. _class_CubeMap_storage_mode:

- :ref:`Storage<enum_cubemap_storage>` **storage_mode** - The ``CubeMap``'s storage mode. See ``STORAGE\_\*`` constants.


Enums
-----

  .. _enum_CubeMap_Flags:

enum **Flags**

- **FLAG_MIPMAPS** = **1** --- Generate mipmaps, to enable smooth zooming out of the texture.
- **FLAG_REPEAT** = **2** --- Repeat (instead of clamp to edge).
- **FLAG_FILTER** = **4** --- Turn on magnifying filter, to enable smooth zooming in of the texture.
- **FLAGS_DEFAULT** = **7** --- Default flags. Generate mipmaps, repeat, and filter are enabled.

  .. _enum_CubeMap_Storage:

enum **Storage**

- **STORAGE_RAW** = **0** --- Store the ``CubeMap`` without any compression.
- **STORAGE_COMPRESS_LOSSY** = **1** --- Store the ``CubeMap`` with strong compression that reduces image quality.
- **STORAGE_COMPRESS_LOSSLESS** = **2** --- Store the ``CubeMap`` with moderate compression that doesn't reduce image quality.

  .. _enum_CubeMap_Side:

enum **Side**

- **SIDE_LEFT** = **0** --- Identifier for the left face of the ``CubeMap``.
- **SIDE_RIGHT** = **1** --- Identifier for the right face of the ``CubeMap``.
- **SIDE_BOTTOM** = **2** --- Identifier for the bottom face of the ``CubeMap``.
- **SIDE_TOP** = **3** --- Identifier for the top face of the ``CubeMap``.
- **SIDE_FRONT** = **4** --- Identifier for the front face of the ``CubeMap``.
- **SIDE_BACK** = **5** --- Identifier for the back face of the ``CubeMap``.


Description
-----------

A 6-sided 3D texture typically used for faking reflections. It can be used to make an object look as if it's reflecting its surroundings. This usually delivers much better performance than other reflection methods.

Member Function Description
---------------------------

.. _class_CubeMap_get_height:

- :ref:`int<class_int>` **get_height** **(** **)** const

Returns the ``CubeMap``'s height.

.. _class_CubeMap_get_side:

- :ref:`Image<class_image>` **get_side** **(** :ref:`int<class_int>` side **)** const

Returns an :ref:`Image<class_image>` for a side of the ``CubeMap`` using one of the ``SIDE\_\*`` constants or an integer 0-5.

.. _class_CubeMap_get_width:

- :ref:`int<class_int>` **get_width** **(** **)** const

Returns the ``CubeMap``'s width.

.. _class_CubeMap_set_side:

- void **set_side** **(** :ref:`int<class_int>` side, :ref:`Image<class_image>` image **)**

Sets an :ref:`Image<class_image>` for a side of the ``CubeMap`` using one of the ``SIDE\_\*`` constants or an integer 0-5.


