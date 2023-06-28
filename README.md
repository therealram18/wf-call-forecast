# Wells Fargo Hackathon: Call Forecast
Solution presented in the Shaastra 2023 Wells Fargo Hackathon, for the ML Problem Statement. 

This involved predicting the values for a period of three months following a period of three years during which information about the number of calls on a daily basis was available. 

Calls were split into three categories: calls from holders of the commercial cards, retail cards and student cards. On a graph, the numbers look like this (for the data on the commercial card calls):

![download](https://github.com/therealram18/wf-call-forecast/assets/96683090/2c53bf88-33dd-40ac-969c-d1f9ce78de6e)

The data was analyzed as a function of the day, and a parameter was included to encode the same. The [statsmodels](https://www.statsmodels.org/stable/index.html) library was also utilized to observe any trends.

The model architecture used was the Long Short Term Memory, [here is a nice explanation of how this works](https://colah.github.io/posts/2015-08-Understanding-LSTMs/).

Two implementations are presented, one using PyTorch, and the other using Keras. The best accuracy (which was found in the case of Keras) is **81%**. The obtained results file is also attached. 
