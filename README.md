# Diamond Protobuf Handler

This a handler for the [Diamond](https://github.com/python-diamond/Diamond) metric collector. It sends the gathered metrics encoded as [Googles Protocol Buffers](https://github.com/google/protobuf) over the HTTP(S) protocol to an endpoint. And exisitng endpoint that writes the metrics to an [InfluxDB](https://influxdb.com/) can be found [here](https://github.com/monitoring-ng/collector).

Since Diamond only accepts pull-requests that are fully pep8-clean but the protobuf compiler generates python code who couldn't give to sh\*ts about, it wasn't possible for me to get it into the upstream repo. If you want to use it, just put it into the correct directories in your existing configuration, or build Diamond yourself, putting the contents of this repo into ```src/diamond```.
