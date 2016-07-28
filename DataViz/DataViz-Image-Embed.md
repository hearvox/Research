<h1>Chart Images</h1>
How can <a href="http://headwaterseconomics.org/">Headwaters Economics</a> make our HE data charts easier for other sites to use? Our goals are to encourage:
<ul>
<li>Embedding HE images in external articles.</li>
<li>Citing HE in images used externally.</li>
<li>Linking back from the external images to the HE report.</li>
</ul>

First we'll look how other research and news sites present charts (static images, i.e., not interactives). What do they include in the image: the chart title, the data source(s), their site's name/logo? Also, is the image in an HTML link?

<em>The org name links to the article; the image links its full size:</a>
<table class="files">
<thead>
<tr>
<td></td>
<th scope="col">title</th>
<th scope="col">src</th>
<th scope="col">name</th>
<th scope="col">link</th>
<td></td>
</tr>
</thead>
<tbody>
<tr>
<td><a href="http://www.brookings.edu/research/reports/2016/06/16-informal-child-care-is-more-likely-to-harm-children-loeb">Brookings Institution</a><br />
Image links to model window (larger view of same image larger -- not a gallery).</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td><a href="http://www.brookings.edu/~/media/Research/Files/Reports/2016/06/16-informal-child-care-is-more-likely-to-harm-children-loeb/figure-1.png"><img src="http://www.brookings.edu/~/media/Research/Files/Reports/2016/06/16-informal-child-care-is-more-likely-to-harm-children-loeb/figure-1.png" width="340" /></a></td>
</tr>
<tr>
<td class="age"><a href="http://fivethirtyeight.com/features/the-jobs-recovery-may-not-be-flashy-but-its-strong/">FiveThirtyEight</a><br />
Site name and logo in image.</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td></td>
<td><a href="http://i2.wp.com/espnfivethirtyeight.files.wordpress.com/2016/07/casselman-julyjobs-1.png"><img src="http://i2.wp.com/espnfivethirtyeight.files.wordpress.com/2016/07/casselman-julyjobs-1.png" width="350" /></a></td>
</tr>
<tr>
<td><a href="https://www.theguardian.com/sustainable-business/2016/jul/02/america-solar-power-workforce-growing-market-solarcity-suniva">The Guardian</a></td>
<td>√</td>
<td></td>
<td></td>
<td></td>
<td><a href="https://i.guim.co.uk/img/media/913cb4b590085d0b0fe940f49f0b09e1ae7a10b9/0_0_882_593/master/882.jpg?w=620&q=20&auto=format&usm=12&fit=max&dpr=2&s=aa781b5445f87617e4a9befd5b26477a"><img src="https://i.guim.co.uk/img/media/913cb4b590085d0b0fe940f49f0b09e1ae7a10b9/0_0_882_593/master/882.jpg?w=620&q=20&auto=format&usm=12&fit=max&dpr=2&s=aa781b5445f87617e4a9befd5b26477a" width="350" /></a></td>
</tr>
<tr>
<td><a href="http://www.heritage.org/research/reports/2016/07/eliminate-favorable-treatment-of-biofuels">Heritage Foundation</a><br />
Image links to itself.</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td><a href="http://www.heritage.org/~/media/infographics/2016/07/bg3145/ud-ag-2016-biofuels-chart-5-corn-and-ethanol-prices-600.ashx"><img src="http://www.heritage.org/~/media/infographics/2016/07/bg3145/ud-ag-2016-biofuels-chart-5-corn-and-ethanol-prices-600.ashx?h=385&w=600" width="350" /></a></td>
</tr>
<tr>
<th scope="row"><a href="">NY Times</a></th>
<td>√</td>
<td>√</td>
<td>√</td>
<td></td>
<td><a href=""><img src="" width="300" /></a></td>
</tr>
<tr>
<th scope="row"><a href="">Pew Research Center</a></th>
<td>√</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td><a href=""><img src="" width="250" /></a></td>
</tr>
<tr>
<th scope="row"><a href="">YouGov</a></th>
<td>√</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td><a href=""><img src="" width="250" /></a></td>
</tr>
<tr>
<td><a href="https://www.propublica.org/article/unsafe-at-many-speeds">ProPublica</a><br />
<p>Use mostly interactives, very few static images.</p></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><a href="https://www.propublica.org/images/ngen/gypsy_image_630/20160525-lanewidthadapted-630.jpg"><img src="https://www.propublica.org/images/ngen/gypsy_image_630/20160525-lanewidthadapted-630.jpg" width="350" /></a></td>
</tr>
<tr>
<th scope="row"><a href=""></a></th>
<td>√</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td><a href=""><img src="" width="250" /></a></td>
</tr>
<tr>
<th scope="row"><a href="">Vox</a></th>
<td>√</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td><a href=""><img src="" width="250" /></a></td>
</tr>
<tr>
<th scope="row"><a href="">YouGov</a></th>
<td>√</td>
<td>√</td>
<td>√</td>
<td>√</td>
<td><a href=""><img src="" width="250" /></a></td>
</tr>
</tbody>
</table>

<h2>NY Times: SVG and CSS</h2>
The New York Times has few or now static images. All its charts seems to be either interactives, <a href="http://www.nytimes.com/2016/07/23/upshot/were-about-to-enter-a-period-of-polling-volatility.html#embedded-polling-averages">drawn using SVG</a>, or <a href="http://www.nytimes.com/2016/03/31/science/global-warming-antarctica-ice-sheet-sea-level-rise.html#g-antarctica-600">text styed with CSS</a>.

<h2>The Guardian: Social sharing images</h2>



