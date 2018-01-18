---
layout: page
title: Anycast enumeration and geolocation
permalink: /miscellany/item-1/
---

Use of anycast IP addresses has increased in the last few years: once relegated to DNS root and top-level domain servers, anycast is now commonly used to assist distribution of general purpose content by CDN providers. Yet, most anycast discovery methodologies rely so far on DNS, which limits their usefulness to this particular service. This raises the need for protocol agnostic methodologies, that should additionally be as lightweight as possible in order to scale up anycast service discovery. Our anycast discovery method allows for exhaustive and accurate enumeration and city-level geolocation of anycast replicas, with the constraints of only leverages a handful of latency measurements from a set of known probes. The method, which exploits an iterative workflow to enumerate (optimization problem) and geolocate (classification problem) anycast instances, is described in [^JSAC-16],[^TECHREP-16],[^INFOCOM-15a]. The method is so lightweight and protocol agnostic that we were able to perform several censuses of the whole IPv4 Internet (during March 2015), as described in [^CoNEXT-15]. We keep performing such censuses and making this dataset available to the scientific community to the interactive Google maps interfaces accessible below.


## List of resources (at a glance)

<img style="float: left;" width='64px' src="/images/googlemaps.png">
**Googlemap interface:**
<br /> The new interface giving access to a spatio-temporal view of the [new monthly censuses](http://goo.gl/MGDmCz) (since December 2015), described in [^LONGITUDINAL-17]
The old version gives access to [^CoNEXT-15] results and uses the googlemap engine demoed at [^INFOCOM-15b]
<br><br>

<img style="float: left;" width='64px' src='/images/list.png' alt='' title='' />
**Anycast list:**
<br /> Browse the characteristics of monthly censuses in [tabular format](http://perso.telecom-paristech.fr/~drossi/anycastLongitudinalSlickgrid) or check the [monhtly lists of anycast IP/24](http://goo.gl/DPUJz1) (since December 2015)
Results concerning the [top-100 anycast ASes](http://goo.gl/Ff8gdQ) described in [^CoNEXT-15] (March 2015)

<br><br>
<img style="float: left;" width='64px' src="/images/tarball.png">
**Raw measurement:**
<br /> [Census](http://perso.telecom-paristech.fr/~drossi/index.php?n=Dataset.Anycast#censuses) measurement (described in [^CoNEXT-15])
Monthly [censuses](http://perso.telecom-paristech.fr/~drossi/index.php?n=Dataset.Anycast#censuses) measurements since 2016/06 (described in [^LONGITUDINAL-17])

<br><br>
<img style="float: left;" width='64px' src="/images/github.png">
**Code and dataset:**
<br /> [version 1.0 of iGreedy source code](http://goo.gl/7ESrCR), including dataset with ground truth, used to obtain results of [^JSAC-16]
Our [scalable census analyzer](https://github.com/TeamRossi/anycast-census), used to analyze the above raw measurement [^LONGITUDINAL-17]

<br><br>
<img style="float: left;"  rowspan="5" width='64px' src="/images/papers.png">
**Publications:**
 If you find these dataset and code useful, we would be grateful if you could please cite one of our papers in the [publication](http://perso.telecom-paristech.fr/~drossi/index.php?n=Dataset.Anycast#PAPER) section.
iGreedy is introduced in [^INFOCOM-15a], thorougly analyzed in [^JSAC-16] (and exhaustively analyzed in [^TECHREP-16 ] ).
We apply iGreedy since [^CoNEXT-15] to collect monthly censuses of IPv4 anycast [^LONGITUDINAL-17] (if still in doubt which is the most appropriate for your work don't hesitate to contact us!)

{% bibliography %}

[^LONGITUDINAL-17]: [LONGITUDINAL-17] Cicalese, Danilo and Rossi, Dario, [A longitudinal study of IP Anycast](http://www.enst.fr/~drossi/paper/rossi17longitudinal.pdf). July 2017.
[^JSAC-16]: [JSAC-16] Cicalese, Danilo, Joumblatt, Diana , Rossi, Dario, Buob, Marc-Olivier , Auge, Jordan and Friedman, Timur , [Latency-Based Anycast Geolocalization: Algorithms, Software and Datasets](http://www.enst.fr/~drossi/paper/rossi16jsac.pdf) . IEEE Journal on Selected Areas of Communications, Special issue on Measuring and Troubleshooting the Internet, 6:1889-1903, june 2016.
[^TMA-16]: [TMA-16] Giordano, Danilo, Cicalese, Danilo, Finamore, Alessandro, Mellia, Marco, Munafo, Maurizio, Joumblatt, Diana and Rossi, Dario, [A First Characterization of Anycast Traffic from Passive Traces](http://www.enst.fr/~drossi/paper/rossi16tma.pdf) . In IFIP workshop on Traffic Monitoring and Analysis (TMA),, pages 30-38, April 2016.
[^TECHREP-16]: [TECHREP-16] Cicalese, Danilo, Joumblatt, Diana , Rossi, Dario, Buob, Marc-Olivier , Auge, Jordan and Friedman, Timur , [Latency-Based Anycast Geolocalization: Algorithms, Software and Datasets (Extended Technical Report)](http://www.enst.fr/~drossi/dataset/anycast/anycast-techrep.pdf) . In Tech. Rep., 2016.
[^CoNEXT-15]: [CoNEXT-15] Cicalese, Danilo, Auge, Jordan, Joumblatt, Diana, Friedman, Timur and Rossi, Dario, [Characterizing IPv4 Anycast Adoption and Deployment](http://www.enst.fr/~drossi/paper/rossi15conext.pdf) . In ACM CoNEXT, awarded the IRTF Applied Network Research Prize at IETF96, Heidelberg, December 2015.
[^INFOCOM-15b]: [INFOCOM-15b] Cicalese, Danilo, Joumblatt, Diana , Rossi, Dario, Buob, Marc-Olivier , Auge, Jordan and Friedman, Timur , [A Lightweight Anycast Enumeration and Geolocation](http://www.enst.fr/~drossi/paper/rossi15infocom-b.pdf) . In IEEE INFOCOM, Demo Session, Hong Kong, China, Apr 2015.
[^INFOCOM-15a]: [INFOCOM-15a] Cicalese, Danilo, Joumblatt, Diana , Rossi, Dario, Buob, Marc-Olivier , Auge, Jordan and Friedman, Timur , [A Fistful of Pings: Accurate and Lightweight Anycast Enumeration and Geolocation](http://www.enst.fr/~drossi/paper/rossi15infocom.pdf) . In IEEE INFOCOM, Hong Kong, China, Apr 2015.
[^AIMS-15]: [AIMS-15] Cicalese, Danilo, Auge, Jordan, Joumblatt, Diana , Rossi, Dario and Friedman, Timur , [Anycast census and geolocation](http://www.enst.fr/~drossi/paper/rossi15aims.pdf) . In 7th Workshop on Active Internet Measurements (AIMS 2015), San Diego, CA, Mar 2015.
[^AINTEC-2014]: [AINTEC-2014] D. Rossi, [Anycast enumeration and geolocation](http://www.enst.fr/~drossi/paper/rossi14aintec.pptx) . Technical report, Keynote speech at ACM SIGCOMM AINTEC'2014, 2014.