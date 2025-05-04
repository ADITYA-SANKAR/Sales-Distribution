# Sample data for sales distribution across products
labels = ['Product A', 'Product B', 'Product C', 'Product D']
sizes = [35, 25, 25, 15]
colors = ['gold', 'lightblue', 'lightgreen', 'violet']
explode = (0.1, 0, 0, 0)  # only "explode" the 1st slice

plt.figure(figsize=(6, 6))
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%',
        shadow=True, startangle=140)
plt.title("Sales Distribution by Product")
plt.axis('equal')  # Equal aspect ratio ensures that pie is drawn as a circle.
plt.show()
