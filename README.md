# stat632

student-mat.csv: contains math class data

student-por.csv: contains portugese language class data

student-merge.R: #contains the following R code for combining data:
d1=read.table("student-mat.csv",sep=";",header=TRUE)
d2=read.table("student-por.csv",sep=";",header=TRUE)

d3=merge(d1,d2,by=c("school","sex","age","address","famsize","Pstatus","Medu","Fedu","Mjob","Fjob","reason","nursery","internet"))
print(nrow(d3)) # 382 students


---------------------
In R, executed command `write.csv(d3,"student.csv)` to create the following:

student.csv
contains combined dataset

student.txt : contains list of variables and descriptions




Citation:

P. Cortez and A. Silva. Using Data Mining to Predict Secondary School Student Performance. 
In A. Brito and J. Teixeira Eds., Proceedings of 5th FUture BUsiness TEChnology Conference (FUBUTEC 2008) 
pp. 5-12, Porto, Portugal, April, 2008, EUROSIS, ISBN 978-9077381-39-7. 
[Web Link] http://www3.dsi.uminho.pt/pcortez/student.pdf
