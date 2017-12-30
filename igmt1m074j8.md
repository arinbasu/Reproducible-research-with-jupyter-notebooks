Table 1. The results of the summary analyses    
    
    | Continent|  mean_afr| mean_alr| mean_gnipercap| mean_psenrol_f|  mean_pbp|
    |---------|---------|--------|--------------|--------------|---------:|
    |         1|  37.30000| 76.90000|      14893.529|       85.78947|  2.366667|
    |         2|  20.50000| 97.91154|      19777.083|       92.91111|  2.590909|
    |         3| 111.64444| 61.69048|       3050.435|       67.57447| 35.837500|
    |         4|  49.60000| 91.60000|      24524.000|       95.00000|  3.000000|
    |         5|  77.88889| 87.94091|       7397.143|       89.13793| 14.044444|
    |         6|  39.26087| 87.60714|      12167.200|       89.04000| 12.420000|
    |         7|  57.33333| 69.81250|       2865.556|       85.44444| 28.314286|



```R
## The summarised data can be graphically explored using ggplot
# We plot the mean adult literacy rate by continent
# We can store this figure using a png file format

png("alr_cont.png")
ggplot(sum_mydata) +
 geom_bar(aes(x = Continent, y = mean_alr), stat = "identity") +
 ggtitle("Mean Adult Literacy Rate by Continent") +
 ylab("Mean adult literacy rate (%)") +
 xlab("Continent")
dev.off() 
```
