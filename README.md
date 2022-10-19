# Welcome to GitHub Desktop!





## uloha 1 

combin <- function(n,k)
{
  combin <- c(1)
  for (i in 1:k)
    combin <- combin * (n-i+1)/i
  return(combin)
  
}

combin(6,2)
combin(9,4)

## uloha 2

odhad <- function(x)
{
  an <- c(1)
  min <- 1e-10
  repeat
  {
    an <- 0.5*(an+(x/an))
    if(abs(an*an-x)<min)
      break
  }
  return(an)
}

odhad(2)
odhad(4)
odhad(7)

## uloha 3

integ <- function(f,a,b)
{
  lower_bound = a 
  upper_bound = b
  f <-  function(x) {x}
  integral = integrate(f, lower_bound, upper_bound)
  return(integral)
    
}

integ(x,3,7)
integ(x,1,6)

## uloha 4


library(stringr)
clear.dia <- function(s)
{
  stri_trans_general(s,"LATIN-ASCII")
}
clear.dia("čučoriedka")
clear.dia("mačička")
clear.dia("žirafa")