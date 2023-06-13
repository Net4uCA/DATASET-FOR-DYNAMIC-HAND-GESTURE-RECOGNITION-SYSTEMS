# DATASET-FOR-DYNAMIC-HAND-GESTURE-RECOGNITION-SYSTEMS
Computer vision systems are commonly used to design touch-less human-computer interfaces (HCI) based on dynamic hand gesture recognition (HGR) systems, which have a wide range of applications in several domains, such as, gaming, multimedia, automotive, home automation. However, automatic HGR is still a challenging task, mostly because of the diversity in how people perform the gestures. In addition, the number of publicly available hand gesture datasets is scarce, often the gestures are not acquired with sufficient image quality, and the gestures are not correctly performed. In this data article, we propose a dataset of 27 dynamic hand gesture types acquired at full HD resolution from 21 different subjects, which were carefully instructed before performing the gestures and monitored when performing the gesture; the subjects had to repeat the movement in case the performed hand gesture was not correct, i.e., the authors of this paper that were observing the gesture found that it did not correspond to the exact expected movement and/or the camera recorded a viewpoint did not allow for a plain visualizing of the gesture. Each subject performed 3 times the 27 hand gestures for a total of 1701 videos collected and corresponding 204120 video frames.
## If you make use of these datasets please consider citing the publication:
  Fronteddu, G., Porcu, S., Floris, A., & Atzori, L. (2022). A dynamic hand gesture recognition dataset for human-computer interfaces. Computer Networks, 205, 108781.
  
  BibTex format:
  
  @article{fronteddu2022dynamic,
  title={A dynamic hand gesture recognition dataset for human-computer interfaces},
  author={Fronteddu, Graziano and Porcu, Simone and Floris, Alessandro and Atzori, Luigi},
  journal={Computer Networks},
  volume={205},
  pages={108781},
  year={2022},
  publisher={Elsevier}
  }

## The dataset is available here.
https://ieee-dataport.org/documents/dataset-dynamic-hand-gesture-recognition-systems

## The associated results are presented here:
https://www.sciencedirect.com/science/article/pii/S1389128622000172

# Instructions: 
In the following, we discuss the details of the provided datasets.

hand_gestures_dataset_videos.zip - This dataset contains the videos of the recorded hand gestures. The zip contains 27 main folders. Each main folder refers to a hand gesture class, for a total of 27 main folders named “class_xx”, where “xx” identifies the class from 01 to 27. Within each of the class folders there are 21 sub-folders, one folder for each of the subjects that performed the hand gestures. These folders are named “Useryy_”, where “yy” identifies the user from 01 to 21. Each of the user folders contains three videos (.avi) corresponding to the three hand gestures performed by the user for each hand gesture class. The size of the full dataset is 21.34 GB.

 

HGD_VideoFrames_class_XX.zip - These datasets contain the video frames extracted from the videos of the recorded hand gestures. Each zip file contains the video frames of a hand gesture class, for a total of 27 zip files named “HGD_VideoFrames_class_XX.zip”, where “xx” identifies the class from 01 to 27. Therefore, each zip file contains one of the 27 class folders. Within each of the class folders there are 21 sub-folders, one folder for each of the subjects that performed the hand gestures. These folders are named “Useryy_”, where “yy” identifies the user from 01 to 21. Each of the user folders contains, in turn, 3 sub-folders, one folder for each of the three hand gestures performed for each hand gesture class. These sub-folders are named, respectively, “Useryy_1”, “Useryy_2”, and “Useryy_3”, and contain 120 video frames (.png) extracted from the corresponding video. The size of each zip file is about 9 GB.

 

hand_gesture_timing_stats.csv - This dataset contains timing information regarding the gestures performed by the subjects. The size of this dataset is 36 KB. It has 567 records plus the header. The meaning of the columns is as follows:

class: hand gesture class, from 01 to 27.

user: user who performed the hand gestures, from 01 to 21.

start_frame_1: starting frame related to the first performed hand gesture. It is a number between 0 and 119.

end_frame_1: ending frame related to the first performed hand gesture. It is a number between 0 and 119.

exec_time_1: execution time (in seconds) related to the first performed hand gesture. It is computed as the difference between the ending frame and the starting frame divided by the 30 fps set for video recording.

start_frame_2: starting frame related to the second performed hand gesture. It is a number between 0 and 119.

end_frame_2: ending frame related to the second performed hand gesture. It is a number between 0 and 119.

exec_time_2: execution time (in seconds) related to the second performed hand gesture. It is computed as the difference between the ending frame and the starting frame divided by the 30 fps set for video recording.

start_frame_3: starting frame related to the third performed hand gesture. It is a number between 0 and 119.

end_frame_3: ending frame related to the third performed hand gesture. It is a number between 0 and 119.

exec_time_3: execution time (in seconds) related to the third performed hand gesture. It is computed as the difference between the ending frame and the starting frame divided by the 30 fps set for video recording.

mean_exec_time: mean execution time (in seconds) for that related user and hand gesture. It is computed as the mean of the execution times computed for the three hand gestures performed by that user for that class.

std_dev_exec_time: standard deviation of the three execution times (in seconds) computed for the three hand gestures performed by that user for that class.

total_mean_exec_time: total mean execution time (in seconds) for that class. It is computed as the mean of all the execution times computed for the three hand gestures performed by all the users for that class.

total_std_dev_exec_time: total standard deviation of all the execution times (in seconds) for that class. It is computed as the standard deviation of all the execution times computed for the three hand gestures performed by all the users for that class. Note that in this case the standard deviation has been computed dividing by (N-1) as the entire population is considered.
