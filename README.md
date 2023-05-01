# Dual Axis Chart

# What is dual axis chart in tableau

Dual-axis charts are particularly useful for analyzing two measures that have different scales.

In the case of measures with the same scale, they can share the same axis using the blend method. 

Blending measures in Tableau will consist of dragging one measure or axis and dropping it onto an existing axis.

•In the data source Amazingmart we have 3 sheets which includes:-

# Listoforders

# OrderBreakdown

# SalesTarget

First we have to use Data blending.

By using Data blending we are joining the first two which is (listoforders) and (orderbreakdown)

and in another only this will be used alone(salesoftarget)

# Disclaimer:- 

we are using data blending and not inner join because we will have to aggregate our dataset 

and by aggregating the dataset in this particular data we will loose some main data.

Another reason for using Data blending is when the data source is different we can't use join function.

# let's start

• Now first we have to put months(Orderdate) in columns to see how the graph shows in respect to this.

next we will add SUM(sales) and Category to see different types of category with graph 

which include Furniture,Office Supplies,Technology

• Now from Salestarget sheet we have to drag drop SUM(target) to know how much target 

of products is in every year.

Now using mapping,the target will be in proper format for using in visualization.


# creating dual axis in graph

right click on target and go to dual axis and it will automatically overlap the graph

on bar chart to get aesthetic view.Also right click and use synchronise axis to not over burden in the  graph.

•We have created a calculated field by using 

sales-SUM[(salesoftarget (amazingmart)].[Target]

To get detailing drag drop category to detail to get more better view of it.

•Now using slicing filters we can see with different products how the targets and sales gets changed.
![Screenshot (27)](https://user-images.githubusercontent.com/125815238/235460623-35b1ce3c-944e-4583-89a5-a12c32f1fd56.png)

![Screenshot (28)](https://user-images.githubusercontent.com/125815238/235460735-431a5cc1-9645-496a-93c7-959f4c534d04.png)

![Screenshot (29)](https://user-images.githubusercontent.com/125815238/235460805-1d054d28-e403-478b-a2ba-8c08ae3381eb.png)


