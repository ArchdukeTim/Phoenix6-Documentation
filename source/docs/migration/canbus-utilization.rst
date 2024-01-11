CAN Bus Utilization
===================

CTR Electronics goes through great efforts to make our products efficient on CAN bus bandwidth. This article highlights the average default bus utilization of supported Phoenix 6 devices. Users should keep total CAN bus utilization below 90% to prevent any unexpected behavior. Information on changing the default CAN update frequency is available in the :ref:`status signal <docs/api-reference/api-usage/status-signals:changing update frequency>` and :ref:`control request <docs/api-reference/api-usage/control-requests:changing update frequency>` documentation.

.. note:: Using Phoenix API will automatically start up a diagnostic server which adds a constant 0-5% total CAN bus utilization.

.. list-table::
   :widths: 18 20 20 20 22
   :header-rows: 1

   * - Device
     - Phoenix 5 (CAN 2.0)
     - Phoenix 6 (CAN 2.0)
     - Phoenix 5 (CAN FD)
     - Phoenix 6 (CAN FD) [1]_

   * - .. centered:: Talon FX
     - 4.7%
     - 4.1%
     - 2.0%
     - 1.8%

   * - .. centered:: CANcoder
     - 1.8%
     - 1.7%
     - 0.9%
     - 0.9%

   * - .. centered:: Pigeon 2
     - 5.5%
     - 3.1%
     - 2.5%
     - 1.3%

.. [1] Phoenix 6 devices on CAN FD also increase the default update frequency of many status signals to 100 Hz.
