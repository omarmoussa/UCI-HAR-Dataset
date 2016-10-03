str(dtTidy)

key(dtTidy)

dtTidy

summary(dtTidy)

dtTidy[, .N, by=c(names(dtTidy)[grep("^feat", names(dtTidy))])]

f <- file.path(path, "DatasetHumanActivityRecognitionUsingSmartphones.txt")
write.table(dtTidy, f, quote=FALSE, sep="\t", row.names=FALSE)
