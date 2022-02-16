# lab2
choco <- read.csv("https://ds202-at-isu.github.io/labs/data/choco.csv")

choco$Review.Date = as.factor(choco$Review.Date)

ggplot(data = choco, aes(x=Review.Date)) + 
  geom_bar(aes(weight=Rating))
