[IEEE Xplore Conference Paper](https://ieeexplore.ieee.org/document/10816793)

Railway safety is a significant challenge, especially in countries with large rail networks, such as India, which carries billions of passengers and freight every year. Unwanted human presence on railway tracks kills thousands of people every year—over 26,000 lives were lost in India in 2021 alone. This is a stark reminder of the need for innovative, technology-driven safety solutions.

With the power of artificial intelligence, a new system has been designed to tackle this problem, integrating object detection and activity recognition. The system uses YOLO-V8 (You Only Look Once Version 8), one of the advanced algorithms in object detection, to monitor railway tracks in real time, detect human presence, and recognize activities such as standing, sitting, or lying down—all leading to more safety and accidents prevented.

## Revolutionizing Railway Safety with AI
- Traditional safety measures like manual surveillance, physical barriers, and CCTV monitoring often fall short due to scalability issues, high costs, and limited coverage. In contrast, AI-powered systems offer real-time monitoring, high accuracy, and adaptability across diverse conditions.
- It employs a robust dataset with state-of-the-art detection techniques for the identification and categorization of human activities on railway tracks. It fills a critical gap in current railway safety measures and offers a scalable solution for effectively preventing accidents.

## Key Components of the System
1. Data Collection and Annotation
- A robust dataset is a must to train AI models. For achieving accuracy, over 3,700 high-resolution images were gathered using a Samsung GN5 sensor. The diversity of scenarios the dataset accounted for included different times of day such as day, night, dawn, and dusk and varying weather conditions such as clear skies, rain, and fog. Roboflow was used to annotate because of its accuracy and user-friendly interface. Using its interface, a bounding box around humans in poses such as standing, sitting, or lying on the tracks was applied along with any other objects relevant to these images. This was reviewed minutely for few errors, providing the highest possible quality data.
2. Detection using YOLO-V8
- The backbone algorithm of this system is the YOLO-V8 algorithm. This algorithm was selected due to its real-time capabilities and better accuracy. Google Colab's T4 GPU is used for the training of this model with a batch size of 16 and optimized with the AdamW optimizer. 
 Data augmentation techniques, including horizontal flipping, rotation, brightness adjustments, and grayscale conversion, were used to increase the diversity of the dataset. These steps improved the robustness of the system, allowing it to work well in real-world conditions, such as low visibility and occlusions.
3. Performance Metrics and Evaluation
- The system was tested using key performance metrics: Mean Average Precision (mAP50): 92.3% score, which means that the system is highly accurate in detecting objects with moderate overlap.
4.Real-World Impact and Applications
- This AI-based solution has proved to be highly promising in addressing railway safety issues. With proper human activity detection, it can send timely notifications that may prevent accidents and casualties. Integrated with real-time notification systems to the train operators and nearby stations will increase its efficiency.
5. Expanding System Capabilities
- Although the system currently detects stationary activities like standing, sitting, or lying down, in the future, it can be given more wide-ranging scenarios such as crowded platforms or crossing pedestrians. It could be augmented with additional sensor inputs, thermal imaging would provide detection with a better accuracy in low light.

## Conclusion
AI-powered systems are radically changing transportation safety. This innovative approach here clearly demonstrates what great potential these technologies hold to save lives. Combining YOLO-V8 with a well-annotated dataset, the system gives an efficient, scalable, and accurate solution to prevent railway accidents. If these technologies flourish further, they may seamlessly become a part of intelligent transportation networks all over the world, and thus make railways safer for all.
