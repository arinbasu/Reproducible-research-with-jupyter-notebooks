
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
