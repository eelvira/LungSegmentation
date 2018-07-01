# LungSegmentation

## Description
The threshold method consists of 4 steps: 
	      1) extraction of large airways;
        2) segmentation of lung regions;
        3) separation of the left and right lungs;
        4) smoothing.


## Motivation and Context
The algorithm includes errors in lung segmentation, which often occur at the borders of the lungs, when the contrast between the lung parenchyma and the surrounding tissue is low due to pathologic abnormalities that show up as dense regions. In normal lung anatomy, the shape of the costal lung surface is convex.
When an error occurs at the costal border, the surface is typically not convex anymore.

This problem was fixed with method, which was described in the work of [van Rikxoort et al.](https://www.ncbi.nlm.nih.gov/pubmed/19673192). Also bronchi and trachea were indicated and segmented in this method. 


## Screenshots :
You can see that the algorithm includes pathologies, whereas the ventricle isn't included in lungs area:
![big1](https://user-images.githubusercontent.com/22271721/33991932-b978a568-e0e1-11e7-94da-26c9d84a2a07.png)
![big2](https://user-images.githubusercontent.com/22271721/33991944-c81b3c98-e0e1-11e7-9d80-421e18dbfdd6.png)

Segmented lungs and trachea (bronchi) in frontal projection:
![3all](https://user-images.githubusercontent.com/22271721/33991962-d1af93ee-e0e1-11e7-9f2d-6a5eeabadf59.png)

![mesh_applied 3 -min](https://user-images.githubusercontent.com/22271721/33988348-32c6cb0a-e0d5-11e7-8b8a-b7a1cbfac080.gif)
