# Exploring GNSS accuracy and precision

APST 142 – GNSS Activity (Spring 2021)

In May 2021, Fleming College GIS students embarked on a field exercise to understand GNSS accuracy using consumer grade GNSS devices.

Step 1: Select a nearby Passive Control Station or Known Survey Point

Using the passive control network database on Government of Canada [website](https://webapp.geod.nrcan.gc.ca/geod/data-donnees/passive-passif.php?locale=en), I was able to see the locations of different control station across Canada.

I had bad luck in previous field exercises locating horizontal and vertical control stations, so I decided to pick a Canadian Base Network monument instead. The Canadian Base Network uses the NAD83CSRS ??? and were big blocks of concrete sticking out of the ground. I was able to see this location from Google Satellite imagery due to its size and I knew it was going to be an easy find.

[This one](https://webapp.geod.nrcan.gc.ca/geod/data-donnees/station/report-rapport.php?id=963020) by Humber College was the closest to me so it made sense to go. I also chose this control point because it was highly recommended by my classmates. Time for step two, which includes some planning before heading out the door.

Step 2: Plan your point collection

The first thing I did was to check the weather for my field day. The weather was not good this whole week, so I tried my best to pick a time when it was convenient and where the rain stopped. Since the Earth&#39;s atmosphere can introduce noise, it is important to check the [Ionospheric Noise Index and Map](http://www.trimbleionoinfo.com/Images.svc/TEC) to limit severe interference.

I made sure to consult the Trimble GNSS Planning online afterwards to see if there would be dilution of precision of error while I am in the field.

![](RackMultipart20210507-4-kx7rgo_html_e58f2db00445257a.jpg)

The geometry of satellite could introduce errors, which is based on a principle called the Dilution of Precision (DOP). Lowest DOP is good around the afternoon around 3pm!

![](RackMultipart20210507-4-kx7rgo_html_a409b0efe8def56a.jpg)

I knew I was likely to be working with only GPS satellite selection, so I turned other satellite constellations off. This planning chart was a one stop shop and showed me the visibility of satellites and Ionospheric formation.

![](RackMultipart20210507-4-kx7rgo_html_731213179c96c05f.jpg)

In my survey monument, I was expecting to have about 9 satellites available around my field time.

![](RackMultipart20210507-4-kx7rgo_html_c65e6d26bac49b6f.jpg)

The sky plot of GPS satellites at the time of my field collection. Notice only the American GPS constellations are selected (shown in green labelling).

Based on Google Maps&#39; satellite views, it looked like there were no tall buildings around or large objects that would interfere with my GNSS reading. This one was out of my control, but a wise surveyor had done some thinking long before me. Thanks, Mr. Surveyor!

Step 3: Collect a series or average number of points.

This was the fun part. When I got on scene of the control marker, I realized that it was situated on top of a hill by a beautiful arboretum. I was lucky that it was not raining at the time and I could soak in the gorgeous scenery around me while I did my &quot;work&quot;.

I tried three different devices for this experiment. They were:

1. Garmin Nuvi (Purchased ~2008)
2. Magellan eXplorist GC (For geocaching)
3. iPhone 11

For my iPhone, I used ArcGIS&#39;s Field Maps and I took the coordinates from my Magellan straight off the screen. I sensed that there might be some difficulty to compare because the datums and coordinate system could be different.

![](RackMultipart20210507-4-kx7rgo_html_f24587365373de1c.jpg)

I turned on my devices to let them soak (stabilize) for about 15 minutes. Unfortunately, the Garmin Nuvi did not hold a charge well as it was old. It was out of the experiment before I could make it to the control monument ☹.

Before I started measuring, I think my Magellan should be accurate up to 5m and my iPhone would be around 10m at best. I would probably rate the accuracy from best to worst as Magellan, Garmin Car GPS (if it worked!), iPhone.

I took multiple points with the iPhone with different averaging to see whether it would significantly improve its accuracy.

Step 4: Compare and Share!

I created an ArcGIS online web map documenting the points I have collected with different satellite devices. [Take a look](https://maps.arcgis.com/apps/mapviewer/index.html?webmap=7299bc33b847446680a8bc61cb0ef361).

[![](RackMultipart20210507-4-kx7rgo_html_1a69f6f2e9188f24.jpg)](https://maps.arcgis.com/apps/mapviewer/index.html?webmap=7299bc33b847446680a8bc61cb0ef361)

Since my iPhone did not have the ability to measure Dilution of precision (PDOP), I decided to create polylines for measurement. However, if you are to look at my iPhone web layer attributes, you will find more information about the point collection.

It turns out using the averaging function did not improve its accuracy beyond 5m. In fact, one of the points without averaging was closest to the control station, but it was likely due to luck. What I found surprising was that the iPhone and Magellan eXplorist GC had roughly the same accuracy.

At the end I found trying to get all the points on the same datum and coordinate system became challenging while mapping. In the future, I hope to use an android device and a newer GNSS unit to see if I can get the accuracy down to 1-2m.

That is all for this field camp experiment. Until next time!