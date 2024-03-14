# AmbulanceDetection
Documentation of ambulance detection using computer vision
Abstract
The number of vehicles has increased in recent days. Managing this huge number of vehicles is a tedious process. Traffic Signals are used to control the flow of the vehicles in an orderly manner. Sometimes an ambulance may need to wait for a long time in a traffic signal and if it waits for too long, it would put the patient’s life at risk. Traffic police can manually identify an ambulance and try to clear the traffic jam, but it is not possible with today’s enormous vehicles. Detection of Ambulance using Computer Vision is an application of computer vision and image processing which is capable of extracting images of vehicles and detecting ambulance. It is implemented using Python, OpenCV, TensorFlow and CNN. It captures the live feed of traffic using a camera and extracts the vehicles. Then it is classified as an ambulance or non-ambulatory vehicle. By automating this process, it is possible to clear a way for an ambulance that is waiting in a traffic signal.

Introduction
Emergency vehicles play an important role in every life-threatening situation. Traffic jam takes more than 20% of patients' lives in an ambulance but when the patient’s condition is very serious the percentage of patient deaths is increased. These are situations when an emergency patient needs to go to the hospital immediately and the ambulance gets stuck in a traffic jam. This scenario is dangerous in the case of heart patients who need to be rushed to the hospital in time. In traffic jams, many people do not bother to give a pass-way for the emergency vehicle and also traffic police can’t see which lane they should clear for the ambulance. Therefore, many patients lose their lives before reaching hospitals.
We can reduce these problems by introducing an intelligent automated system integrated with a traffic control system that will detect and give priority to emergency vehicles. We need to build a system to detect cars and classify them as an emergency or regular car. After detecting every vehicle, they have classified it into an emergency vehicle and regular vehicles. If an emergency vehicle is found, the computer can notify the traffic police or an automated system to clear its way.

❖	Introduction to Existing Systems
Traffic problems nowadays are increasing because of the growing number of vehicles and the limited resources provided by current infrastructures. The simplest way of controlling a traffic light use a timer for each phase in a round-robin fashion. Another way is to use electronic sensors to capture the location of the vehicle and check whether it is waiting for a signal or not. This method requires installing some sensors in that particular vehicle, which is impossible for the huge number of vehicles available.

	Problem with Existing Systems
RFIDs and Bluetooth in the existing work have been used in vehicle detection for a long time. These devices however have a few drawbacks when being used for detecting vehicles:
★ The number of devices required to be installed for vehicle detection is increased.
★ Since more devices are bought, the cost is high.
★ Due to the low response speed, the connection takes time to be established.
★ Have a low range, hence it requires to be placed at every diametrical distance from the last device, for greater accuracy.

❖	Need for Improvement (Scope for Improvement)
➔	The accuracy of the classification model is around 84%. This can be improved to more than 95% for a more reliable model
➔	A User Interface can be created to use this software with ease.
➔	Adding a feature for live tracking of the ambulance through the traffic for better navigation.

 

❖	Objectives
(Learning model , model implementation , Problem Understanding, Title, Goal, Objective of the Project)
In our work, the only piece of hardware we propose to use is the surveillance camera itself. The system will detect vehicles through images instead of using electronic sensors embedded in the pavement. A camera will be installed within certain distances from the traffic light it will capture the footage of the vehicles at regular intervals. The captured footage is then converted to frames and the YOLO algorithm is used to extract the vehicles. The extracted images are then processed by our CNN model to detect whether it is an ambulance or not.
Advantages :

●	Fewer types of equipment needed
●	Fully automated system
●	Highly scalable

Develop Detection Algorithms: Design and implement computer vision and/or sensor-based algorithms capable occurately detecting and recognizing ambulances in real-time.

Integrate with Traffic Infrastructure: Establish communication protocols between the detection system and existing traffic management infrastructure to prioritize the passage of ambulances at intersections and along congested routes.
Enhance Response Coordination: Enable seamless integration with emergency services dispatch systems to provide timely information on ambulance locations and optimize response coordination.
Evaluate System Performance: Conduct rigorous testing and evaluation of the system's performance under various traffic conditions and emergency scenarios to ensure reliability and effectiveness.
Deploy and Iterate: Deploy the system in a pilot area and gather feedback from emergency responders, traffic authorities, and the public. Use this feedback to refine and iterate upon the system for continuous improvement.
Project Outcomes:
• Understand the context of neural networks and deep learning. 
• Have a working knowledge of neural networks and deep learning. 
• Explore the parameters for neural networks. 
• Use CNN and RNN for solving real world problem. 


❖	Problem State Definition
The project aims to develop a robust ambulance detection system that significantly improves emergency response capabilities and contributes to saving lives in critical situations.
Literature Survey
[1]	K Agrawal1, M K Nigam1, S Bhattacharya1, and Sumathi G1 published paperwork in 2021, for Ambulance Detection using Image Processing and Neural Network which is a vehicle detection and tracking system, that recognizes the vehicle (i.e., Ambulance in this case) amidst the traffic congestion. According to their work, The Ambulance tracking system is activated at the mapped junctions and that program detects the ambulance coming close to it and turns the traffic light to Green for the next 15 seconds. Geocoding is the practice of transforming addresses (like a physical address) to location information (like longitude and latitude) that can be used to locate a label on a map or to mark a grid. They plan to provide ambulances with this software to make it easy to transform addresses into a programmable format for review and retrieval. This data is converted to a system that shows all the crossings it must pass to meet the endpoint.
Link :
(PDF) Ambulance detection using image processing and neural networks
https://www.researchgate.net/publication/356515102_Ambulance_detection_using_image_proces sing_and_neural_networks
[2]	In 2018, Shuvendu Roy1, Md. Sakif Rahman2 have proposed an automated system to detect emergency cars from CCTV footage using the deep convolutional neural network. Their method has shown good results in detecting and classifying emergency cars.
Link :
Emergency Vehicle Detection on Heavy Traffic Road from CCTV Footage Using Deep Convolutional Neural Network | Semantic Scholar
https://www.semanticscholar.org/paper/Emergency-Vehicle-Detection-on-Heavy-Traffic-Road-
Roy-Rahman/38f8b6cd3762778425145cd19e540dbd9ba9d7c2
[3]	Huansheng Song, Haoxiang Liang, Huaiyu Li, and Zhe Dai Xu Yun in 2019, published their work that discusses the challenges that directly affect the accuracy of vehicle counts, due to the different sizes of vehicles. To address this, they have proposed a vision-based vehicle detection and counting system. A new high-definition highway vehicle dataset with a total of 57,290 annotated instances in 11,129 images is published in this study. Compared with the existing public datasets, the proposed dataset contains annotated tiny objects in the image, which provides the complete data foundation for vehicle detection based on deep learning. The experimental results verify that using the proposed segmentation method can provide higher detection accuracy, especially for the detection of small vehicle objects. Moreover, the novel strategy described in this article performs notably well in judging driving direction and counting vehicles. This paper has general practical significance for the management and control of highway scenes.
Link :

Vision-based vehicle detection and counting system using deep learning in highway scenes | European Transport Research Review
https://etrr.springeropen.com/articles/10.1186/s12544-019-0390-4

used to locate a label on a map or to mark a grid. They plan to provide ambulances with this software to make it easy to transform addresses into a programmable format for review and retrieval. This data is converted to a system that shows all the crossings it must pass to meet the endpoint.
Link :
(PDF) Ambulance detection using image processing and neural networks
https://www.researchgate.net/publication/356515102_Ambulance_detection_using_image_proces sing_and_neural_networks
[4]	In 2018, Shuvendu Roy1, Md. Sakif Rahman2 have proposed an automated system to detect emergency cars from CCTV footage using the deep convolutional neural network. Their method has shown good results in detecting and classifying emergency cars.
Link :
Emergency Vehicle Detection on Heavy Traffic Road from CCTV Footage Using Deep Convolutional Neural Network | Semantic Scholar
https://www.semanticscholar.org/paper/Emergency-Vehicle-Detection-on-Heavy-Traffic-Road-
Roy-Rahman/38f8b6cd3762778425145cd19e540dbd9ba9d7c2

[5]	Huansheng Song, Haoxiang Liang, Huaiyu Li, and Zhe Dai Xu Yun in 2019, published their work that discusses the challenges that directly affect the accuracy of vehicle counts, due to the different sizes of vehicles. To address this, they have proposed a vision-based vehicle detection and counting system. A new high-definition highway vehicle dataset with a total of 57,290 annotated instances in 11,129 images is published in this study. Compared with the existing public datasets, the proposed dataset contains annotated tiny objects in the image, which provides the complete data foundation for vehicle detection based on deep learning. The experimental results verify that using the proposed segmentation method can provide higher detection accuracy, especially for the detection of small vehicle objects. Moreover, the novel strategy described in this article performs notably well in judging driving direction and counting vehicles. This paper has general practical significance for the management and control of highway scenes.
Link :

Vision-based vehicle detection and counting system using deep learning in highway scenes | European Transport Research Review
https://etrr.springeropen.com/articles/10.1186/s12544-019-0390-4
 

In 2019, K.Rubini, M.Vidhya, S.R Yeshawini, and A.Gowthami proposed an idea that focuses on controlling the speed of the surrounding vehicles near an ambulance, so hence the ambulance can reach the hospital on time. It can be done by using RSSI (Received Signal Strength Indication) which works based on the Message Queuing Telemetry Transport algorithm. Node MCU acts as transmitter and server acts as receiver. Node MCU has an inbuilt Wi-Fi module (EP8266). It receives the signal from the server and identifies that signal strength which is used to reduce the speed of other vehicles within the particular limit. An APR voice module is used to provide intimation to the surrounding vehicles about the arrival of the ambulance. Also, the traffic for the ambulance to reach without time lag. The original signal is again restored once the ambulance moves over a particular distance from the signal that has been fixed earlier.
Link :

Automatic Ambulance Detection and Intimation Using RSSI https://www.ijeter.everscience.org/Manuscripts/Volume-7/Issue-3/Vol-7-issue-3-M-07.pdf
[6]	Kapileswar Nellore and Gerhard P. Hancke proposed their idea in 2016. This paper presents an approach to scheduling emergency vehicles in traffic. The approach combines the measurement of the distance between the emergency vehicle and an intersection using visual sensing methods, vehicle counting and time-sensitive alert transmission within the sensor network. The distance between the emergency vehicle and the intersection is calculated for comparison using Euclidean distance, Manhattan distance and Canberra distance techniques.

Link :
Traffic Management for Emergency Vehicle Priority Based on Visual Sensing https://pubmed.ncbi.nlm.nih.gov/27834924/


METHODOLOGY
(Dataset : ½ page of dataset description Block diagram
Algorithms Steps )

The proposed methodology is implemented in Python and packages include the following:
➢	Tensorflow
➢	CNN
➢	YOLO
➢	Keras
➢	Open CV

IMPLEMENTATION :
The implementation is segregated into 4 Modules and considered as 2 Phases as follows:
The videos captured by the camera sensor are converted into images and these images are processed by various algorithms finally, the program gives the output whether the vehicle detected is an ambulance to not. After that, it will alert the user if the ambulance is present or not.

A.	Training
Before the detection of the vehicle and giving output based on the result, the machine must be taught what an ambulance looks like. For this, we created a tiny dataset consisting of a thousand images, and a model must be trained which will be called in the confirmation segment.TensorFlow 2.1.0 algorithm is particularly used to avoid compatibility issues and is installed. Validation and trained images generated after training are stored in their respective folders in Google Drive and the drive is linked to the training algorithm. Matplotlib is used to give the output graphs.
Pre-Processing: More than 1000 images were downloaded from various internet sources and given as input for training to generate a trained dataset that can be used for detection. ImageDataGenerator function is used to manipulate the existing images and make more copies, to increase the dataset size Train generator and Validation generator functions are used to resize and segregate the images and save them in Train and Validation folders in the drive, both have 2 folders each - 0 and 1, Images that have ambulance are saved in 1 and others in 0. Batch size for training the data is set as 32 and the images are resized to 224x224 pixels.
Training: After the pre-processing, the standard TensorFlow algorithm runs to train the dataset. Using the Keras open-source library, a sequential list is created. As we are working on CNN, 4 layers of 2D convolutions are set, and after each convolution – The max-pooling operation runs and the least relevant results are dropped out. The whole process runs 20 times (epochs = 20) and takes a maximum of 25 minutes.
Combining: After training the whole data is combined and optimized using adam optimizer and losses are calculated to make the model more efficient. Using the Fit generator, the model is created, and later, it is saved in the drive folder. The whole model is based on the metrics of accuracy and loss.

B.	Detection
It takes place in several steps and includes 3 modules:
➢	Frames Extraction
➢	YOLO Detection
➢	Image Classification
1.Frames Extraction: Camera Sensor captures small video clips of traffic; these Clips are taken as input and are sent to the processor. Clips are converted into pictures and are sent for processing.

2.YOLO Detection: Images in the overall folder go to the YOLO program that detects if the vehicle is a truck. It is a predefined algorithm that uses the COCO dataset developed by Microsoft. YOLO algorithm detects whether the image that is passed through it contains are ambulance     or not.
If the vehicle qualifies as an ambulance, then a copy of these images is saved in the “detected” folder  after adding a bounding box around it.

3.Image Classification: The image then passes to the main function, where our model is called,
   and the image is processed to check if it is an ambulance. If it qualifies as an ambulance then,  it will be labelled as  “ambulance” on the outer box or the labelling box. 




Flow chart of detection process

