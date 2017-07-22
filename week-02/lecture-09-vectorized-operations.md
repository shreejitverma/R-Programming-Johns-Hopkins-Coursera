Vectorized Operations
=====================

Many operations in R are vectorized kaing the code more efficient, concise, and easier to read.

	> x <- 1:4; y <- 6:9
	> x + y
	[1]  7  9 11 13
	> x > 2
	[1] FALSE FALSE  TRUE  TRUE
	> x >= 2
	[1] FALSE  TRUE  TRUE  TRUE
	> y == 8
	[1] FALSE FALSE  TRUE FALSE
	> x * y
	[1]  6 14 24 36
	> x / y
	[1] 0.1666667 0.2857143 0.3750000 0.4444444

In other languages you might have to run a loop to add two vectors together. But in R x + y acts as you'd expect and sums the two vectors.

	> x <- matrix(1:4, 2, 2); y <= matrix(rep(10, 4), 2, 2)
	> x * y		## element-wise multiplication
	     [,1] [,2]
	[1,]   10   30
	[2,]   20   40
	> x / y
	     [,1] [,2]
	[1,]  0.1  0.3
	[2,]  0.2  0.4
	> x %*% y 		## true matrix multiplication
	     [,1] [,2]
	[1,]   40   40
	[2,]   60   60

