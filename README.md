# binomial-pricing-model
Design a binomial pricing model to calculate option values
- Apply the Law of One Price to construct two portfolio, one holding stock and cash in a bank account receiving risk-free rate
- From portfolios relationship at time T derive the risk-neutral probability and apply it to derive the present value of the European call option
- Explain why the relationship of 0<d(down factor)<(1+r)(risk-free rate)<u(up factor) should be held
- Visualize the binomial pricing tree with a node network, i represents the time steps and j represents the ordered price outcomes. Perform zig-zag move by timing with factor (u/d) to iterate all possible outcomes in one time step
- Perform recurssion to derive outcomes at previosu time step after having all the outcomes at further time step, until getting the present value of the option
- use numpy array to store the values at each column to conduct array operation rather than generating single value by for-loop function (it is conducting a single period pricing many times, however we can do it all at once). Array multiplication is much faster when complexity or N is large
