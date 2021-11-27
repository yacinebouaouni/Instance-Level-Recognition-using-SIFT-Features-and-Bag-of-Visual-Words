# Instance-Level-Recognition-using-SIFT-Features

The goal of instance-level recognition is to match (recognize) a specific object or scene. Examples include recognizing a specific building, such as Notre Dame, or a specific painting, such as `Starry Night’ by Van Gogh. The object is recognized despite changes in scale, camera viewpoint, illumination conditions and partial occlusion. An important application is image retrieval - starting from an image of an object of interest (the query), search through an image dataset to obtain (or retrieve) those images that contain the target object.


## Part 1: 
Extract Sparse features using SIFT for matching specific objects in images. The matching will then be improved using Lowe’s second nearest neighbour test and by doing a geometric verification to keep the matches that exhibit a consistency over a certain transformation.

## Part 2: Compact descriptors for large scale image retrievel
The goal in large scale image retrievel is to find the match of a query image in a large database of images. This can be done by comparing the number of verified matches between the query and the images of the database using SIFT features, however, this will take a lot of time! 
Instead, we can compute a global descriptor that combines all the SIFT features using the bag-of-visual-words (BoVW) approach. This approach can even be more accelerated if used with a KDTree data structure.
