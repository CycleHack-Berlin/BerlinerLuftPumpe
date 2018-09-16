# OpenStreetMap query

```
[out:json][timeout:25][bbox:{{bbox}}];
(
  node["compressed_air"="yes"];
  node["amenity"="compressed_air"];
  node["service:bicycle:pump"="yes"];
  node["amenity"="bicycle_repair_station"];
  node["service:bicycle:diy"];
  node["amenity"="air_filling"];
  node["bicycle:air"="compressed_air"];
);

{{style:

node
{ color:black; fill-color: black;}

node[compressed_air]
{ color:green; fill-color:green; }

node[amenity=compressed_air]
{ color:darkgoldenrod; fill-color:darkgoldenrod; }

node[service:bicycle:pump]
{ color:deeppink; fill-color:deeppink; }

node[amenity=bicycle_repair_station]
{ color:blueviolet; fill-color:blueviolet; }

node[amenity=air_filling]
{ color:red; fill-color:red; }

node[service:bicycle:diy]
{ color:gray; fill-color:gray; }

node[bicycle:air=compressed_air]
{ color:blue; fill-color:blue; }

}}

out body;
>;
out skel qt;
```
