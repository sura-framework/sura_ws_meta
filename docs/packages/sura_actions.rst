sura_actions
============

``sura_actions`` gives SURA robots simple autonomous tasks. A task is sent as a
ROS 2 action, and the robot reports progress while it runs.

For **underwater robots (AUVs)**, the package can:

* Surface or move to a requested depth.
* Move to a requested pose (position and orientation).
* Follow a route made of waypoints.

For **surface robots (USVs)**, it can move to a requested pose or follow a
waypoint route on the water surface.

The package also lets operators add and edit waypoints, save routes to a file,
and load them again. A control manager selects the control mode needed by each
action.

``sura_bringup`` starts the appropriate action servers for the robot family.
The action servers that use ROS 2 lifecycle nodes must be configured and
activated before they accept a task. See the package's ``README.md`` for
launch commands and examples.
