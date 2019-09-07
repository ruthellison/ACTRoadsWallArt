# ACT Roads Wall Art
This project was created for the GovHack 2019 competition. You can access the project on the GovHack website here: https://hackerspace.govhack.org/team_management/teams/601
## Video
Video to be inserted here
## Description
How do we use data from the past to predict a better future for Canberra? Connect our citizens with their environment? We believe that predicting a better future for Canberra starts with appreciating what we currently have. The ACT Roads Wall Art project helps connect our citizens to our local environment by turning a piece of every day Canberra - our transport road networks - into a beautiful piece of wall art that acts as a reminder of a piece of infrastructure that connects us all.

## Data story
How we arrived at this project

## Workflow
1. Download ACT Roads Centrelines dataset
2. Extract and repackage each supplied dataset into separate zips
3. Use MapShaper.org to explore datasets
4. Extract border, road centrelines & road polygons to SVG
4. Import SVGs into illustrator
5. Observe that the road polygons have significant artifacting, rendering them unusable for this project

### Artwork 1 - All ACT map
A lasercut map of Canberra, with the border cut from wood and the road network engraved
1. Simplify paths to reduce node count.
2. Colour border separately so it can cut rather than engraved.
3. Test-cut a small section with a high density area.
4. Observe that the density is too high and these will need to be rastered.

Artwork 2 - CBD Map
1. A lasercut map of Canberra, focusing on the CBD & parliamentary zone, with the roads in wood and the space between removed
2. Simplify paths to reduce node count.
3. Set stroke width to a visually appealing size.
4. Observe that some artifacting where strokes meet occurs, addressed by setting the stroke ends to round instead of square.
5. Outline all strokes.
6. Merge the outlines into a single outline.
7. Stroke a rectangle around the piece for a border. Duplicate it, and use the duplicate as a clipping mask. Use the clipping to crop the roads.
8. Outline the border and merge it with the road network. 
9. Import into Lightburn, set power & speeds for cuts
10. Cut on a sheet of Bunnings 3mm plywood

