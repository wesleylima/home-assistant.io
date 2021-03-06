---
layout: page
title: "CPU speed"
description: "Instructions on how to integrate CPU speed within Home Assistant."
date: 2015-10-15 11:00
sidebar: true
comments: false
sharing: true
footer: true
logo: cpu.png
ha_category:
  - System Monitor
ha_release: pre 0.7
ha_iot_class: Local Push
redirect_from:
 - /components/sensor.cpuspeed/
---


The `cpuspeed` sensor platform to allow you to monitor the current CPU speed.


<p class='note warning'>
  You can't use this sensor in a Container (like Hass.io) as it requires access to the physical CPU. Also, not all [ARM CPUs](https://github.com/workhorsy/py-cpuinfo/#cpu-support) are supported.
</p>

## {% linkable_title Configuration %}

To add this platform to your installation, add the following to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
sensor:
  - platform: cpuspeed
```

{% configuration %}
name:
  description: Name to use in the frontend.
  required: false
  type: string
  default: CPU speed
{% endconfiguration %}
