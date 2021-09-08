# Assignment2-yerramothu

****

# Dinesh Yerramothu 
#### My Favorite city is Hyderabad.
Hyderabad is the state's largest and most well-known city. **This city's residents come from a variety of religious and cultural origins. Christians, Muslims, and Hindus are all represented.** The Husain Sagar separates the twin cities of Hyderabad and Secunderabad, also known as **Hyderabad and Secunderabad.** There are many different types of people, each having their own languages, clothing, religion, and so on. Listed below are some of the most common.The city is also known for producing **various films** in the **Telugu language,** which is also known as **Tollywood**. Hyderabad's intercity transportation system is well-known. **my favourite part is Hyderabadi biryani, also known as Hyderabadi dum biryani,** is a style of biryani from Hyderabad, India made with basmati rice and goat meat and cooked with the dum pukht method. Originating in the kitchens of the Nizam of Hyderabad, it combines elements of Hyderabadi and Mughlai cuisines.

******

# Directions from Maryville to Hyderabad
1. Firstly, We are going to fly Hyderabad VIA KANSAS-CHICAGO-DOHA-HYDERABAD 
2. Getting started from Maryville City via cab to Kansas City Airport(MCI) as per scheduled time.
3. Check-in and board the flight in Kansas and relax for 2hrs(Approx) and you'll be reaching Chicago Airport.
4. Check for next flight time and head to the terminal and wait at the lobby. 
5. When the time is right, board your next flight and relax for 15hrs(Approx) and after reaching Doha. gohead for right terminal and check-in to last flight to reach Hyderbad.

### Things required for travel
* Camera
* Powerbank and chargers
* Laptop
* Snacks


[Click here to know about Me](AboutMe.md)

*****

# Victuals
Below are some of my favourite recomendations that you should try.

| Food/Drink | Location | Cost
| -- | -- | -- |
| Burgundy Wine | France | $125  |
| Chicken Chettinad | Chennai  | $18 |
| Naturals Ice Cream | Mumbai | $15 |

*****

# Pithy Quotes

> "If you are good at something never do it for free." - **The Joker** 

> "The deepest craving of human nature is the need to be appreciated." - **Willam James**

*****

# Code Fencing

> In graph theory, a component of an undirected graph is an induced subgraph in which any two vertices are connected to each other by paths, and which is connected to no additional vertices in the rest of the graph. For example, the graph shown in the illustration has three components. A vertex with no incident edges is itself a component. A graph that is itself connected has exactly one component, consisting of the whole graph. Components are also sometimes called connected components.

Search for connected components in a graph: (https://en.wikipedia.org/wiki/Component_(graph_theory))

Sample Code as follows:

int n;
vector<int> g[MAXN] ;
bool used[MAXN] ;
vector<int> comp ;

void dfs(int v) {
    used[v] = true ;
    comp.push_back(v);
    for (size_t i = 0; i < (int) g[v].size(); ++i) {
        int to = g[v][i];
        if (!used[to])
            dfs(to);
    }
}

void find_comps() {
    for (int i = 0; i < n ; ++i)
        used [i] = false;
    for (int i = 0; i < n ; ++i)
        if (!used[i]) {
            comp.clear();
            dfs(i);
            cout << "Component:" ;
            for (size_t j = 0; j < comp.size(); ++j)
                cout << ' ' << comp[j];
            cout << endl ;
        }
}

Link for the source code: (https://cp-algorithms.com/graph/search-for-connected-components.html)


