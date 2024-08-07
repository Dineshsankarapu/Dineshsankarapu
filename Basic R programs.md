7. Write a R Program to Plot Shaded Area between vertical lines
x <- seq(0, 10, length.out = 100)
y <- sin(x)
plot(x, y, type = "l")
polygon(c(3, 5, 5, 3), c(-1, -1, 1, 1), col = "lightblue", border = NA)
Csv

Sure, I can help you with that! Here are the R programs for the tasks you mentioned:

1. Read the content of a CSV file and show as a data frame:
```R
data <- read.csv("your_file.csv")
print(data)
```

2. Export a CSV file without row names:
```R
data <- data.frame(x = c(1, 2, 3), y = c("a", "b", "c"))
write.csv(data, file = "your_file.csv", row.names = FALSE)
```

3. Write to a CSV file without index:
```R
data <- data.frame(x = c(1, 2, 3), y = c("a", "b", "c"))
write.csv(data, file = "your_file.csv", row.names = FALSE)
```

4. Append a row to a CSV file:
```R
data <- data.frame(x = c(4), y = c("d"))
write.table(data, file = "your_file.csv", append = TRUE, sep = ",", col.names = FALSE)
```

5. Calculate mean, median, and variance of a CSV file:
```R
data <- read.csv("your_file.csv")
mean_value <- mean(data$column_name)
median_value <- median(data$column_name)
variance_value <- var(data$column_name)
```

6. Display the structure of a CSV file:
```R
data <- read.csv("your_file.csv")
str(data)
```

7. Convert a text file into a CSV file:
```R
data <- read.table("your_file.txt", sep = ",")
write.csv(data, file = "your_file.csv", row.names = FALSE)
```

Let me know if you need any further assistance with these programs!

