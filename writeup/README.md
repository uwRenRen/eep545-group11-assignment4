# Project 4: Planning [![tests](../../../badges/submit-proj4/pipeline.svg)](../../../pipelines/submit-proj4/latest)

Q6. 
The number of sampled vertices and connection radius were held constant at 40 and 4, respectively, while the maximum curvature was varied:
  -Curvature at 3 had a path length of 16.0869m and a shortcut path length of 13.8936m
  -Curvature at 4.5 had a path length of 14.7731m and a shortcut path length of 13.5019m
  -Curvature at 9 had a path length of 13.6062m and a shortcut path length of 12.9429m
  -Curvature at 15 had a path length of 13.2060m and a shortcut path length of 12.6398m
  
As the maximum curvature increases, the minimum turning radius decreases, allowing the car to make sharper turns and remove the need for the path to make an entire loop similar to path curvature 3 made near the bottom of the map. As the curvature increases, the circular loop disappears and the turns become sharper. The route also changes depending on the curvature. At curvatures of 3 and 9, the planner travels around the right side of the obstacle, whereas at curvatures of 4.5 and 15, the planner travels around the left side. Quantitatively, the path length decreases as the curvature increases from 3 to 15. The number of roadmap edges also increases from 347 to 451 because the higher curvature allows more configurations to be connected within the same connection radius.

Q7. 

κ = tan(δ) / L

Given a maximum steering angle of 0.34 radians and a wheelbase of 0.33 meters:

κ_max = tan(0.34) / 0.33

κ_max = 1.072 m⁻¹

The maximum curvature of the MuSHR car is approximately 1.072 m⁻¹
