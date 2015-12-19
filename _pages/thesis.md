---
title: "Leveraging human-computer interactions and social presence with physiological computing"
---

I obtained a PhD in computer science from the university of Bordeaux. During 3 years, between 2012 and 2015, I had been part of the Laboratoire Bordelais de Recherche en Informatique ([LaBRI](http://www.labri.fr)) and worked in [Inria](http://www.inria.fr/en/) as a member of the [Potioc](https://team.inria.fr/potioc/) team. I was supervised by [Martin Hachet](http://people.bordeaux.inria.fr/hachet/) and [Fabien Lotte](https://sites.google.com/site/fabienlotte/).

My thesis explored how physiological computing could contribute to human-computer interaction (HCI) and foster new communication channels among the general public. My thesis committee was composed of [Stephen H. Fairclough](http://physiologicalcomputing.org/), [Anatole Lécuyer](http://people.rennes.inria.fr/Anatole.Lecuyer/), [Nicolas Roussel](http://interaction.lille.inria.fr/~roussel/) and [Thorsten O. Zander](http://www.phypa.org/team/thorsten-zander.html) -- quite a dream team if you may.

Over the course of this work I published 10 peer-reviewed papers, including a journal publication, 6 publications in the very best conferences in human-computer interaction ([UIST](http://uist.acm.org/uist2014/), [INTERACT](http://www.interact2015.org/), [TEI](http://www.tei-conf.org/16/), [CHI](https://chi2016.acm.org/) -- all with acceptance rate around 25%), and a best student paper award at the [PhyCS '15](http://www.phycs.org/?y=2015) conference. OK, sorry, that was just to show-off while I can, in case someone wanting to hire a post-doc ends up here. More informative content below, namely the abstract of my thesis and the slides used during my defense.

![Overall picture of my thesis](/images/thesis/overall.jpg)

## Abstract

My work, which studied physiological sensors at large and electroencephalography (EEG) in particular, covers four aspects.

First, we[^1] investigated how those measurements could be employed to assess the mental state of the users and how they relate to other evaluation methods, such as inquiries and behavioral measures. Our review directly led to practical applications, consisting in the continuous evaluation of HCI. We created the first Brain-Computer Interface (BCI) that could discriminate visual comfort from visual discomfort during the viewing of stereoscopic images. In another study, we found evidences that workload could be assessed continuously with EEG during 3D manipulation tasks. When we extended on this work to monitor attention and error recognition besides workload, we compared different interaction techniques through the use of a serious game, shaping a framework that could help to assess the overall user experience.

[^1]: If in science it's common to use the "we" pronoun as a formal way to speak about oneself, even when only one person is implied, I cannot stress enough how much my work benefited from the help of my teammates. 

These various applications necessitate components that are still too difficult to use in the field. We made several technical contributions that permit lowering the barrier between end users and physiological sensors. We participated in the software integration of a low-cost and open-hardware EEG device, OpenBCI. We implemented a signal processing pipeline that uses low-cost webcams to measure heart rate remotely, by the mean of photoplethysmography (PPG). We crafted wearables that could quickly equip users so that electrocardiography, electrodermal activity or electroencephalography may be measured during public exhibitions. Those various developments helped us to envision new usages for our sensors beside HCI evaluation.

Indeed, thanks to the steady dissemination in everyday life of devices that sense physiological signals, an additional communication channel for people may come to exist. So as to ground those insights, we elaborated two scenarios involving the most common measure, heart rate. In a study about human-agent interaction, participants tended to prefer virtual avatars that were mirroring their own internal state, meaning that the social presence of artificial beings could be reinforced with little effort. A follow-up study focused on interactions between users, taking advantage of a board game to describe how physiological monitoring could alter our relationships.

This last study profited from advances in HCI to mask computers from the participants, integrating seamlessly digital content -- for instance biofeedback -- to the physical world. The combination of spatial augmented reality and tangible interface enable the emergence of hybrid objects that could convey a high level of information while maintaining ease of use and attractiveness. Those tools helped to build a "Tangible EEG interface", Teegi. Teegi takes the appearance of a puppet and let novices discover by themselves about their brain activity. The prototype in our laboratory became a mobile installation that we bought to public festivals. Finally, we pushed forward this project to integrate more physiological sensors and give more freedom about their visualizations, the latter spanning across several layers of abstraction. Using a co-design approach that took place in a museum, we explored how such proxy shifts our representations, about our selves as well as about the others.

Four pictures of a 3-years journey during which I came to think that the purpose of computer science and human-computer interaction is to enhance well being and facilitate human relationships on the whole -- or at least this is the path into which I tried to venture, and this work represents one more step toward this goal I hope. Beyond the possibility for computers to comprehend some of our internal and mental states, physiological computing unveils another mean to mediate oneself, raising our social awareness.

## Defense

Here are the slides used during my defense, powered by [reveal.js](http://lab.hakim.se/reveal-js/). Press space bar to move forward, comments are embedded. For a full page version, visit [http://phd.jfrey.info/thesis-defense/](http://phd.jfrey.info/thesis-defense/) -- expects a 16:9 ratio. 

<iframe src="http://phd.jfrey.info/thesis-defense" width="800" height="500" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen ></iframe>
