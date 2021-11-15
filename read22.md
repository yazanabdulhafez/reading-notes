# RecyclerView

## Create dynamic lists with RecyclerView

RecycleView make it easier to handle displying a large set of data as a list. When an item scrolls off the screen, RecyclerView doesn't destroy its view. Instead, RecyclerView reuses the view for new items that have scrolled onscreen.

![ResycleView](https://miro.medium.com/max/200/1*Bu_PjgiOEM9CVgJVz3XiNQ.gif)

### Key classes

Several different classes work together to build your dynamic list:

* RecyclerView is the ViewGroup that contains the views corresponding to your data.
* Each individual element in the list is defined by a view holder object.which extended from the RecyclerView.
* Adapter binds the views to their data, we define the adapter by extending RecyclerView.Adapter.
* The layout manager arranges the individual elements in your list.

### Steps for implementing your RecyclerView

1. First of all, decide what the list or grid is going to look like.
2. Design how each element in the list is going to look and behave.
3. Define the Adapter.

### Plan The layout

The items in your RecyclerView are arranged by a LayoutManager class. The RecyclerView library provides three layout managers, which handle the most common layout situations:

* `LinearLayoutManager` arranges the items in a one-dimensional list.
* `GridLayoutManager` arranges all items in a two-dimensional grid.
* `StaggeredGridLayoutManager` is similar to GridLayoutManager, but it does not require that items in a row have the same height (for vertical grids) or items in the same column have the same width (for horizontal grids). The result is that the items in a row or column can end up offset from each other.

### Implementing your adapter and view holder

* Adapter and view holder are two classes work with each other The ViewHolder is a wrapper around a View that contains the layout for an individual item in the list. The Adapter creates ViewHolder objects when its needed also sets the data for those views.

* The process of associating views to their data is called binding.

* When you define your adapter, you need to override three key methods:

1. <span style="color: blue;">onCreateViewHolder()</span>: This method creates and initializes the ViewHolder and its associated View, but does not fill in the view's contents—the ViewHolder has not yet been bound to specific data.

2. <span style="color: blue;">onBindViewHolder()</span>:This method is called by RecyclerView  to associate a ViewHolder with data. The method fetches the appropriate data and uses the data to fill in the view holder's layout.

3. <span style="color: blue;">getItemCount()</span>:this method called by RecyclerView   to get the size of the data set.

## Resources used in this reading

1. [Create dynamic lists with RecyclerView](https://developer.android.com/guide/topics/ui/layout/recyclerview#key-classes)
