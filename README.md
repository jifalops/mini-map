[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/jifalops/mini-map)

# mini-map
A drag-to-resize google-map with optional directions.

## Installation

```
bower i -S mini-map  # Polymer 2.0 hybrid (1.x compatible)
```

## Demo
<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="mini-map.html">
    <geo-codec id="codec" api-key="AIzaSyAUPOaJubJnaRTPUd_xX8MOA62gRtSlfCc"></geo-codec>
    <next-code-block></next-code-block>
    <script>
      var map = document.getElementById('map');
      var codec = document.getElementById('codec');
      var search = document.getElementById('search');
      map.icon = '../marker.png';
      function geocode() {
        codec.geocode(search.value, function(address, lat, lng, place) {
          map.lat = Number(lat);
          map.lng = Number(lng);
        });
      }
      setTimeout(geocode, 500);
    </script>
  </template>
</custom-element-demo>
```
-->

```html
<input id="search" value="usa" />
<button onclick="geocode()">Search</button><br/>
<mini-map id="map" api-key="AIzaSyAUPOaJubJnaRTPUd_xX8MOA62gRtSlfCc" zoom="3">
  <span>Info</span>
</mini-map>
```

Full demo:
[webcomponents.org](https://www.webcomponents.org/element/jifalops/mini-map/demo/demo/index.html)
| [github](https://jifalops.github.io/mini-map/components/mini-map/demo/).

API: [webcomponents.org](https://www.webcomponents.org/element/jifalops/mini-map/mini-map)

## Contributing

1. Fork it on Github.
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT](https://opensource.org/licenses/MIT)
