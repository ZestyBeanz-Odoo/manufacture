==============
Repair Picking
==============

.. 
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! source digest: sha256:576ed4d5c0c1e57002a5f0fbd364f753297c27ebe3e35595ae64c9cd000b216d
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-LGPL--3-blue.png
    :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
    :alt: License: LGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fmanufacture-lightgray.png?logo=github
    :target: https://github.com/OCA/manufacture/tree/14.0/repair_picking
    :alt: OCA/manufacture
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/manufacture-14-0/manufacture-14-0-repair_picking
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
    :target: https://runboat.odoo-community.org/builds?repo=OCA/manufacture&target_branch=14.0
    :alt: Try me on Runboat

|badge1| |badge2| |badge3| |badge4| |badge5|

This module extends the repair management functionality in Odoo, providing additional
options for handling the repair process in a more customizable and efficient way.
It allows the configuration of repair steps based on specific business requirements
and adds new picking types for managing component addition and removal in repair orders.

The main features are:

- Customize repair steps: Choose between a 1-step, 2-step, or 3-step repair process.
- Add and remove components during the repair process using separate picking types.
- Associate repair orders with pickings for improved traceability.
- Automatic creation of pickings and procurement routes based on the selected repair steps.
- Manage repair locations and routes more efficiently with warehouse settings.

**Table of contents**

.. contents::
   :local:

Configuration
=============

#. Navigate to Inventory > Configuration > Warehouses, and select a warehouse.
#. In the "Repair Steps" field, choose between "Repair", "Pick component, repair", or "Pick component, repair, store removed component" to define the repair process.
#. Define the "Repair Location", "Add Component to Repair" picking type, "Remove component from Repair" picking type, and "Repair Route" as needed.

Usage
=====

#. Navigate to Repair > Repair Orders and create a new repair order.
#. In the Operations tab, add components to be added or removed during the repair process.
#. Confirm the repair order. This will automatically generate the necessary
   pickings based on the configured repair steps.
#. Process the pickings as required during the repair process.
#. If the repair order needs to be canceled, all associated pickings that are not
   in "cancel" or "done" state will also be canceled automatically.

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/manufacture/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us to smash it by providing a detailed and welcomed
`feedback <https://github.com/OCA/manufacture/issues/new?body=module:%20repair_picking%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* ForgeFlow

Contributors
~~~~~~~~~~~~

* Joan Sisquella <joan.sisquella@forgeflow.com>

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

This module is part of the `OCA/manufacture <https://github.com/OCA/manufacture/tree/14.0/repair_picking>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
