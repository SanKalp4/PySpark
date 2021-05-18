# PySpark

```N.B.```  https://nbviewer.jupyter.org/ paste github project link to showcase the notebook if github fails to load the same.

Sudden cardiac death (SCD) is a major global health problem, accounting for up to 20% of deaths in Western societies including India. Work life stress, lifestyle, hypertension, health ignorance is causing cardiac arrest even in age group lower than 20 years. Cardiac arrest is responsible for half of the cardiac disease related death.

This project revolves around devicing ml techniques using Pyspark to predict the probability of having a cardiac arrest by taking certain attributes in consideration.

The objective is to predict whether a person will have cardiac arrest or not based on certain attributes like demographics, health conditions etc.

- Features/Attributes

```ID-Patient ID```

```Gender```

```Age```

```Hypertension```

```Heart disease```

```Job type```

```Residence type```

```Blood sugar level```

```Body mass index```

```Smoking status```

-Target  

```Cardiac arrest```  ‘Yes’-```0``` ‘No’-```1```

N.B. Used Synthetic Minorty OverSampling Technique to achieve a higher AUC but best practice is to undersample the majority class and then use with SMOTE. SMOTE does not consider the effect of majority class which is a disadvantage which may give promising model but not perform that greatly with realworld test data. 
Without SMOTE , LR is pulling up an AUC score of 0.83.
