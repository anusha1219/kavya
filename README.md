https://m.rbi.org.in/scripts/bs_viewcontent.aspx?Id=3526

https://learning.oreilly.com/live-training/courses/hands-on-machine-learning-with-python-classification-and-regression/0636920276951/


Retail Banking
Investment Banking
Risk and Compliance
Surveillance
Corporate Banking
Wealth Management
Exchanges/Trading/Broker-Dealer
Clearing/CCP



import matplotlib.pyplot as plt
import math
import numpy as np

# set the minimum potential
rm = math.pow(2, 1 / 6)
t = np.linspace(-10, 10, 1000, endpoint = False)
x = []
y = []

for i in t: 
    x_i = np.sin( 3 * t[i] )
    y_i = np.sin( 4 * t[i] )
    x.append(x_i)
    y.append(y_i)

# plot the graph
plt.plot(x,y)

# set the title
plt.title('Plot sin(4t) Vs sin(3t)')

# set the labels of the graph
plt.xlabel('sin(3t)')
plt.ylabel('sin(4t)')

# display the graph
plt.show()
