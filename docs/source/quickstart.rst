Quickstart
==========


.. _installation:

Installation
------------

idk how to install hanchu plz write this


Running a Scenario
------------------

To run a scenario, first create two terminal windows. In the first one, change into your Carla directory. 
Run the command ``./CarlaUE4.sh`` to start your Carla Engine. Now, in the other window, you can run the command 
``python3 EI_Drive.py`` to start a scenario, default being ``demo``. 

To change to scenario being ran, add the argument ``test_scenario=`` with the name of the test scenario that 
you want to run.

Modifying Existing Scenarios
----------------------------

To modify parameters of existing scenarios, go to the directory

.. code-block:: console
    EIdrive/scenario_testing/config_yaml/test_scenario

Here, the ``.yaml`` files hold to the settings applied to the whole scenario. 
Important settings that you might may wish to modify: 

- ``vehicle_perception``: when it is ``perception_true``, vehicles can use camera and LIDAR data. To turn it off, set it to ``perception_false``.

- ``game_map``: ``map_activated`` turns the game map visualization on. We leave ``map_deactivated`` off to save processing power.


To modify parameters of existing scenarios, go to the directory

.. code-block:: console
    EIdrive/scenario_testing/config_yaml/test_scenario/scenario

Here, the ``.yaml`` files hold to the settings applied to specific vehicles in the corresponding scenario.

