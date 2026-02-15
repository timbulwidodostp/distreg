# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Distribution regression as in Foresi and Peracchi (1995) Use distreg With (In) R Software
install.packages("remotes")
remotes::install_github("zengying17/ate_pct-r")
install.packages("sandwich")
library("sandwich")
library("atepct")
# Estimate Distribution regression as in Foresi and Peracchi (1995) Use distreg With (In) R Software
distreg = read.csv("https://raw.githubusercontent.com/timbulwidodostp/distreg/main/distreg/distreg.csv", sep = ";")
y0 <- median(distreg$lcfincome)
distreg <- distreg(lcfincome ~ lfincome + HEDUC, distreg, y0)
distreg
# Distribution regression as in Foresi and Peracchi (1995) Use distreg With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
