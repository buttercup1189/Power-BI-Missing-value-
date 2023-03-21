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
 Upper =  75 percentile + (1.5* IQR)+
