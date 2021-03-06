## Shortcode syntax (proposed) for Tableau embed ##
```
[he-tableau name="{TABLEAU-FILENAME}" height="{INTEGER}" embed="{VERS_NUM}"]Text for interactive chart's caption, source, etc.[/he-tableau]
```

## Shortcode attributes and default values ##
| attr | setting | default | note |
| ---- | ------- | ------- | ------ |
| `name` | param: name | _(no default)_ |  |
| `height` | chart height | `650px` | |
| `width` | chart width | `100%` | 740px or 1000px 'widescreen' |
| `tabs` | param: tabs | `no` | |
| `share`  | param: showShareOptions | `true` | |
| `embed` | param: embed_code_version | `3` |  |
| `filter` | param: filter | `iframeSizedToWindow=true` | |
| `mobile` | param: filter | `yes` | |
| &#x1F538; | CSS class: wrapper  | `tableauPlaceholder` | Eg, for &lt;div&gt; |
| &#x1F538;  | CSS class: &lt;object&gt; | `tableauViz` | |
| &#x1F538;  | param: host_url | `https%3A%2F%2Ftableau.headwaterseconomics.org%2F` | |
| &#x1F538;  | param: site_root | `''` | |
| &#x1F538;  | param: toolbar | `no` | |
| &#x1F538;  | param: showAppBanner | `false` | | 

_(<sup>&#x1F538;</sup> Fixed value: not settable in shortcode)_

## Shortcode examples ##

So, these 5 shortcodes:

1. ```[he-tableau name="MinorityRuralWest7-1-17&#47;Dashboard1"]```

2. ```[he-tableau name="NPSVisitationHistory&#47;NPSVisitationHistory" height="510"]```

3. ```[he-tableau name="NonLabor2017&#47;MedicaidViz" height="490"]Source: Bureau of Economic Analysis, Regional Economic Accounts, 2015[/he-tableau]```

4.  ```[he-tableau name="MTHomes2-19-18&#47;MTHomesbyCounty" width="640" height="500" embed="2"]The four most populated counties--Gallatin County (Bozeman), Flathead County (Kalispell), Yellowstone County (Billings), and Missoula County (Missoula)--account for more than 50 percent of homes built since 2000. This <a href="https://headwaterseconomics.org/economic-development/local-studies/montana-home-construction-sortable-data">interactive table</a> sorts by county, homes built, open space lost, and other indicators.[/he-tableau]```

5. ```[he-tableau name="WhitefishTrails&#47;FlatheadTrailUse" height="857"]```

Would replace these existing Tableau HTML blocks:

```html
1. <div class='tableauPlaceholder' style='width: 749px; height: 650px;'>
<object class='tableauViz' width='749' height='650' style='display:none;'>
	<param name='host_url' value='https%3A%2F%2Ftableau.headwaterseconomics.org%2F' />
	<param name='site_root' value='' />
	<param name='name' value='MinorityRuralWest7-1-17&#47;Dashboard1' />
	<param name='tabs' value='no' />
	<param name='toolbar' value='no' />
	<param name='showShareOptions' value='true' />
</object>
</div>

2. <figure class='chart-responsive'>
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
</figure>

3. <div class='tableauPlaceholder' style='width: 744px; height: 490px;'>
<object class='tableauViz' width='744' height='490' style='display:none;'>
	<param name='host_url' value='https%3A%2F%2Ftableau.headwaterseconomics.org%2F' />
	<param name='site_root' value='' />
	<param name='name' value='NonLabor2017&#47;MedicaidViz' />
	<param name='tabs' value='no' />
	<param name='toolbar' value='no' />
	<param name='showShareOptions' value='true' />
</object>
</div>
<span style="font-size: small;"><em>Source: Bureau of Economic Analysis, Regional Economic Accounts, 2015</em></span>

4. <figure class="chart-stack">
<div class="tableauPlaceholder" style="width: 640px; height: 500px;">
<object class='tableauViz' width='640' height='500' style='display:none;'>
	<param name='host_url' value='https%3A%2F%2Ftableau.headwaterseconomics.org%2F' />
	<param name='embed_code_version' value='2' />
	<param name='site_root' value='' />
	<param name='name' value='MTHomes2-19-18&#47;MTHomesbyCounty' />
	<param name='tabs' value='no' />
	<param name='toolbar' value='no' />
	<param name='showAppBanner' value='false' />
	<param name='showShareOptions' value='true' />
</object>
</div>
<figcaption class="chart-stack-caption">The four most populated counties--Gallatin County (Bozeman), Flathead County (Kalispell), Yellowstone County (Billings), and Missoula County (Missoula)--account for more than 50 percent of homes built since 2000. This <a href="https://headwaterseconomics.org/economic-development/local-studies/montana-home-construction-sortable-data">interactive table</a> sorts by county, homes built, open space lost, and other indicators.</figcaption>
</figure>

5. <div class='tableauPlaceholder' style='width: 1000px; height: 857px;'>
<object class='tableauViz' width='1000' height='857' style='display:none;'>
	<param name='host_url' value='https%3A%2F%2Ftableau.headwaterseconomics.org%2F' />
	<param name='embed_code_version' value='3' />
	<param name='site_root' value='' />
	<param name='name' value='WhitefishTrails&#47;FlatheadTrailUse' />
	<param name='tabs' value='no' />
	<param name='toolbar' value='no' />
	<param name='showAppBanner' value='false' />
	<param name='filter' value='iframeSizedToWindow=true' />
</object>
</div>
```

## Reference ##
Tableau: [Parameters for Embed Code](https://onlinehelp.tableau.com/current/pro/desktop/en-us/embed_list.html)
