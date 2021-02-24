---
layout: post
title: Drone Lynq Integration
date: 2019-11-14 02:30 -0500
tags: mechanical, electrical, hacking, integration, retrofit
image:
  feature: 2019-07_DroneLynqIntegration/drone-1.jpg
  teaser: 2019-07_DroneLynqIntegration/drone-1.jpg
photos:
  set: drone
  size: 9
  gallery: 2019-07_DroneLynqIntegration
url: drone-lynq-integration
---

In a previous job I was tasked me with integrating our then-flagship product (a personal tracking device) into an entry-level drone as a proof of concept that our technology could be an effective way to manage drone location. Because the size of the drone was quite small, limiting added weight was a priority, the device needed to be stripped as much as possible.

The internals were removed from their plastics, the display was done away with, the user interface button removed. The li-ion battery was discarded in favor of jacking power directly from the drone's 3.3v power line (a small firmware modification was also necessary to prevent a low-battery warning). The most open section of the drone's internals were chosen for mounting the added hardware, and an orientation was found that would allow the original micro-USB port to be accessed (for firmware changes and device configuration via computer). Regardless of the orientation or location, however, part of the board would need to be trimmed down to allow for proper clearance and thus allow for reassembly of the drone. With access to the schematics for the device, I was able to confirm that portions of the board being removed would either not damage traces on any of the internal layers of the board, or would only affect disused portions of the system (such as the charging circuit). Finally, the board was wrapped in polyimide tape, glued in place, and the drone was re-assembled. Externally, the only indication of any modification at all was the externally-accessible micro USB port, and the drone's flight was unaffected. Projects like this which provide challenges on multiple fronts are some of my favorites!