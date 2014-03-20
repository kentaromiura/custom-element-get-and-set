custom-element-get-and-set
==========================

custom web component for setting and printing properties

*&lt;k-set>* accepts 3 attributes: _property_, _value_, _target_

property: the name of the property to be setted

value: the value of the property

target: _parent_ | _global_ | _private_ where to store the property. default to private if omitted

  parent: will store the property on the parent element

  global: will store the property on the global object (window)

  private: will store the property on the private object

*&lt;k-get>* accepts 2 attributes: _property_, _source_

property: the name of the property to print

source: _scoped_ | _parent_ | _global_ | _private_ the source where to read the property. default to private if omitted

  scoped: try to look if the property is on the parent, if not look on the parent's parent and so on, if not found try looking in private first and global as last.

  parent: look on the parent node

  global: look on the global object (window)

  private: look on the private object
