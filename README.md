import matplotlib.pyplot as plt

# Data for sales distribution
labels = ['Product A', 'Product B', 'Product C', 'Product D']
sizes = [35, 25, 25, 15]
colors = ['gold', 'lightblue', 'lightgreen', 'violet']
explode = (0.1, 0, 0, 0)  # Emphasize the first slice

# Create pie chart
plt.figure(figsize=(6, 6))
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%',
        shadow=True, startangle=140)
plt.title("Sales Distribution by Product Category")
plt.axis('equal')  # Ensures the pie chart is circular
plt.savefig('sales_distribution.png')  # Save the image to include in your GitHub repo
plt.show()
