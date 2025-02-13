================
PoS Order Margin
================

.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fpos-lightgray.png?logo=github
    :target: https://github.com/OCA/pos/tree/16.0/pos_margin
    :alt: OCA/pos
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/pos-16-0/pos-16-0-pos_margin
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runbot-Try%20me-875A7B.png
    :target: https://runbot.odoo-community.org/runbot/184/16.0
    :alt: Try me on Runbot

|badge1| |badge2| |badge3| |badge4| |badge5| 

This module shows margins in PoS frontend during an order creation.

**Table of contents**

.. contents::
   :local:

Configuration
=============

* If you want to disable the display of the margin, in the front-office UI, you can
  uncheck the check box in the `res.config.settings` shop form:

.. figure:: https://raw.githubusercontent.com/OCA/pos/16.0/pos_margin/static/description/pos_config_setting.png

Known issues / Roadmap
======================

This dependency can be removed, when Odoo Core will be correctly refactored,
moving this ``@api.model`` function in a more generic module (``account``
for exemple).

Changelog
=========

16.0.1.0.0
~~~~~~~~~~

* Migrate to V16.0
* Remove ``pos.order`` and ``pos.order.line`` funcionality from V14.0.
  It's already done by V16.0.
* Remove tests.
* Create a ``res.config.settings`` field `pos_iface_display_margin`
  to display margins in PoS frontend.

14.0.1.0.0
~~~~~~~~~~

* Migrate to V14.0

13.0.1.0.0
~~~~~~~~~~

* Migrate to V13.0
* Reuse ``sale_margin`` computation to handle multi currency context.
* Correct computation of margin, if a module that adds ``uom_id`` on
  ``pos.order.line`` is installed.
* Add test

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/pos/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed
`feedback <https://github.com/OCA/pos/issues/new?body=module:%20pos_margin%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* GRAP
* FactorLibre

Contributors
~~~~~~~~~~~~

* Sylvain LE GAL (https://twitter.com/legalsylvain)
* Wolfgang Pichler
* Murtaza Mithaiwala (https://twitter.com/MurtazaMithaiw4)
* Dhara Solanki <dhara.solanki@initos.com>
* Juan Carlos Bonilla <juancarlos.bonilla@factorlibre.com>

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

.. |maintainer-legalsylvain| image:: https://github.com/legalsylvain.png?size=40px
    :target: https://github.com/legalsylvain
    :alt: legalsylvain

Current `maintainer <https://odoo-community.org/page/maintainer-role>`__:

|maintainer-legalsylvain| 

This module is part of the `OCA/pos <https://github.com/OCA/pos/tree/16.0/pos_margin>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
