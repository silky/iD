## 1.8.1
* Fix tag help lookup (#2844)
* Support Internet Explorer 11 and Edge browsers (#2571)
* New road styling for bumpy/unpaved roads (#2564, #2750, #2847)
* Disambiguate building/office presets (#2793, #2799)
* Add handrail field to steps preset (#2815)
* Choose "best" imagery by default (#2826)
* Fix language detection when `navigator.languages` is empty (#2838) (thanks @jleedev)
* Support multiple overlays and fix alignment of minimap (#2813) (thanks @brianreavis)

## 1.8.0
* Don't update the urlhash during the walkthrough (#1795)
* Add surface type to parking preset (#2816)
* Make 100% background brightness the default (#2824)
* Use SVG for preset and feature icons (#2785)
* Add "Help Translate" icon next to "Report a Bug" (#2766)
* Update highway colors to match openstreetmap-carto (#2764)
* Prefer suggested capitalization in autocomplete box (#2791)
* Better support for browser language preferences (#2810) (Thanks @kriscarle)
* Disallow joining ways with conflicting tags (#2358) (Thanks @jfirebaugh)
* Add rugby union and rugby league presets (#2808) (Thanks @bagage)
* Add military presets (#2177) (Thanks @arunasank)
* Discard yh:WIDTH tags (#2806)
* Fetch proper tag references for relation types (#2797) (Thanks @tyrasd)
* Proper perimeter calculation in infobox (#2789)
* Fix bug creating points at edge of screen when panning (#2758)
* Add motorcycle parking preset (#2787)
* Better autocomplete suggestions in taginfo-sourced dropdowns (#2748)
* Add traffic signal type preset
* Fix bug where pressing '1' triggered fullscreen (#2786)
* Improvements to translated preset terms (#2777, #2756) (Thanks @bagage)
* Disable save button when changeset comment is empty (#1488)
* Better handling of multilingual `alt_name`, `old_name`, etc (#2658)
* Add preset for Semi-Detached House (#2776)

## 1.7.4
* Show docs for the selected value in raw tag editor (#2754) (Thanks @M1dgard)
* Improve display of implied values in access UI field (#2763)
* Better handling of preset search terms (#2756) (Thanks @M1dgard)
* Support cross-browser fullscreen display mode with F11 / ⌘⇧F (#2755) (Thanks @PaulAnnekov)
* Fix performance issue with multipolygon outer test (#2755)
* Change caption "Access" -> "Allowed Access" (#2761)
* Fix broken link and other help improvements (#2760)
* Fix bug with displaying label when centroid undefined (#2757) (Thanks @tyrasd)
* Replace close 'X' with Cancel button on save panel (#2378)
* Add `recycling:glass_bottles`, `recycling:plastic` (#2730)
* Add preset for `leisure=bowling_alley` (#2734)
* Render `highway=road` differently from `highway=unclassified` (#2742)
* Improve rendering of `highway=track` - dashed casing now more visible on dark backgrounds (#657)
* Change `highway=path` rendering to be more like `highway=footway` to avoid new user errors (#2327)
* Prevent users from accidentally adding `highway=yes` (#2744)
* Better styling for ephemeral tags (e.g. razed/abandoned/construction/proposed) (#2740, #1893)
* Add `bicycle=dismount` access option (#2726)
* Add support for Irish postcodes in address field (#2729) (Thanks @rory)
* Add "Road Surface" preset for `area:highway=*` (#2627)
* Add presets for Casino and Adult Gaming Center (#2684)
* Restore complete list of `address:` keys for address UI field (#2698)
* Preset searching should consider tag values (#2719)
* Add `highway=corridor` preset and universal `level` field for indoor mapping (#2687, #2218)
* Use space key to toggle radial menu (#2706)
* Add presets (`volcano`, `saddle`, `adit`, `tree_row`, `plant_nursery`) (Thanks @jmespadero)
* Use HTTPS if location protocol is HTTPS in `iD.Connection` (#2681) (Thanks @frewsxcv)
* Don't write unsavable changes to `localStorage` (#2705)
* Add recycling_type preset field (#2689) (Thanks @ebrelsford)
* Fast zoom and pan with Cmd/Control modifier key (#2691) (Thanks @rowanhogan)
* Improve handling of Wikipedia URLs (#2694) (Thanks @1ec5)
* Add minimap toggle to background menu, show GPX layer in minimap (#2693) (Thanks @rowanhogan)
* Add cycleway UI field for highways with bike lanes (#2686) (Thanks @ebrelsford)
* Improve appearance of Mapillary markers (#2690) (Thanks @pgiraud)

## 1.7.3
* Add fee field to toilet preset (#2639) (Thanks @alexandrz)
* Several improvements for more reliable save and post-save data fetch (#2667)
* Use locale passed in from container iframe instead of detected locale (#2672)
* Allow html entities in translated documentation titles (#2674)
* Add presets for `man_made=storage_tank` and `man_made=silo` (#2662)
* Add presets for RV/Marine toilet disposal and related fields (#2623)
* Add preset for `waterway=fuel` (#2589)
* Add preset for `amenity=biergarten` (#2641)
* Infobox for distance/area measurement and more info, hotkey Cmd-I (#2573)
* Fallback to 'en-US' when no language detected (#2650)
* Don't clean description/note/fixme values (#2659)
* Only urlencode tag values that start with http (#2657)
* Remove `platform` and `browser` from changeset tags (#2643)
* Clip oneway markers to viewport (#2638)
* Performance improvements for iD.Difference
* Fix error restoring changes after deleting a node (#2637)

## 1.7.2
* Fix for 404 Error caused by duplicates in multi-fetch node request (#2626)
* Fix oil well preset (#2621) (Thanks @1ec5)

## 1.7.1
* Add oil well preset (#2618) (Thanks @1ec5)
* Add radio mast preset (#2613) (Thanks @1ec5)
* Don't commit empty changesets (#1483)
* Add place=farm preset (#2604) (Thanks @Stalfur)
* Cleanup strings for website and email tags (#2323)
* Use semicolon-space as separator for opening_hours tags (#2301)
* Clear cached userDetails when auth events occur (#2588)
* New styling for barriers (#2592)
* In wireframe mode, draw all points (#2591)
* Invert background opacity widget display values (#2595)
* Save custom background imagery layer to localstorage (#2566)
* Better introductory help text (#2504) (Thanks @hkirat)
* Smarter way movement - avoid zorroing connected ways (#2516, #729)
* Add basic browser and platform info to changeset tags (#2559, #2449)
* Add drive_through preset to fast_food, atm, etc (#2459) (Thanks @brianegge)
* Use combo not checkbox for building field (#2553)
* Fix bug with copy/paste when originals are deleted (#2557)
* Tag motorway_link with explicit oneway=yes (#2555)
* Map-In-Map locator (toggle with '/' key) (#2554)
* Add service field for railways (#2552)
* Feature filtering: don't match multipolygon lines as 'Others' (#2548)
* Add network=* tag to public transport presets (#2549) (Thanks @gileri)
* Add incline field for highway=steps preset (#2456)
* Support node v0.12 (#2535)
* Resolve editing conflicts before saving (#2525, #1053)
* Don't delete ways from route, boundary, multipolygon relations (#2526, #1461) (Thanks @systemed)

## 1.7.0

* Fix typo in smoothness field - should be "impassable" (#2523)
* Update to Mapillary API v2 calls (#2522) (Thanks @peterneubauer)
* Add Rounded tooltips (#2521) (Thanks @samanpwbb)
* Add gender field to amenity=toilets preset (#2422)
* Update landuse presets (no single nodes, and better descriptions) (#2518)
* Update tree and forest presets to use leaf_type and leaf_cycle fields (#2512)
* Add shop=houseware preset (#2509)
* Make "Yes" and "No" translatable (#2286)
* Fix group home preset (#2510)
* Add amenity=grit_bin preset (#2500)
* Prevent user from zooming out too far when drawing (#2499)
* Add amenity=bicycle_repair_station preset (#2497)
* Add leisure=nature_reserve preset (#2496)
* Support copy and paste of selected features with ⌘-C/⌘-V (#642)
* Add amenity=public_bookcase preset (#2507) (Thanks @guillaumep)
* Add substation type field (#2486)
* Add junction=yes preset (#2484)
* Add takeaway and delivery fields to food presets (#2483)
* Add levels field to building=commercial preset (#2454)
* Add amenity=register_office preset (#2431)
* Add landuse=garages preset (#2430)
* Add natural=cave_entrance preset (#2412)
* Add amenity=fast_food preset (#2446)
* Switch to landuse=farmland as preferred Farm preset (#2478)
* Add bench and covered fields to bus stop preset (#2451)
* Replace icon fields with dropdown (#2433)
* Add Map Data panel
    - Data Layers (GPX, Mapillary)
    - Area filling options (full, partial, wireframe) (#813)
    - Map Features filtering (#1299, #1871, #2033)

## 1.6.2

* Fix "TypeError: r is undefined" (#2421)

## 1.6.1

* Remember raw tag editor expansion state across sessions (#2416)
* Translate text in changes section on save panel (#2417)
* Encode URL hash correctly (#2406)
* Capture ⌘-S even in input fields (#2409)
* Added some traffic_calming=* presets
* Prefer power=substation to sub_station
* Include state/province in U.S. and Canadian address formats
* Improve the error message on saving when offline (#2373)

## 1.6.0

* Add network field to Road Route relation preset (#2372)
* Updated TIGER layer to use TIGER 2014
* Added support for street-level imagery from Mapillary
* Added support for taginfo projects data
* Better infer restriction for no_u_turn (#2345)
* Update to rbush 1.3.3
* Improved a variety of presets
* Added `comment` url param to prefill changeset comment (#2311)

## 1.5.4

* Do not fully fill certain landuse values, e.g. landuse=residential (#542)
* Class midpoints to match parent way and adjust styles
* Test visibility of gpx coords instead of just comparing extents

## 1.5.3

* When adding gpx, only rezoom map if gpx not in viewport (#2297)
* Workaround for Chrome crash (#2295)
* Add mtb fields (#2244)
* Support option strings for combo fields (#2296)
* Render triangular midpoints to show direction of any selected way (#2292)

## 1.5.2

* Fixed Chrome/Windows selection bug (#2151)
* Don't automatically tag motorways, etc. as oneway=yes
* Disable Move and Rotate operations if area < 80% contained in the viewport

## 1.5.1

* Fix mixed content errors on https osm.org (#2281)
* Fix suggested access values for parking (#2280)

## 1.5.0

* Add support for localized address fields (#2246)
* Rendering improvements for layers (#2250)
* Add a map scale (#2266)
* Fix preset buttons (#2247)
* Better midpoint rendering (#2257)

## 1.4.0

* Ensure combobox menus are closed on blur (#2207)
* Limit imagery_used tag to 255 characters (#2181)
* Simplify and fix midpoint drawing logic (#2136)
* Prefer more specific 'Crosswalk' preset over generic 'Crossing'
* Add amenity=dojo preset
* Correctly trim whitespace in semicolon-separated multivalues (#2236)
* oneway fields now show "Assumed to be No" or "Assumed to be Yes" instead of "Unknown" (#2220)
* Add turn restriction editor

## 1.3.10

* `oneway=no` overrides implicit oneways on junction=roundabout, etc. (#2220)
* Add presets for fords, parking_entrance, charging_station, compressed_air, churchyard, shop=wine
* Improve access placeholders (#2221)
* Trim tag keys, and prevent duplicate tag keys (#2043)
* Fix inline tag help for fields that handle multiple tags
* Add 'width', 'length', 'lit' for appropriate presets (cycleways, sidewalks, sports pitch, etc)
* Render embarkment/cutting with dashed casing
* Rendering fixes for buildings, tunnels
* Add population field for various place presets
* Improvements to circularize action (#2194)
* Building field is yes/no (fixes #2111)
* Area fill colors in preset icons match map fill colors
* Add fill style for landuse=military

## 1.3.9

* Prevent closed areas from invalid disconnection (#2178)
* Remove layer field from waterway=stream
* Add preset for place=suburb and shop=seafood
* Remember last custom tile layer (#2094)
* Mapbox Satellite now supports z17-z19

## 1.3.8

* Disable circularize and orthogonalize operations when way is <80% contained in the viewport
* Add place=neighbourhood preset
* Add denomination=* field for cemetary, graveyard, funeral home
* Add preset for shop=funeral_directors
* Add icon for public_transport=stop_position
* Support quartile scheme for any imagery source (#2112)
* Zoom to GPX after adding (#2144)
* Correctly update UI after choosing GPX file (#2144)
* Add preset for leisure=ice_rink
* Add picnic area stuff: firepit, picnic_table, bbq
* Add 35 as an option in the maxspeed dropdown
* Add religion to cemetery preset (#2164)
* Fix tag reference layout on FF (#2159)
* Add "crop" field for landuse=farm/farmland/farmyard (#2149)
* Add "trees" field for landuse=orchard
* Add landuse=landfill
* Add the hoops=* field to the basketball preset (#1984)
* Add amenity=nightclub
* Add smoking field for many presets under amenity, building, office, tourism (#1990)
* barrier=fence shouldn't be an area (fixes #2158)
* Remove building_area from hospital, school, kindergarden
* Fix recycling field keys (#2140)

## 1.3.7

* Added building presets
* Improve how tags are merged when merging to a multipolygon
* Disable merge operation if at least one relation is incomplete
* Add shop=bookmaker, shop=lottery, and shop=art presets
* Use https URLs where supported
* Fix duplicate/missing objects after restoring data from localStorage
* Remove addr:housename field from address preset

## 1.3.6

* More protection against relation loops (#2096)
* Fix freeze when using Clinic preset (#2102)
* Allow rotating closed multipolygon members (#1718)
* Bump threshold for Orthogonalize to 12 degrees
* Added social_facility presets (#2109)

## 1.3.5

* Smoother and faster panning, zooming, and tooltips
* Fix bug relating to deleted nodes outside the viewport (#2085)
* Ensure "New Relation..." is always available (#2066)
* Add area=yes when necessary (#2069)
* Suppress radial menu when clicking warning (#2035)
* Protect against relation loops (#2072)
* Correct arrow direction on drawn segment (#2078)
* Don't upload tags with empty values (#1894)
* Add support for ids and locations as search input (#2056)
* Sort relation suggestions most recent first (#2052)
* Fix for Safari selection bug in combo box (#2051)
* Fix midpoint missing after undoing split (#2040)
* Don't remove addr:housenumber when changing address preset (#2047)
* Many preset additions: clock, rest area, service area, veterinary, funiculars, narrow gauge railways,
  gauge field, electrified field, tunnel field, crafts, doctor, dentist, clinic, studio, aerialways,
  and pistes.

## 1.3.4

* Replace TIGER 2012 layer with next-generation TIGER 2013 layer (#2010)
* Add tooltips to "untagged feature" warnings
* Add pressets and category for golf features (#2013)
* Information and bike parking preset refinements
* Faster/smoother zooming and panning
* Add "quick add" presets for common proper names
* Fix zoom to feature when clicking search results (#2023)

## 1.3.3

* Support for loading GPX-files via url parameter (#1965)
* Update osm-auth (#1904)
* Update 3rd party dependencies (Lo-Dash, D3, RBush)
* Build iD.Way.areaKeys from presets
* Add public_transport, military, emankment presets
* Reverse cardinal directions for relation member roles
* Improved warning visibility (#1973)
* Fix undo-related bug (#1978)

## 1.3.2

* Update maki
* Fix Disconnect of way with multiple intersections (#1955)
* Fix unclosed area rendering (#1958)
* Add presets for amenity=shelter, footway=sidewalk, footway=crossing, and various office values
* Add area categories
* Full-height background settings pane
* Add suggestions of common shop and amenity names
* Handle https wikipedia URLs
* Use assumed values for access placeholders (#1924)
* Distinguish between power=line and power=minor_line
* Reset invalid opacity values to default (#1923)

## 1.3.1

* Fix misalignment -> Fix alignment (#1913)
* Update maki (#1916)
* Prioritize boundary tag to minimize area fills (#1920)
* Fix background defaulting to 0% brightness (#1923)

## 1.3.0

* Fix corner case that could cause getting stuck in drag mode (#1910)
* Improved display of changed objects in save screen
* Improved performance
* Show attribution for overlay layers (#1909)
* Add OpenStreetMap GPS traces layer
* Show a list of multiple selected features in the sidebar
* Autocomplete city and postcode values (#1753)
* Add a button to trigger file browser for GPX (#1758)
* Prevent 'zoom in to edit' from showing up during save success (#1792)
* Add delete button to all forms (#1492)
* Omit non-OSM features from search results (#1890)
* Add additional check to prevent snapping to area fills (#1887)
* Fix adding localized value before name (#1797)
* Disable removing incomplete relation members (#1768)
* Show all combobox entries when clicking the caret (#1755)
* Improvements and fixes to the behavior of multilingual name fields
* Don't show combobox menu with only one item
* Don't prevent following an existing way when drawing (#1430)
* Allow "yes" and "no" check values to be translated (#1819)
* Treat a sole area=yes tag as "untagged" (#1867)
* Special case 'yes' values for type fields (#1876)
* Don't add addr:housenumber=yes when applying Address preset (#1874)
* Ensure preset fields are consistently ordered (#1876)
* Preserve existing Wikipedia language (#1868)
* Don't allow dragging of the map when the click starts in a button (#1869)
* Prefer to render highway=* styles over railway=* (#1880)
* Workaround cosmetic issues caused by a Chrome regression (#1879)
* New presets: man_made=observation, shop=locksmith, leisure=common and more

## 1.2.1

* Split only the line of a node shared by a line and an area
* Handle multipolygon corner case when splitting (#1799)
* Don't automatically apply building tags to shop=car (#1813)
* Don't suggest adding a relation to itself (#1820)
* Fix restoring changes when something is selected (#1857)
* Use generic access value as placeholder (#1780)
* Filter on combobox value, not title (#1836)
* Show relation documentation for relation presets (#1862)
* Limit squaring to near square or near straight nodes (#1733)
* More clever splitting of closed ways
* Improve circularize action
* Add more tags to areas list

## 1.2.0

* Don't auto-save intro tutorial edits (#1745, #1795)
* Added waypoint display to GPX layer
* Added "Straighten" operation
* Improve "Orthogonalize" behavior, rename to "Square"
* Add and improve many presets
* Save commit messages on blur (#1783)
* Add KSJ2 tags to discard list (#1794)
* Fix display of labels with wide characters
* Catch localStorage quota exception (#1807)
* Avoid consecutive identical nodes when adding a midpoint (#1296)
* Stop nudge when exiting move mode (#1766)
* Add "Continue" operation
* Delete relations that become empty (#465, #1454)
* Support polygon imagery bounds (#768)
* Pull imagery from editor-imagery-index
* Insert areas in sorted order (#1693)
* Fix some walkthrough glitches (#1744)

## 1.1.6

* Fix walkthrough on Firefox (#1743)
* Fix icon at end of walkthough (#1740)
* Fix walkthrough (#1739)

## 1.1.5

* Add amenity=ranger_station preset (1723)
* Add terms for tourism=artwork (#1726)
* Reduce prominence of share links, add G+
* Default wildcard tag values to "yes" (#1715)
* Add help topic on relations (#1708)
* Add default "Locator Overlay" layer (#1301)
* Refine toilet preset (#1697)
* Change delete shortcut to ⌘⌫/Ctrl-Backspace (#1698)
* Fix close button event binding in save dialog (#1713)
* Fix error when deleting a triangle vertex (#1712)
* Add support for an externally provided asset map (#1699)

## 1.1.4

* Fix adding multilingual name (#1694)
* Fix social buttons (#1690)
* Work around a Firefox bug that sometimes caused elements to be unselectable or stuck dragging (#1691, #1692)

## 1.1.3

* Fix behavior of enter key in name field (#1681)
* Remove area=yes when choosing an area preset (#1684)
* Save history more frequently (#1345)
* Fix combobox menu scroll bar behavior (#963)
* After editing, give a sense when map is updated (#1660)
* Clarify undo/redo tooltips (#1670)
* Add emergency=fire_hydrant preset (#1674)
* Refine power=generator preset (#1675)
* Add leisure=track preset (#1683)

## 1.1.2

* Fix cursor offset when clicking/dragging after resizing the window (#1678)
* Include low-frequency tag values if they have a wiki entry
* Fix tag value suggestions in preset comboboxes (#1679, #1680)

## 1.1.1

* Improve performance when drawing
* Tail should appear only first time
* Fix radial menu tooltip positioning on Firefox

## 1.1.0

* Fix radial menu tooltip positioning

## 1.1.0rc1

* Custom layers support TMS-flipped Y coordinate with {ty} replacement.
* Allow to join more than two ways (#649)
* Many preset additions and improvements
* Fix Japanese language input (#1594)
* Prevent merging over restriction relations (#1512)
* Support multiple overlay layers
* Fix name field for suffixed ISO 639-1 codes (#1628)
* Add ability to create a new relation (#1576)
* Permit translating all preset term lists (#1633)
* Include GPX and overlay layers in imagery_used (#1463)
* Move sidebar to left, map controls to right
* Rework search UI and consolidate with geocoder
* More dramatic different between hover and active edit feature pane

## 1.1.0beta1

* Performance improvements
* Added a UI for multilingual name tags
* "Report a bug" in footer is now an icon
* New style for radio buttons and check boxes
* Incomplete relations can no longer be deleted (previously, attempting to do so would generate a JS error)
* Render bridge casing for bridge=viaduct, etc. (#1500)
* Only draw intersections for {high,water,rail,aero}way lines (#1471)
* Improve tag reference loading feedback (#1262)
* Added relation presets
* Display relation members and memberships in inspector
* The sidebar is now persistent, rather than sliding in and out
* The feature being hovered over is previewed in the sidebar
* Zoom to feature only if map parameter isn't also specified
* Don't zoom too far in (>z20) (#1511)
* Don't zoom too far out (<z16). (#1522)
* Added the ability to create multipolygons
* Fix URL template host rotation
* Fix strokes sometimes being clipped as polygons (#1527)
* Refine selection behavior when dragging a node:
  * Preserve the sidebar state (#1401)
  * Show vertices of selected way (#1478)
  * Reselect exact previous selection when finished
* Fix one way marker rendering (#1534)
* You can now click the preset icon to return to the preset list
* All preset fields now have placeholders
* The save dialog now appears in the sidebar
* Added Address preset (#1524)
* Shorten "Zoom in" text, don't hide it on narrow screens (#1477)
* Fix "View on OSM" in sidebar footer (#1473)
* When deleting a vertex, reselect another vertex if possible (#1457)
* The sidebar now has a searchable Feature List (#1545)
* You can add a member to a relation via the "All relations" section of the sidebar

## 1.0.1

* Test, imagery, translation, and preset updates
* Fix untranslatable strings
* Prefer to keep existing ways when joining
* Fix creating intersecting ways and cope with 0 and 1 node ways
* Fix IE detection in `dist`
* Fix GPX track display
* Fixes for Opera compatibility
* Update `osm-auth` to 0.2.1
* Fix the `note` functionality and textarea UI in presets
* Fix walkthrough translation issues
