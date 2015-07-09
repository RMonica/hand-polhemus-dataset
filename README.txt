Author: Riccardo Monica <rmonica[at]ce.unipr.it>
  RIMLab, Department of Information Engineering, University of Parma, Italy
  http://www.rimlab.ce.unipr.it/

2015 07 09

This dataset contains 330 trajectories recorded with the FasTrak Polhemus sensor. The sensor acquired the movement of the hand of an user while performing some simple activities on a table. The sensor was fastened to the user's wrist and recorded its translation and rotation with respect to a base placed on the table.
The recording started automatically when the hand entered the bounding box fitted above the table surface. The table size was about 2.0x1.4 meters, and the user was located near one of the long sides of the table. The user was asked to place the object randomly on the table.
The trajectories were sampled at 100Hz.

Four different users took part in the experiment.
The 220 trajectories in the placements_removals directory are produced by users with the task of adding or removing a single object from the table, and then leave the workspace.
The 110 trajectories in the pick_and_place directory are produced by users with the task of picking an object, placing it to another position, and then leave the workspace.

The files containing the trajectories are named as follow:
user[U]_[object_name][N].traj
where
- [U] is an anonymous numeric user identifier;
- [object_name] is the name of the moved object;
- [N] is an incremental identifier of the trajectory.

Trajectory files are text files, containing an array of 4x4 transformation matrices, each corresponding to a sample from the sensor. Each matrix is represented as four lines of four numbers in text form, followed by a blank line.

For each trajectory, a ground truth is supplied in a text file with the same name and the ".res" suffix. This file contains the coordinates at which the actual changes occurred in the environment, obtained by manual labelling (human error may have occurred). The file can contain multiple lines, with three numbers in each, corresponding to the coordinates XYZ of each change.

-- COPYRIGHT NOTICE --
Copyright (C) 2014-2015 Riccardo Monica
  RIMLab, Department of Information Engineering, University of Parma, Italy
  http://www.rimlab.ce.unipr.it/

To the extent possible under law, Riccardo Monica has waived all copyright and related or neighboring rights to this dataset.
  http://creativecommons.org/publicdomain/zero/1.0/
