# Maschinendynamik
Projects


# Stabbkräfte

 ```python
philist = sol.y[0]
phidotlist =  sol.y[1]
 
stabkrafte = [m*l*(i**2) + m*g*math.cos(j)   for i, j in zip(phidotlist, philist)] #Stabkraft = Sdyn + Ssta

fig, ax = plt.subplots()
plt.grid()
plt.rcParams["figure.figsize"] = (5,3)
ax.plot(t, stabkrafte)
ax.set_title("Stabkräfte")
ax.set_xlabel("t (s)")
ax.set_ylabel("S (Newton)")

 ```
 ![indir](https://user-images.githubusercontent.com/54573938/212378170-dfaf5a65-2209-47d3-863d-a3c87c08d4d5.png)
