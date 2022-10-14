# Contain R script
Hi i will share some simple calculations and graphs in R,with the following dataset.oh yeah, it doesn't use any package to run the plot,so you can immediately run the program.
# Datasets
kota <- c(7.7, 7.86, 9.06, 10.58, 9.07, 10.13, 9.41, 8.6, 8.98)

# Plot
There are various kinds of plots here, this is only for one variable

 - Bar Plot
barplot(nama_variabel, main="Judul plot", horiz=FALSE,
  names.arg=c("variabel x","etc . . ."))
  
 - Pie Plot
 label <- c("variabel x","etc . . .")
pie(nama_variabel, labels = label, main="Judul plot")

 - Stem and Leaf Plot
 stem(nama_variabel)

 - Line Plot
 plot(nama_variabel, type = "o")


# Mean,Median,Mode,Varian,Data varians

 - Mean
    hasil <- mean(nama_variabel_data)
    print(hasil)
    
 - Median
	hasil <- median(nama_variabel_data)
    print(hasil)
   
 - Mode
	mode = function() {
     return(names(sort(-table(nama_variabel_data)))[1])
    }
     mode()
     
 - Varians
 hasil <- var(nama_variabel_data)
print(hasil)

 - Data Varians
 hasil <- sqrt(var(nama_variabel))  
print(hasil)

 
