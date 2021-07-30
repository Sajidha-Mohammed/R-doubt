# R-doubt
``` r
 ggplot(s, aes(x = factor(Disease.diagnosis))) +  
      geom_bar(aes(y = (..count..)/sum(..count..))) + 
      scale_y_continuous(labels = percent)+
      geom_text(aes(y = ((..count..)/sum(..count..)), label = scales::percent((..count..)/sum(..count..))), stat = "count", vjust = 0.5,hjust=0) +
     coord_flip() 
```
