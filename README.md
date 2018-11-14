Write a program to create barplots for all the categorical columns in mtcars.
library(ggplot2)
library(dplyr)
library(cowplot)
plot1 <- ggplot(mtcars, aes(mpg)) +geom_bar()
plot2 <-  ggplot(mtcars, aes(cyl)) +geom_bar()
plot3 <- ggplot(mtcars, aes(disp)) +geom_bar()
plot4 <- ggplot(mtcars, aes(hp)) +geom_bar()
plot5 <- ggplot(mtcars, aes(drat)) +geom_bar() 
plot6 <- ggplot(mtcars, aes(wt)) +geom_bar() 
plot7 <- ggplot(mtcars, aes(qsec)) +geom_bar() 
plot8 <- ggplot(mtcars, aes(vs)) +geom_bar() 
plot9 <- ggplot(mtcars, aes(am)) +geom_bar() 
plot10 <- ggplot(mtcars, aes(gear)) +geom_bar() 
plot11 <- ggplot(mtcars, aes(carb)) +geom_bar() 
cowplot::plot_grid(plot1, plot2, plot3, plot4, plot5, plot6, plot7, plot8, plot9, plot10, plot11)



2. Create a scatterplot matrix by gear types in mtcars dataset.

library(car)
scatterplotMatrix(~mpg+cyl+disp+hp+drat+wt+qsec+vs+am+carb|gear, data = mtcars, main = "Gear type")


3. Write a program to create a plot density by class variable.

