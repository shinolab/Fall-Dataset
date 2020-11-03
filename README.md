# FallDataset

This dataset contains 3D positions of body joints in disturbance-induced fall using kinect V2.

## LAYOUT
![図 002](https://user-images.githubusercontent.com/72964903/97974651-3f46a500-1e0b-11eb-892d-2e8ed51a8aac.jpeg)

## SUBJECTS

| Subject No.| Age | Weight [kg] |Height [cm]|Sex|
| ------ | ------ |------ | ------ | ------ |
| 1 | 24 | 48 | 164 | Male |
| 2 | 24 | 58 | 168 | Male |
| 3 | 24 | 65 | 178 | Male |
| 4 | 26 | 73 | 184 | Male |
| 5 | 27 | 58 | 167 | Male |
| 6 | 24 | 62 | 173 | Male |
| 7 | 23 | 66 | 168 | Male |
| 8 | 26 | 50 | 170 | Male |
| 9 | 24 | 50 | 167 | Male |
| 10 | 24 | - | 159 | Male |
| 11 | 23 | 70 | 175 | Male |


## DATASET STRUCTURE

```
├─fall : data including fall activity
│   └─11-folders : one per subject  
│       └─2-CSV files : each file including 50 fall activities
│         (*subject1 has 6 CSV files and subject11 has 1 CSV file)  
│           
└─walk : data including only gait
    └─1-folders :   only subject1 data  
        └─ 2-CSV files : each file including only gait    
```



## Description of columns in each CSV file (unit: m)
- [Columns 1-3] : Center Of Gravity X,Y,Z-axis (Calculated from the following joint data)
- [Columns 4] : Head X-axis
- [Columns 5] : Neck X-axis
- [Columns 6] : Spine Shoulder X-axis
- [Columns 7] : Spine Mid X-axis
- [Columns 8] : Spine Base X-axis
- [Columns 9] : Shoulder Right X-axis
- [Columns 10] : Elbow Right X-axis
- [Columns 11] : Wrist Right X-axis
- [Columns 12] : Hand Right X-axis
- [Columns 13] : Thumb Right X-axis
- [Columns 14] : Hand Tip Right X-axis
- [Columns 15] : Shoulder Left X-axis
- [Columns 16] : Elbow Left X-axis
- [Columns 17] : Wrist Left X-axis
- [Columns 18] : Hand Left X-axis
- [Columns 19] : Thumb Left X-axis
- [Columns 20] : Hand Tip Left X-axis
- [Columns 21] : Hip Right X-axis
- [Columns 22] : Knee Right X-axis
- [Columns 23] : Ankle Right X-axis
- [Columns 24] : Foot Right X-axis
- [Columns 25] : Hip Left X-axis
- [Columns 26] : Knee Left X-axis
- [Columns 27] : Ankle Left X-axis
- [Columns 28] : Foot Left X-axis
- [Columns 29-53] : Y-axis of [columns]6-28
- [Columns 54-78] : Z-axis of [columns]6-28
- [Columns 79] : Check the frame rate of kinect V2
- [Columns 80] : Fall instructions was Displaying or not (0:Not Displaying,1:Displaying)

![骨格の場所.003](/uploads/e6a63621664dc68a5b4d08e7d61286f2/骨格の場所.003.jpeg)


## Citing
If you use this dataset in your research please consider to include the following citation in your publications:  

R.Mori, T.Furukawa, Y.Makino, H.Shinoda "Measurement of Disturbance-Induced Fall Behavior and Prediction Using Neural Network", IEEE SMC2020
