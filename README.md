# circos-example
Example files to configure a circos connectogram for brain connectivity data


aal-map.txt file lists regions and the lobes they belong to (Roughly) and gives colours.

Example links file given in maps.links.txt

Edit links file to show edges and weights needed.

Region names should match those in aal-map.txt file.

Then run the local script

``
./parsemap -map aal-map.txt -links maps.links.txt  -datadir ./data/ 
``

then call the circos script, which should be in the path.

``
circos  -conf etc/brain.conf
``


