---
layout: post
title: "Field testing in Abu Dhabi"
date: 2013-05-20 12:48
comments: true
categories: iPad Mobile Blue Carbon Abu Dhabi
author: Tim Wilkinson
---

<h2>Field testing in Abu Dhabi</h2>

{% img left /images/field_testing_abu_dhabi/the_app.png 300 The Blue Carbon iPad App %}

<p>UNEP-WCMC Informatics recently built their first in-house mobile application integrated with the AGEDI Blue Carbon 12 month Demonstration project to map the blue carbon habitats of Abu Dhabi.</p>

<p>The iOS application enables field scientists and volunteers to collect data on the location, size and characteristics of Mangroves, Seagrass, Salt Marsh and Algal Mat from the field regardless of there being a data connection.</p>

<p>The application was built with HTML, CSS and Javascript through <a href="http://phonegap.com/">phonegap</a> and syncronises to CartoDB, a geospacially enabled PostreSQL database, feeding the main browser based blue carbon application.</p>

<p>Throughout the development phase we tested the application, validating substitute habitats around Cambridge, and user tested with members of the field scientist team before they left for Abu Dhabi.</p>

<p>There is of course no substitute however for putting yourself in the end users shoes and actually using the application in the intended environment for an extended period of time.</p>

<p>In May of this year I had the opportunity to do just that, and took the iPad through its paces in Abu Dhabi mapping a number of areas of Mangrove east of the main city.</p>

<p>The application had been used by the field teams in late January / February and they’d done a great job of carefully logging all issues/errors they encountered, the scenarios under which they occurred, date, time and even climatic conditions.</p>

{% img left /images/field_testing_abu_dhabi/waterproof_case.png 250 The iPad in its waterproof Over Board case %}
{% img left /images/field_testing_abu_dhabi/using_the_app_for_navigation.png 250 Using the app for navigation %}


<p>The conditions in which the field work is taking place are fairly extreme. In May the temperature in Abu Dhabi is around 37 degrees celsius, and the habitats we are recording are in wet, tidal locations, often only accessible by beaching the boat at low tide. The soil conditions around mangroves are loose and effectively muddy, and the large seagrass fields can only be validated by boat, either with divers or by using a viewing device over the side of the boat.</p>

<p>The iPad is protected with a waterproof soft case which held up well in the heat, although cloudless skies and dazzling sun meant that glare was a problem.</p>

<p>We identified an area of mangrove that abutted a building site and had been previously mapped using remote sensing. As a test task I set about checking the accuracy of the remote sensing, and whether the extent of the habitat had been reduced at all by the nearby construction work.</p>

<p>The geolocation feature of the application was helpful in navigating to the site, and having the habitat layers made it simple to identify the specific regions of interest.</p>

{% img left /images/field_testing_abu_dhabi/using_the_aplication.png 250 discussing the work %}

<p>Having found a suitable place to anchor the boat we waded to shore and began the process of validation on foot. Making use of the geolocation feature again, I located myself relative to the mangrove extent and tapped the screen to mark the first point of my validation polygon. I walked a hundred yards and tapped the screen again at my location to create a second point. Using the geolocation marker in this way I worked around the extent of the mangrove until I arrived back at my first position.</p>

<p>Having been around the whole area I was in a good position to then record attributes such as density and size. We encountered some Arabian Deer grazing on the flowering mangrove plans, so I recorded that in the ‘notes’ section and took a few photos which could later be added to the validation via the desktop web interface.</p>

{% img left /images/field_testing_abu_dhabi/island_approach.png 250 Approaching the mangrove field from the Persian Gulf %}

<p>Two main things to note were that in this instance the remote sensing geometries were very detailed, and due to zoom limitations of the maps we had on the application the validation was only accurate to about 5 meters in a total area size of around 160m2. The second issue appeared when we synchronized the validation with the main application and reviewed it via the web interface. The validation was offset by around 2 meters which was either due to the difference in maps being used or due to the accuracy of the geolocation on the device.</p>


<p>The small size of the validation area amplified the inaccuracies, which on larger areas wouldn’t have the same significance, but we’ll go back and identify why the offset is occurring so we can improve accuracy.</p>

<h2>Conclusions</h2>

<ol>
<li>The glare issue is unsatisfactory and needs to be improved on, probably through modifications to the waterproof case.</li>
<li>The application needs to make use of higher resolution satellite maps to improve the levels of accuracy.</li>
<li>The satellite maps on the mobile application need to be the same as the desktop version (we’d used RapidEye imagery for the mobile app in an attempt to get better detail at higher zoom levels), to ensure consistency.</li>
<li>When validating existing habitats where there is no change it would be beneficial to be able to draw a rough polygon and have it snap to the original data to make sure accuracy isn’t lost. This is particularly valuable where the original data is highly detailed.</li>
<li>A feature to take photos directly in the application and have them attached to the validation would same time and help with cataloging.</li>
</ol>


<p>A really valuable trip, with lessons learned for future development and improvements.</p>



