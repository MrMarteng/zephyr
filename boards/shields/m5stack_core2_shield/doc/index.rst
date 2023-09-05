.. _m5stack_core2_shield:

M5Stack-Core2 base shield
####################################

Overview
********

M5Stack-Core2 comes with a base shield that is connected to the M5Stack
extension connector. It features a MPU6886 6-axis motion tracker and a SPM1423
microphone.

Pins Assignments
================

+----------------------+--------------+
| Shield Connector Pin | Function     |
+======================+==============+
| 16                   | I2C - intSDA |
+----------------------+--------------+
| 17                   | I2C - intSCL |
+----------------------+--------------+
| 23                   | I2S - MCLK   |
+----------------------+--------------+
| 22                   | I2S - OUT    |
+----------------------+--------------+

Programming
***********

Set ``-DSHIELD=m5stack_core2_shield`` when you invoke ``west build``.
For example:

.. zephyr-app-commands::
   :zephyr-app: samples/drivers/mpu6050
   :board: m5stack_core2
   :shield: m5stack_core2
   :goals: build

References
**********

.. target-notes::

.. _datasheet:
   https://docs.m5stack.com/en/core/core2
