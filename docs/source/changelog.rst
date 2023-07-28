Changelog
=========

Version 1.0.1
--------------
**Date** 2023-07-28

GENERAL
^^^^^^^^
    - YD-48 Removed Bisect Branding
    - YD-39 Finished Migration from BiSect to Pufferfish

PROXY
^^^^^^
    - YD-73 Added a Cross-Server tablist
       - So you can see your friends no matter what server you are on!

SMP
^^^^
    - YD-78 Items no longer despawn when chunk unloads
    - YD-83 Removed chat timer and spam detection

CREATIVE
^^^^^^^^^
    - YD-56 Wrong message when being sent to CREATIVE
    - YD-55 Player permission tweaks
       - /spawn no longer has a wait period (cooldown still exists)
       - Players now teleport to their last known location instead of spawn
          - Unless you join for the first time
       - /speed Added
       - /flyspeed Added 
    - YD-53 Server update
       - All 3rd party plugins updated
       - WorldEdit removed, FAWE Added
       - Spawn locations updated
       - Creative World has been prerendered to the worldborder
       - Plot Data is now stored on the database
       - PlotSquared support added to Dynmap
    - YD-72 FAWE Limits
       - Max Memory: 80%
       - Tick Limiter enabled
          - Interval set to 20 seconds
          - 64 falling blocks per interval
          - 10 Physics events (ms) per interval
          - Max 256 item spawns per interval

Infrastructure
^^^^^^^^^^^^^^^
    - YD-92 RabbitMQ setup
    - YD-37 Redis setup
    - YD-93 Docker Services Stack setup
    - YD-36 MongoDB setup
    - YD-94 Portainer CE setup

Current Bugs (Not Fixed)
^^^^^^^^^^^^^^^^^^^^^^^^^
    - YD-86 Mob Spawning (CognitiveGear)
       - Recent Minecraft updates made it so mobs can only spawn at Light Level 0, but something is wrong on the server and it seems to have been reverted to the original spawning conditions
    - YD-71 FAWE Flood Fill (Ian25)
       - At high Y-levels (seems to be ~304) if you use the fill command it seems to break out of the PlotSquared region by ~11 blocks.
    - YD-90 Boats positional issue (Karbl)
       -  there is some positional issues with boats, often players appear invisible for awhile after getting out of one. noticed that text boxes above players stay at the position that they got into a boat.


Version 0.0.0
--------------
**Date** 2023-07-28

    - initialization of changelog
