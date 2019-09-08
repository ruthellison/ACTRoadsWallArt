# ACT Roads Wall Art
This project was created for the GovHack 2019 competition. You can access the project on the GovHack website here: https://hackerspace.govhack.org/team_management/teams/601
## Video
<iframe width="560" height="315" src="https://www.youtube.com/embed/UAAa_MpXMjY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
## Description
How do we use data from the past to predict a better future for Canberra and connect our citizens with their environment? We believe that predicting a better future for Canberra starts with appreciating what we currently have. The Canberra Roads Wall Art project helps connect our citizens to our local environment by turning a piece of every day Canberra - our transport road networks - into a beautiful piece of wall art that acts as a reminder of a piece of infrastructure that connects us all.

## Data story
We have produced 3 artworks based on the ACT Roads Centrelines dataset: https://www.data.act.gov.au/dataset/Road-Centrelines/r8wk-ud5i

### Initial processing:
1. Download ACT Roads Centrelines dataset
2. Extract and repackage each supplied dataset into separate zips
3. Use MapShaper.org to explore datasets
4. Extract border, road centrelines & road polygons to SVG
5. Import SVGs into illustrator
6. Observe that the road polygons from the Road Polygons datasets have significant artifacting, rendering them unusable for this project. We will work with the ACT Border and ACT Road Centrelines datasets

### Artwork 1 - All ACT map
A lasercut map of Canberra, with the border cut from wood and the road network engraved
1. Simplify paths to reduce node count.
2. Colour border separately so it can cut rather than engraved.
3. Test-cut a small section with a high density area.
4. Observe that the density is too high and these will need to be rastered.
5. Spend many hours trying to script detection of dense areas, eventually gave up and decided to raster all of the populated areas, leaving the rural roads as vector engraving to keep the cut time down
6. Import into Lightburn, set power & speeds for cuts & engraving
7. Cut on a sheet of Bunnings 3mm plywood


### Artwork 2 - CBD Map
A lasercut map of Canberra, focusing on the CBD & parliamentary zone, with the roads in wood and the space between removed.
1. Simplify paths to reduce node count.
2. Set stroke width to a visually appealing size.
3. Observe that some artifacting where strokes meet occurs, addressed by setting the stroke ends to round instead of square.
4. Outline all strokes.
5. Merge the outlines into a single outline.
6. Stroke a rectangle around the piece for a border. Duplicate it, and use the duplicate as a clipping mask. Use the clipping to crop the roads.
7. Outline the border and merge it with the road network.
8. Import into Lightburn, set power & speeds for cuts
9. Cut on a sheet of Bunnings 3mm plywood

### Artwork 3 - CBD Map coasters
A subsection of artwork 2, scaled & cut on acacia coasters
1. Take the saved work from Step 5 of artwork 2
2. Create a circular crop centred on Parliament House
3. Import into Lightburn, set power & speeds for cuts
4. Create a wider circle based on the caoster diameter
5. Cut the wider circle out of scrap, we will use this to position the coaster accurately in the laser
6. Engrave the artwork onto the coaster
