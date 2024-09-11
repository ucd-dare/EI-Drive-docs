Quickstart
==========


.. _installation:

Installation
------------

idk how to install hanchu plz write this


Running a Scenario
------------------

To run a scenario, first create two terminal windows. In the first one, change into your Carla directory.
To start your Carla world, run the command
.. code-block:: console
    ./CarlaUE4.sh

Now you can run a scenario using the other window using the following command. The defualt scenario to be run is ``demo``.
.. code-block:: console
    python3 EI_Drive.py

To change to scenario being ran, add the argument ``test_scenario=`` with the name of the test scenario that 
you want to run.

For example, to run the cooperative perception 1 scenario.
.. code-block:: console
    python3 EI_Drive.py --test_scenario=coop_perception_1


Modifying Existing Scenarios
----------------------------

To modify parameters of existing scenarios, go to the directory ``EIdrive/scenario_testing/config_yaml/test_scenario``.
Here, the ``.yaml`` files hold to the settings applied to the corresponding scenarioo. 
Important settings that you might may wish to modify: 

* ``vehicle_perception``: when it is ``perception_true``, vehicles can use camera and LIDAR data. To turn it off, set it to ``perception_false``.

* ``game_map``: ``map_activated`` turns the game map visualization on. We leave ``map_deactivated`` off to save processing power.


To modify parameters of existing scenarios, go to the directory ``EIdrive/scenario_testing/config_yaml/test_scenario/scenario``

Here, the ``.yaml`` files hold to the settings applied to specific vehicles in the corresponding scenario.

