# Plots-R

#bar plot
ggplot (diamonds, aes (x= cut, fill= type )) + geom_bar() + theme_light() +
scale_fill_manual(values =pal_igv() (15))

#Scattered Plot
ggplot ( diamonds, aes(x= carat, y= price , colour = cut)) + geom_point()+
  theme_bw()+
  xlab("cut") +
  ylab("price") +
  ggtitle("The title")+
  facet_grid(~cut)

#Box plot
ggplot (mpg, aes(x= drv, y= hwy ,fill = trans)) + geom_boxplot() +
            theme_light()

#Violin Plot
 ggplot (mpg, aes(x= drv, y= hwy )) + geom_violin(fill= "red", color = "blue")+
    geom_boxplot(width = 0.2)+ 
    theme_light()+
    coord_flip()
  xlab("cut") +
  ylab("price") +
  ggtitle("The title")+
