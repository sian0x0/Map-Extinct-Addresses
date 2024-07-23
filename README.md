# Mapping extinct streets of Belfast
There are some small streets in 19th century Belfast that were never mapped before they were demolished. 

![482px-Map_of_the_Town_and_Environs_of_Belfast_%281791%29.png](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b3/391_of_%27%28The_Imperial_Gazetteer%3B_a_general_dictionary_of_geography%2C_physical%2C_political%2C_statistical_and_descriptive_..._Edited_by_W._G._Blackie_..._With_..._illustrations%2C_etc.%29%27_%2811252279605%29.jpg/430px-thumbnail.jpg)

They do appear in [street directories](https://www.lennonwylie.co.uk/). Is it possible to recreate a map based on street directories?

## Street directories
The great thing about (some) street directories is that they list every address and intersection in order. In this way, they preserve a large amount of data about the topolocical relations between these features. 

![Millfield-Belfast-Street-Directory-1850](https://github.com/user-attachments/assets/9cad2030-ed8d-448f-934e-947b5a1f527b)

## Networks
It should therefore be possible to map them out as a network, even if the position of each node (address or intersection) is not known. 

![Vancouver_Transit_Network_Map](https://github.com/user-attachments/assets/0b481e25-364f-4349-b0f8-3ff1a833d77e)

## Geocoding
Some features still exist today, and can be geocoded to give their coordinates to "anchor" the network at various points in space, like pinning strings of beads to a board.

## Layout algorithms
Assuming that each address has a similar length of frontage can give more clues than just using the intersections alone. Layout algrithms should be able to place the addresses with no known positions in a street-like fashion (try to to make the strings straight-ish, try not to cross them oover where there is no intersection, etc.)

## Mapping
It should be relatively easy to convert strings like this into LineStrings and other relations used in GIS/mapping systems, which can be overlaid onto modern or old georefernced maps.
