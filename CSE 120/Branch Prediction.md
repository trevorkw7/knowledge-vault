

Q1:

Assume a branch outcome of

  

T T N N T T N N T T N N …

  

T = taken, N = not-taken



  

What is the prediction accuracy of a 1-bit history-based branch prediction scheme where the initial prediction state is not taken (N)?



  

Hint: List branch outcomes, states and predictions the same way as learned in the lecture.

State Time: Prediction: Outcome:
N N T
T T T
T T N
N N N
N N T
T T T
T T N
N N N
N N T
T T T
T T N
N N N


50%
  
  

Q2:

A snapshot of the taken/not-taken behavior of a branch is:

  

T T N N T T N N T T N N T T N N...

  

Determine the steady state prediction accuracy of a 2-bit, saturating counter prediction scheme where the initial prediction state is strongly not taken (N). 

(N,n,t,T)

State Time: Prediction: Outcome: (right/wrong)
N N T w
n N T w
t T N w 
n N N r
N N T w
n N T w 
t T N w 
n N N r
N N T w 
n N T w
t T N w 
n N N r
N N T w
n N T w
t T N w
n N N r


4/16 = 25% prediction accuracy



  

Q3:

Given the branch and assumptions in Q2, what is the steady state prediction accuracy if the initial prediction state is strongly taken (T)?

  
**
T T N N T T N N T T N N T T N N...
(N,n,t,T)
State Time: Prediction: Outcome: (right/wrong)
T T T r
T T T r
T T N w
t T N w 
n N T w
t T T r
T T N w
t T N w
n N T w 
t T T r
T T N w
t T N w 
n N T w
t T T r
T T N w 
t T N w


5 / 16 = 31 %, will converge to 25%

