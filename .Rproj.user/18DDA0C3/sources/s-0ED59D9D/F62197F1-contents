## Put comments here that give an overall description of what your
## functions do

## This function is used to set and retrieve a matrix as well as its inverse.

makeCacheMatrix <- function(x = matrix()) {
  inv <- NULL
  set <- funtion(y){
    x<<- y
    inv <<- NULL
  }
  get <- function() {x}
  setInverse <- function(inverse){inv<<- inverse}
  getInverse <- function(){inv}
  list(set=set,get=get,setInverse=setInverse,getInverse=getInverse)

}


## This function is used to calculate the inverse of a matrix

cacheSolve <- function(x, ...) {
        ## Return a matrix that is the inverse of 'x'
  inv<- x$getInverse()
  if(!is.null(inv)){
    message("getting cached data")
    return(inv)
  }
  p<- x$get()
  inv <- solve(p,...)
  x$setInverse(inv)
  
}
