# Key_point_extracting_from_face
KEY POINT EXTRACTION FROM FACE

The objective of this task is to predict keypoint positions on face images. This can be used as a building block in several applications, such as:
•	tracking faces in images and video
•	analysing facial expressions
•	detecting dysmorphic facial signs for medical diagnosis
•	biometrics / face recognition
Detecing facial keypoints is a very challenging problem.  Facial features vary greatly from one individual to another, and even for a single individual, there is a large amount of variation due to 3D pose, size, position, viewing angle, and illumination conditions. Computer vision research has come a long way in addressing these difficulties, but there remain many opportunities for improvement.

To train the model I experimented with various batch sizes. Large batch sizes trained quickly and gave good results while smaller batches gave slightly better results though took longer to train. While playing with this parameter I took a trained model and ran the training process on it again using a different batch size and ended up with a better model than either batch size had produced alone. This, in part, lead me to construct an iterative training regime consisting of multiple stepwise annealings with decreasing batch sizes for each annealing cycle. With each cycle the model approached the loss of the previous cycle and surpassed it.
