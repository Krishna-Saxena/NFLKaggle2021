# NFLKaggle2021
Problem Statement: match all helmets in an image frame to players on the field.
My solution
- Affine transform the known helmets in the frame to field coordinates
- Define a custom similarity metric for translated vectors and all players' field coordinates
- Use the Gale-Shapely algorithm to find stable matches between known players' field coordinates and transformed vectors
- Use ADAM to find optimal parameters for the affine transform
- Use affine transform to predict remaining players' image coordinates