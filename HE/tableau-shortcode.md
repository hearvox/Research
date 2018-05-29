
HTML element =	CSS class (settable in shortcode)
--------------------------------------------------
wrapper class =	tableauPlaceholder (eg, for <div>)
<object> class =	tableauViz

HTML element =	CSS size (settable in shortcode)
--------------------------------------------------
width =	100% (so 740px, except 1000px for 'widescreen' post or 'Widescreen' template page)
height = 650px

Param: default value (settable in shortcode)
--------------------------------------------------
embed_code_version =	3
site_root = 	''
tabs 

Param (only settable in shortcode -- no default value)
--------------------------------------------------
name

Param =	fixed value (not settable in shortcode)
--------------------------------------------------
host_url =	https%3A%2F%2Ftableau.headwaterseconomics.org%2F
tabs = 	no
toolbar =	no
showShareOptions =	true
showAppBanner =	false
filter =	iframeSizedToWindow=true

So these 5 shortcodes:

[he-tableau name="NPSVisitationHistory&#47;NPSVisitationHistory" height="510"]

[he-tableau name="MinorityRuralWest7-1-17&#47;Dashboard1"]

[he-tableau name="NonLabor2017&#47;MedicaidViz" height="490"]Source: Bureau of Economic Analysis, Regional Economic Accounts, 2015[/he-tableau]


[he-tableau name="MTHomes2-19-18&#47;MTHomesbyCounty" width="640" height="500" embed="2"]The four most populated counties--Gallatin County (Bozeman), Flathead County (Kalispell), Yellowstone County (Billings), and Missoula County (Missoula)--account for more than 50 percent of homes built since 2000. This <a href="https://headwaterseconomics.org/economic-development/local-studies/montana-home-construction-sortable-data">interactive table</a> sorts by county, homes built, open space lost, and other indicators.[/he-tableau]

[he-tableau name="WhitefishTrails&#47;FlatheadTrailUse" height="857"]

Would work for these existing Tableaus:

```html
<figure class='chart-responsive'>
<div class='tableauPlaceholder' style='width: 750px; height: 510px;'>
<object class='tableauViz' width='750' height='510' style='display:none;'>
	<param name='host_url' value='https%3A%2F%2Ftableau.headwaterseconomics.org%2F' />
	<param name='embed_code_version' value='3' /> 
	<param name='site_root' value='' />
	<param name='name' value='NPSVisitationHistory&#47;NPSVisitationHistory' />
	<param name='tabs' value='no' />
	<param name='toolbar' value='no' />
	<param name='showAppBanner' value='false' />
	<param name='filter' value='iframeSizedToWindow=true' />
</object>
</div>
```
