.. _contentselector_type:

ContentSelector
---------------

References to other content are specified by this input type.

.. literalinclude:: code/contentselector.xml
   :language: xml

common fields
  All Input Types have these :ref:`Common Fields <input_types_common_fields>`

relationship
  This setting defines the name of which relationship-type to use. Default is system:reference.

allowContentType
  This is used to limit the content types that may be selected for this input. If you only specify content type name - `citation` - the current app is automatically presumed. You can add another app's name - `my.other.app` - followed by a colon (:) and the content type name `:quote` to allow content from other apps, like so: `my.other.app:quote`. Use one setting for each content-type.

allowPath
  This is used to limit the path of the content that may be selected for this input. The site on which the content exists, can be wildcarded with ${site} Use one setting for each path expression.

.. literalinclude:: code/allowpath-samples.xml
    :language: xml
