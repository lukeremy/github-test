SkillZone <- c("Alex", "Elba", "Heggy", "Bayar", "Diogo", "Piyush", "Victor", "Mary", "Luke")
analyst <- SkillZone[1:3]
fieldtech <- SkillZone[4:6]



teacher <- function(student){
     
     if (student %in% analyst){
          teacher <- "G5"
          paste0(student, "'s teacher is ", teacher)
     }
     
     else if (student %in% fieldtech){
          teacher <- "Dennis"
          paste0(student, "'s teacher is ", teacher)
     }

     else{
          paste0(student, " is not a SkillZone student")
     }
}

teacher("Alex")
teacher("Bayar")
teacher("Mary")