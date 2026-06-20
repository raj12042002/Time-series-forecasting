# Time-series-forecasting
X = [] y = []  for i in range(3,len(sales_scaled)):     X.append(         sales_scaled[i-3:i,0]     )     y.append(         sales_scaled[i,0]     )  X = np.array(X) y = np.array(y)  X = X.reshape(     X.shape[0],     X.shape[1],     1 )
