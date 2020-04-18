# Searching for electromagnetic showers

In this project, the goal is to design a prediction model that is able to discriminate the basetracks belonging to the electromagnetic showers from the background basetracks. The goal is to get the best possible score (ROC AUC). 

## The data files:

https://github.com/hse-aml/hadron-collider-machine-learning/releases/download/Week_4/training.tgz - archive with brick volumes filled with labeled basetracks
https://github.com/hse-aml/hadron-collider-machine-learning/releases/download/Week_4/test.h5.gz - volume with basetracks to discriminate

Each BaseTrack (BT) is described by:

- Coordinates: (X, Y, Z)

- Angles in the brick-frame: (TX, TY)

After the 'add_neighbours' we add dX,dY,dZ,dTX,dTY (distance from the origin) and group close tracks from neighbour plates into pairs.
