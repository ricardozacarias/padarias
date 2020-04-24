# Padarias

This is gonna be the post.

["A Padaria Portuguesa"](https://www.apadariaportuguesa.pt/) 

Abrimos a 5 de Novembro de 2010, a primeira “Padaria Portuguesa”, na Av. João XXI, em Lisboa.

As of April 2020 they have 62 locations in the greater Lisbon area. These days it's kind of hard to walk around the city without stumbling into one of these places.

This made me wonder: what is the actual reach of this business in terms of percentage of area covered?

To answer this question the first thing we need are the coordainates of every single location. Luckily for us, Zomato has a free [API](https://developers.zomato.com/api) which has some limits, but very rich and easy to use. 

Once you get a developer key, you can query the code of your in Zomato's website and then use the /Search API to grab all the restaurants that match your query (note: you can only get 20 restaurants at a time, up to 100 max). This is not really the scope of the article but you can find the code [here](github.com).

Alright so now we have the latitude and longitude coordinates for each store, let's look at them. This is where one of my favorite libraries comes is: Geopandas.

Geopandas adds support for geographic data to [pandas](http://pandas.pydata.org/) objects. SImply, it adds a 'geometry' column to a DataFrame and uses Shapely and fiona

Shapely is a BSD-licensed Python package for manipulation and analysis of planar geometric objects.

Now we need a frame of reference. To answer owr question

With this library we can



