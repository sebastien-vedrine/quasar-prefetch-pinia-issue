I would like to store prefetched data in a Pinia store.

I made a simple example to demonstrate the issue I encounter.

In this example I have 3 routes :
- Route1 uses the IndexPage component
- Route2 and Route3 both use the IndexPage2 component

When I refresh any of the 3 routes independently, I can retrieve the data from the store and dispaly it in the template.

However, when I go from Route2 to Route3, the data can not be retrieved (same component).
Going from Route1 to either Route2 or Route3 works just fine and the data gets retrieved (different component).

N.B.: Going from Route2 to Route1 and then Route3 somehow works.

Edit: Same issue when I retrieve the store data in setup(), therefore it is not linked to preFetch().