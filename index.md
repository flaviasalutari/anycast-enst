---
layout: default
title: Anycast enumeration and geolocation
---


Use of anycast IP addresses has increased in the last few years: once relegated to DNS root and top-level domain servers, anycast is now commonly used to assist distribution of general purpose content by CDN providers. Yet, most anycast discovery methodologies rely so far on DNS, which limits their usefulness to this particular service. This raises the need for protocol agnostic methodologies, that should additionally be as lightweight as possible in order to scale up anycast service discovery. Our anycast discovery method allows for exhaustive and accurate enumeration and city-level geolocation of anycast replicas, with the constraints of only leverages a handful of latency measurements from a set of known probes. The method, which exploits an iterative workflow to enumerate (optimization problem) and geolocate (classification problem) anycast instances, is described in {% cite jsac16 %},{% cite techrep16%},{% cite infocom15a %}. The method is so lightweight and protocol agnostic that we were able to perform several censuses of the whole IPv4 Internet (during March 2015), as described in {% cite conext15 %}. We keep performing such censuses and making this dataset available to the scientific community to the interactive Google maps interfaces accessible below.


## List of resources (at a glance)

<img style="float: left;" width='64px' src="/images/googlemaps.png">
**Googlemap interface:**
<br /> The new interface giving access to a spatio-temporal view of the [new monthly censuses](http://goo.gl/MGDmCz) (since December 2015), described in {% cite longitudinal17%}
The old version gives access to {% cite conext15%} results and uses the googlemap engine demoed at {% cite infocom15b %}
<br><br>

<img style="float: left;" width='64px' src='/images/list.png' alt='' title='' />
**Anycast list:**
<br /> Browse the characteristics of monthly censuses in [tabular format](http://perso.telecom-paristech.fr/~drossi/anycastLongitudinalSlickgrid) or check the [monhtly lists of anycast IP/24](http://goo.gl/DPUJz1) (since December 2015)
Results concerning the [top-100 anycast ASes](http://goo.gl/Ff8gdQ) described in {% cite conext15%} (March 2015)

<br><br>
<img style="float: left;" width='64px' src="/images/tarball.png">
**Raw measurement:**
<br /> [Census](http://perso.telecom-paristech.fr/~drossi/index.php?n=Dataset.Anycast#censuses) measurement (described in {% cite conext15%})
Monthly [censuses](http://perso.telecom-paristech.fr/~drossi/index.php?n=Dataset.Anycast#censuses) measurements since 2016/06 (described in {% cite longitudinal17%})

<br><br>
<img style="float: left;" width='64px' src="/images/github.png">
**Code and dataset:**
<br /> [version 1.0 of iGreedy source code](http://goo.gl/7ESrCR), including dataset with ground truth, used to obtain results of {% cite jsac16 %}
Our [scalable census analyzer](https://github.com/TeamRossi/anycast-census), used to analyze the above raw measurement {% cite longitudinal17%}

<br><br>
<img style="float: left;"  rowspan="5" width='64px' src="/images/papers.png">
**Publications:**
 If you find these dataset and code useful, we would be grateful if you could please cite one of our papers in the [publication](http://perso.telecom-paristech.fr/~drossi/index.php?n=Dataset.Anycast#PAPER) section.
iGreedy is introduced in {% cite infocom15a %}, thorougly analyzed in {% cite jsac16 %}  (and exhaustively analyzed in {% cite techrep16 %} ).
We apply iGreedy since {% cite conext15 %} to collect monthly censuses of IPv4 anycast {% cite longitudinal17 %} (if still in doubt which is the most appropriate for your work don't hesitate to contact us!)

{% bibliography %}