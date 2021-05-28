# Project6-Alzheimer-s-Disease-Classification-
Diffusion tensor imaging (DTI) has been widely utilized to demonstrate structural integrity and define white matter loss in Alzheimer's disease (AD) using diffusion characteristics. It has been demonstrated that WM integrity measurements are useful in classifying AD using machine learning.
The primary goal of this research is to create machine learning-based classification models that can successfully differentiate Alzheimer's disease (AD) from Normal Control, Mild cognitive impairment (MCI) from Normal Control (NC), and Mild cognitive impairment (MCI) from Alzheimer's disease (AD).

DATA:
Exploratory Analysis:
Each of the above matrices were explored and some exploratory analyses were performed to look at the
distribution of AD, MCI and NC amongst the patients/subjects of the dataset.
Figure 2: Showing the proportion of male to female in the data.
As can be seen in the figure above the majority of the subjects consists of Females and the minority are males.![image](https://user-images.githubusercontent.com/80302702/120034871-0b4dfe00-c041-11eb-9ef8-1d9697983956.png)

Females are about 57.43% whereas male patients are about 42.57%. This can be further be explored to check
the distribution of gender amongst the three classes of NC, MCI and AD.

As can be seen in the figure above the majority of the subjects consists of Females and the minority are males.
Females are about 57.43% whereas male patients are about 42.57%. This can be further be explored to check
the distribution of gender amongst the three classes of NC, MCI and AD.
![image](https://user-images.githubusercontent.com/80302702/120034957-29b3f980-c041-11eb-89a7-c30d50bfd073.png)
As can be seen above most of the subjects or patients in the data set consists of females. In class 1 which
consists of patients with Normal and healthy brain male subject are about 97 and females are 138. In class 2
which contains subjects of Mild cognitive impairment, in this class males are about 99 and females are 116.
Class 3 is of AD patients which is of 148 female patients and 102 males.
![image](https://user-images.githubusercontent.com/80302702/120034992-37697f00-c041-11eb-9cd5-f0931e6eac32.png)
Details:
Load data
Matlab
Load(‘MCAD_Load(‘MCAD_AFQ
_competition ')
Python
from scipy.io import loadmat

data = loadmat(‘MCAD_AFQ_competition_competition.mat’, mat_dtype=True).mat’, mat_dtype=True)
R
library(R.matlab)
nms<--readMat (‘MCAD_AFQreadMat (‘MCAD_AFQ_competition_competition.mat’).mat’)
If you load the data successfully, the following matrices will show
Train_diagnoseTrain_diagnose: :
This matrix contains diagnosis information for each subject. Numeral 1 means normal controlnormal control (NC). (NC). Similarly, Numeral Similarly, Numeral 2 represents mild cognitive impairment (MCI), and numeral 3 represents represents mild cognitive impairment (MCI), and numeral 3 represents Alzheimer's disease patients (AD).Alzheimer's disease patients (AD).
Train_Train_sitesitess:
In this matrix, different numberdifferent numberss represent different represent different sitessites that subjects belong to.that subjects belong to.
Train_Train_popupopulationlation::
Here provided age and gender information for each subject. The 1st column is gender in which 0 provide age and gender information for each subject. The 1st column is gender in which 0 representrepresentss malemale and 1 representand 1 representss femalefemale. The 2nd column ishe 2nd column is age.age.
Train_setTrain_set::
This cell providess all data processed by AFQ. all data processed by AFQ. Each row is a fiber tractEach row is a fiber tract whosewhose name can be found in name can be found in a a variable called “fgnames” variable called “fgnames” (matched order). (matched order). EEach column is a tract property.ach column is a tract property. We already put all We already put all subjects from different sites together.subjects from different sites together.

Refrence:
GitHub. 2020. YongLiuLab/AI4AD_AFQ. [online] Available at: <https://github.com/YongLiuLab/AI4AD_AFQ> 


