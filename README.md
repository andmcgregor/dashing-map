# Dashing Map Widget

Live demo: [http://dashing-map.herokuapp.com/](http://dashing-map.herokuapp.com/)

Created by: [@andmcgregor](http://www.twitter.com/andmcgregor)

## About

Uses the Google Maps API to display latitude and longitude coordinates.

## Screenshot

![Dashing map](https://s3-us-west-2.amazonaws.com/vineline/dashing_map.png)

## Installation

Type `dashing install 6386263` while in your project directory.

Add the following line of code to your layout.erb file:

    <script src="http://maps.googleapis.com/maps/api/js?key=<%= ENV['GOOGLE_MAPS_KEY'] %>&sensor=false&libraries=visualization"></script>

And finally set the environment variable `GOOGLE_MAPS_KEY` with your Google Maps API key.

## Using the widget

Include a widget with a `data-view` of `Map`. You can also use `data-color` to color the map and set `data-type` to `heat` to display a heatmap rather than pins. 

    <li data-row="1" data-col="1" data-sizex="3" data-sizey="2">
      <div data-id="map" data-view="Map" data-title="Map" data-type="heat" data-color="#222222"></div>
    </li>

## License

This widget is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/) license.

<img src="http://mirrors.creativecommons.org/presskit/buttons/88x31/png/by-nc-sa.png" width="100">
