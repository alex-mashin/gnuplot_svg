# gnuplot_svg
A JavaScript that makes a gnuplot graph exported to SVG responsitive in the browser.

To have it connected to the exported SVG, set the web server to serve the file `https://github.com/alex-mashin/gnuplot_svg/gnuplot_svg.js`
by the address `/js/gnuplot/gnuplot_svg` and call `gnuplot` like this:
```sh
/usr/bin/gnuplot -e "set terminal svg size $width,$height dynamic enhanced font 'arial,$size' mousing jsdir '/js/gnuplot' \
  name '$name' $heads dashlength 1.0;" -
```

Based on the work by Marko Karjalainen <markokarjalainen@kolumbus.fi> published at http://gnuplot.sourceforge.net/demo_svg_5.4/gnuplot_svg.js.
