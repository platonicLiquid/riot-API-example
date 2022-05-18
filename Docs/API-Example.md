* [Home](Home.md)
* [Sample Page 1](Sample-Page-1.md)
* [API Example](API-Example.md)


# API Example
## Find Champion
### Overview
The **[Find Champion](../find_champion.py)** function returns champion info and allows searching by champion name, role, origin. This function returns a list of dictionaries. When searching by name, it will return a list with only one element. When searching by role or origin, this function will return a list with multiple dictionaries with each dictionary corresponding to a matching champion.

### Syntax
**Function Syntax**

`find_champion(paramenters)`

Where *parameters* are the champion name, **or** role **and/or** origin.

**Paramenters Syntax**

`name = [name]`

`role = [role], origin = [origin]`

### Examples
**Searching by Champion**

Searching for a single champion `champion_to_search_for = find_champion(name = 'miss_fortune')` will return:
> [{'name': 'miss fortune', 'role': 'marksman', 'origin': 'bilgewater'}]


**Searching by Origin**

Searching by origin `origin_to_search_for = find_champion(origin = 'bilgewater')` will return:
> [{'name': 'gangplank', 'role': 'top lane', 'origin': 'bilgewater'}, {'name': 'miss fortune', 'role': 'marksman', 'origin': 'bilgewater'}]

**Note:** If you use an name with an incompatible role/origin (e.g. `name = 'gangplank', origin = 'ionia'`), this function will search for the name first and, if found, will return only the corresponding champion. If no matching champion is found by the given name, it will return a list of all champions for the given role/origin.
