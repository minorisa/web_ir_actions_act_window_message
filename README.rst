.. image:: https://img.shields.io/badge/licence-AGPL--3-red.svg
   :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
   :alt: License


Client side message boxes
#########################

This module allows to show a message popup on the client side as result of a button, 
leveraging icons and css alerts from Bootstrap/FontAwesome.

Usage
=====

Depend on this module and return

.. code:: python

    {
        'type': 'ir.actions.act_window.message',
        'title': _('My title'),
        'message': _('My message'),
        'message_type': 'warning' | 'danger' | 'info'
    }

You are responsible for translating the messages. Message type can be any of the following strings:

* **warning**

  Will use ``class="alert alert-warning`` and ``<i class="fa fa-exclamation-circle fa-4x />``

* **danger** 

  Will use ``class="alert alert-danger`` and ``<i class="fa fa-exclamation-triangle fa-4x />``

* **info** 

  Will use ``class="alert alert-info`` and ``<i class="fa fa-info-circle fa-4x />``

Any other undefined message type will be defaulted to **info**.

Credits
=======

This module has been taken and adapted from OCA repository.

+ Therp BV
+ Odoo Community Association (OCA)
+ Minorisa

Maintainer
----------

.. image:: http://www.minorisa.net/wp-content/themes/minorisa/img/logo-minorisa.png
   :alt: Minorisa Logo
   :target: http://www.minorisa.net

**Minorisa Ready Partner**

Contributors
------------

* Jaume Planas <jaume.planas@minorisa.net>
