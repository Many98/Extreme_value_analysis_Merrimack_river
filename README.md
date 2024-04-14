# Analysis of maximal annual flows of Merrimack river (in slovak)

## Introduction

In this protocol, we attempt to quantify the probabilities of possible anomalous events for the year 2022 using the Merrimack River maximum annual flow data analysis.

### Highlights
![box](https://github.com/Many98/Extreme_value_analysis_Merrimack_river/assets/65658910/9b08bb1c-7913-4d69-9c0b-43aba1b29bff)
![peakplot](https://github.com/Many98/Extreme_value_analysis_Merrimack_river/assets/65658910/08fc15ba-4e47-43ac-b5c4-bc912d30bc57)

![histo](https://github.com/Many98/Extreme_value_analysis_Merrimack_river/assets/65658910/e8352307-ef8f-4378-bd3a-57232f32aae1)
![kde](https://github.com/Many98/Extreme_value_analysis_Merrimack_river/assets/65658910/3efdba77-13b0-41b9-926b-a2afc825eaee)
![qq](https://github.com/Many98/Extreme_value_analysis_Merrimack_river/assets/65658910/be3a0d93-0583-4f7d-ac46-5a593ff670ea)
![me_plot](https://github.com/Many98/Extreme_value_analysis_Merrimack_river/assets/65658910/cf31c54e-1588-43d4-8792-33f28018d3d3)

![pot](https://github.com/Many98/Extreme_value_analysis_Merrimack_river/assets/65658910/ad299388-c3c9-44ce-8d51-86eb6f3f4142)
![pot2](https://github.com/Many98/Extreme_value_analysis_Merrimack_river/assets/65658910/b36ed1ef-a807-4d68-aa16-836bf5e4544c)


### Conclusions

In this protocol, we analyzed the flows of the Marrimack River and tried to quantify the values of the probabilities defined in the introduction. We performed the analysis using the so-called block maximum access or using annual maxima. We then tried to analyze task 7 using the peak over threshold approach. This POT approach turned out to be significantly dependent on the threshold value and we also considered the values of and based on the observations obtained by the block maxima approach. The POT model is an interesting alternative or additional approach to the BM method, but as we found out, it requires significantly more tuning and we could not do this due to time constraints.

In the case of the BM approach, we first tried estimations using the Markova and Chebyshev-Canteli inequalities. As we expected, these brought very rough estimates. As non-parametric estimators, we tried histograms with multiple bin widths, including bins of different widths. We also tried nuclear density estimates. I consider the histogram using the Diaconis method for choosing the width of bins and the kernel estimate using the epanachnik kernel to be the most suitable non-parametric estimates. We reached this conclusion based on further analysis using parametric models and by eye the best fit with the given parametric models. After analyzing the QQ-plots, we selected the GPD, GEV, Gumbel and Fisk distributions for parametric modeling, as they fit our data best. As it turned out, according to the AIC criterion as well as according to the already analyzed QQ-plots, the GEV, Gumbel and Fisk distributions were the most suitable and yielded very similar probability estimates. It was also shown that after fitting the GEV model, the value of the shape parameter was close to zero, and thus the GEV and the Gumbel distribution were almost the same. It is also known that the BM model should asymptotically lead to the GEV distribution and that is why I would choose the Gumbel or GEV distribution as the most suitable model.

