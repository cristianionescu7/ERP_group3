# ERP_group3
Two different instances of the dbc experiment, per subject predictions not possible. Per item instead
90 sentences
For each sentence there are 3 conditions (baseline, event related, event urelated)
We average the reading time per sentence-condition
For each electrode we get the N400 and P600 components per sentence-condition
We predict reading time from N400 and P600 per condition
The linear regression revealed that for each condition there are certain electrode that perform better. We take the best 3 electrodes for each condition and use them in multiple linear regression
for control: 'T8', 'PO9', 'P7'
for script-related: 'O1', 'Oz', 'Pz'
for script-unrelated: 'PO9', 'T7', 'O1'
Then we build RNN and train it on all electrodes
For both regressions and RNN we measure accuracy with R-squared, mean absolute error, mean squared error, loss


!TO DO!:
Get the RNN to be as accurate as possible
Run the linear regression the other way as well (RT as input, N400/P600 as output)
