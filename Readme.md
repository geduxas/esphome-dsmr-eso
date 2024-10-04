Tai ESPHome praplėtimas tinkantis nuskaityti ESO skaitiklius.
Modifikuotas [SlimmeLezer](https://github.com/zuidwijk/dsmr)
ir [ESPHome DSRM](https://github.com/esphome/esphome) priedas. 
Vietoj ESPHome dsmr komponento naudoti dsmr_eso.



Naujam projektui reikia nurodyt

```
substitutions:
  device_name: slimmelezer
packages:
  esodsmr: github://geduxas/esphome-dsmr-eso/p1_standard.yaml@main # p1_standard.yaml; p1_extended.yaml; p1_max.yaml
esphome:
  name: ${device_name}
  name_add_mac_suffix: false
  project:
    name: geduxas.esodsmr
    version: "2.0"
```
