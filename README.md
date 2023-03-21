# Power-BI-Missing-value- 
First >>
Media, Min, Max, Average of count(district) of total id



Second> Imputation - Dax 
New Measure
= IF PRICE IS BLANK, ADD "110" AS AVERAGE VALUE 
= IF(ISBLANK(airbnb[price]),110,airbnb[price])
![image](https://user-images.githubusercontent.com/65704118/226706581-1bc068d0-1d34-4a32-b310-5cdb9d058652.png)

# Outliers
//Finding outliers  using standard deviation
 lower =-3 * SD
 upper = 3 * SD 
 outlier 
 Value <lower or upper> Value
 
 //Finding outliers : Interquartile Range (IQR)
 lower = 25 percentile - (1.5* IQR) 
 Upper =  75 percentile + (1.5* IQR)
 
 // Addressing outliers
 1) Removing observation
 2) Imputation
 >> Winsorzing 
 Winsorizing or winsorization is the transformation of statistics by limiting extreme values in the statistical data to reduce the effect of possibly spurious outliers. It is named after the engineer-turned-biostatistician Charles P. Winsor (1895–1951).

 
 ![image](https://user-images.githubusercontent.com/65704118/226718998-7bb5c842-1400-4e6c-aba0-49e54eb207ac.png)
 ![image](https://user-images.githubusercontent.com/65704118/226719611-31caff9c-8fe2-40ed-b083-7868437db09c.png)


