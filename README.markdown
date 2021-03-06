Route-Me: iOS map library
-------------------------

Route-Me is an open source map library that runs natively on iOS.  It's designed
to look and feel much like the inbuilt iOS map library, but it's entirely open,
and works with any map source.

This fork contains the same framework as in the original repository, but compiles
into an easy to use RouteMe.framework, based on [this description][buildfw].
   [buildfw]: https://github.com/jverkoey/iOS-Framework#walkthrough

Currently, [OpenStreetMap][1], [Microsoft VirtualEarth][2], [CloudMade][3],
[OpenAerialMap][4], [OpenCycleMap][5], [SpatialCloud][6], [TileStream][7], and two
offline-capable, database-backed formats (DBMap and [MBTiles][8]) are supported
as map sources.

Please note that you are responsible for getting permission to use the map data,
and for ensuring your use adheres to the relevant terms of use.


   [1]: http://www.openstreetmap.org/index.html
   [2]: http://maps.live.com/
   [3]: http://www.cloudmade.com/
   [4]: http://www.openaerialmap.org/
   [5]: http://www.opencyclemap.org/
   [6]: http://www.spatialcloud.com/
   [7]: http://mapbox.com/tilestream
   [8]: http://mbtiles.org/


Installing
----------

As Route-Me is undergoing some significant changes, the recommended course of
action is to clone a copy of the repository:

      git://github.com/florianheller/route-me.git

Or, [download the trunk][dl].

Just include the RouteMe.framework in your Xcode-project and import the &lt;RouteMe/RouteMe.h&gt; header.

See the 'samples' subdirectory for usage examples.

There are three subdirectories - RouteMe, Proj4, and samples. Proj4 is a support class used to do map projections. The RouteMe project contains only the route-me map framework. "samples" contains some ready-to-build projects which you may use as starting points for your own applications, and also some engineering test cases. `samples/SampleMap` and `samples/ProgrammaticMap` are the best places to look, to see how to embed a Route-Me map in your application.

See LicenseRouteMe.txt for license details. In any app that uses the Route-Me library, include the following text on your "preferences" or "about" screen: "Uses Route-Me map library, (c) 2008-2010 Route-Me Contributors". Your data provider will have additional attribution requirements.


   [dl]: http://github.com/florianheller/route-me/zipball/master
   
   
News, Support and Contributing
------------------------------

Join our [mailing list][list] for news and to communicate with project members
and other users:

To report bugs and help fix them, please use the [issue tracker][tracker]

[list]: http://groups.google.com/group/route-me-map
[tracker]: http://github.com/route-me/route-me/issues

