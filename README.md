

Actions
=======

Setting up GraphHopper files
----------------------------

    $ tar xfz SG-gh.ghz

Or, from the graphhopper package, call

    graphhopper$ ./graphhopper.sh import <XXX.osm>

Refreshing the cache
--------------------

    $ sbt "run cache"

Running the routing
-------------------

    $ sbt "run route"

OR

    $ sbt run



TODO
====

1. Set up the web server to preview routes (DS)
2. Parallelize create step (DS)
3. More constraints on route feasibility
  a. Max detour time (hard coded time)
  b. Max detour time (as % of max route)
4. Other scoring functions?
5. Threshold annealing (Liwei)
6. Best regret route creation