Q1

#Project title: a reproducible study on logistic growth

#Project contents:

Main files used in the study: experiment.csv, fit_linear_model.R, plot_data.R, plot_data_and_model.R

The csv file I used is "experiment.csv".

In the "plot_data.R" file, I plot the relationship between t (time) and N (population size) in a scatter plot.

In the "fit_linear_model.R" file, I made two linear models under two different conditions:
1) when t is small and K (carrying capacity) is much bigger than the population size
2) when t is large enough so that the population size reaches the carrying capacity

In the "plot_data_and_model.R" file, I fit my data in the logistic model `N = (N0*K*exp(r*t))/(K-N0+N0*exp(r*t))` and make a scatter plot between N and t.

Results: my data fit quite well in the logistic growth, where I set N0 (initial population)=879, r=0.01, K=60000000000 (6*10^10)
N0 and K are found in the file "experiment.csv". r (population growth rate) is the slope in my linear model 1 when t is small. At the beginning when population size is much smaller than carrying capacity, the relationship between N and t is almost linear, and the slope is about the population growth rate.

Q2

The function of exponential growth `N(t) = N0exp(r*t) where N0=879, r=0.01, and t=4980 min, so N(4980)=3.73*10^24`

Under logistic growth `N = (N0*K*exp(r*t))/(K-N0+N0*exp(r*t))` where `K=6*10^10, N(4980)=6*10^10`

`6*10^10 is much smaller than 3.73*10^24`, and this is because the population already reaches the carrying capacity (K) when t=4980

Q3



