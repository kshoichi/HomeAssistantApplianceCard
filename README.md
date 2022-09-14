> My "Appliances" card. Shows appliance status, time remaining, and progress.

![Screenshot](https://i.redd.it/cg7xbbtg94p51.png)

I drew some appliances and added some circle graphs to keep track of
them. They are all LG appliances, so all the data comes from the LG
ThinQ integration and a few custom sensors that translate the
attributes into usable data. It will work with any data that you
supply, not just LG.

The LG integration has to be loaded from HACS first (SmartThinQ LGE
Sensors) before you'll see it in Home Assistant's integration list.

The number on each appliance updates to show the remaining time and
the circle graph animates as the cycles complete.

## Install ##

Steps to install:

Install the following items from [HACS](https://hacs.xyz/):

* [SmartThinQ LGE Sensors](https://github.com/ollo69/ha-smartthinq-sensors)
* [vertical-stack-in-card](https://github.com/ofekashery/vertical-stack-in-card)
* [circle-sensor-card](https://github.com/custom-cards/circle-sensor-card)

In Home Assistant / Configuration / Integrations, install the
SmartThinQ LGE Sensors Integration.

Add any necessary custom sensors to translate attributes into values
the circle-graph card can use. There's
a [sensors.yaml](./sensors.yaml) in my repo to help get you started.

Copy all the images from the github link to your www directory (you can
use the File Editor addon for this)

Copy the [yaml](./AppliancesCard.yaml) from github and paste it into
a new card. Edit the entity_id's and styles to fit your system.
