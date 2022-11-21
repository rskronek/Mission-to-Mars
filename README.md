# Mission to Mars
In this module, I automated a web browser to visit different websites to extract data about the Mission to Mars. I stored it in a NoSQL database, and then rendered the data in a web application created with Flask.


### Bootstrap and other changes
 * Changed to background color of webpage to black and the font color to white to match that of NASA.gov
 * Imported from Google the font _Titillium Web_ and set as the default page font, because that is the font used on NASA.gov
 * Backroung color of the `jumbotron` component changed to the same blue used on the NASA.gov website
 * **Scarpe New Data** button changed from `btn-primary` to `btn-danger` to match the red, white, blue, and black theme of the NASA.gov website.
and the `active` class added
 * Data table alternating row color also changed to use NASA blue
 * Mars hemisphere DIVs class changed from `col-md-6` to `col-md-3` so all four images can fit on one row in desktop mode

### MongoDB contents
```json
[
  {
    _id: ObjectId("63785e9fa4f1dabb946742d0"),
    facts: '<table border="1" class="dataframe table table-striped">\n' +
      '  <thead>\n' +
      '    <tr style="text-align: right;">\n' +
      '      <th></th>\n' +
      '      <th>Mars</th>\n' +
      '      <th>Earth</th>\n' +
      '    </tr>\n' +
      '    <tr>\n' +
      '      <th>Description</th>\n' +
      '      <th></th>\n' +
      '      <th></th>\n' +
      '    </tr>\n' +
      '  </thead>\n' +
      '  <tbody>\n' +
      '    <tr>\n' +
      '      <th>Mars - Earth Comparison</th>\n' +
      '      <td>Mars</td>\n' +
      '      <td>Earth</td>\n' +
      '    </tr>\n' +
      '    <tr>\n' +
      '      <th>Diameter:</th>\n' +
      '      <td>6,779 km</td>\n' +
      '      <td>12,742 km</td>\n' +
      '    </tr>\n' +
      '    <tr>\n' +
      '      <th>Mass:</th>\n' +
      '      <td>6.39 × 10^23 kg</td>\n' +
      '      <td>5.97 × 10^24 kg</td>\n' +
      '    </tr>\n' +
      '    <tr>\n' +
      '      <th>Moons:</th>\n' +
      '      <td>2</td>\n' +
      '      <td>1</td>\n' +
      '    </tr>\n' +
      '    <tr>\n' +
      '      <th>Distance from Sun:</th>\n' +
      '      <td>227,943,824 km</td>\n' +
      '      <td>149,598,262 km</td>\n' +
      '    </tr>\n' +
      '    <tr>\n' +
      '      <th>Length of Year:</th>\n' +
      '      <td>687 Earth days</td>\n' +
      '      <td>365.24 days</td>\n' +
      '    </tr>\n' +
      '    <tr>\n' +
      '      <th>Temperature:</th>\n' +
      '      <td>-87 to -5 °C</td>\n' +
      '      <td>-88 to 58°C</td>\n' +
      '    </tr>\n' +
      '  </tbody>\n' +
      '</table>',
    featured_image: 'https://data-class-jpl-space.s3.amazonaws.com/JPL_Space/image/featured/mars2.jpg',
    last_modified: ISODate("2022-11-20T10:26:17.606Z"),
    news_paragraph: 'During this next phase, the program will mature critical technologies and make critical design decisions as well as assess industry partnerships.',
    news_title: 'NASA Moves Forward With Campaign to Return Mars Samples to Earth',
    hemispheres: [
      {
        title: 'Cerberus Hemisphere Enhanced',
        img_url: 'https://marshemispheres.com/images/full.jpg'
      },
      {
        title: 'Schiaparelli Hemisphere Enhanced',
        img_url: 'https://marshemispheres.com/images/schiaparelli_enhanced-full.jpg'
      },
      {
        title: 'Syrtis Major Hemisphere Enhanced',
        img_url: 'https://marshemispheres.com/images/syrtis_major_enhanced-full.jpg'
      },
      {
        title: 'Valles Marineris Hemisphere Enhanced',
        img_url: 'https://marshemispheres.com/images/valles_marineris_enhanced-full.jpg'
      }
    ]
  }
]
```