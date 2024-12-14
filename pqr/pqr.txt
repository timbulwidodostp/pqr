# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Penalized Quantile regression with fixed effects Use pqr (pqrfe) With (In) R Software
install.packages("pqrfe")
library("pqrfe")
pqr = read.csv("https://raw.githubusercontent.com/timbulwidodostp/pqr/main/pqr/pqr.csv",sep = ";")
# Estimation Penalized Quantile regression with fixed effects Use pqr (pqrfe) With (In) R Software
x = cbind(pqr$X1, pqr$X2, pqr$X3, pqr$X4)
y = cbind(pqr$y)
subj = cbind(pqr$subj)
pqr = pqr(x=x, y=y, subj=subj, tau=0.75, effect="lasso", c = 0)
pqr
# Penalized Quantile regression with fixed effects Use pqr (pqrfe) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished