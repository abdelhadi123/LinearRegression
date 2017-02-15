import matplotlib.pyplot as plt
import numpy as np

def sq(f):                      # def of square function
    return f*f

#########################################################

X=[0,1,2,3,4,5,6,7,8]                            #Our DATA
Y=[1,10,7,13,23,15,29,36,45]

##### calculating the sum of X*Y ######
i=0
a=0

while i<=X[-1]:
    a=a+(X[i]*Y[i])
    i=i+1
    
sum_product=a

#####################################

N=len(X)                              # number of point
sum_x = sum(X)                        # the sum of X's
sum_y = sum(Y)                        # the sum of Y's

########## calculating the sum of X^2 ###############

t=0
j=0
for j in X:
    t=t+sq(X[j])
    j = j+1

############### numerator and denominator of the slope #######################

numerator = (sum_product/N)-(sum_x/N)*(sum_y/N)

denominator = (t/N)-((sum_x/N)*(sum_x/N))

slope = numerator/denominator

intercept = (sum_y/N) - slope * (sum_x/N)

def linear(formula, x_range):  # ploting the linear function y=slope*x+intercept
    x = np.array(x_range)  
    y = eval(formula)
    plt.plot(x, y,'r--')  


linear('slope*x+intercept',range(0,len(X)))

plt.plot(X,Y,'bo')                       
plt.show()

