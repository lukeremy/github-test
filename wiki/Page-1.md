threesus <- function(ft_per, attempts){

     if(ft_per < 0 | ft_per > 100) stop ("Please enter a valid number for free throw percentage")
     if(0 < ft_per & ft_per < 1) warning("Are you sure you entered a percent for free throws?")
     if(!(is.numeric(attempts))) stop("Please enter a valid number for attempts")
     
     ft_per <- as.numeric(ft_per)/100
     
     prob <- round((ft_per^attempts)*100,1)
     
     paste("Steph has a", prob, "% chance of making",
         attempts, "free throw attempts in a row.")
     # prob
}

threesus(94,"ten")
threesus(101,10)
threesus(.94,10)
threesus(94,10)
threesus(90,10)
threesus(99,10)