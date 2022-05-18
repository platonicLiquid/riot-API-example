# Home
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Table of Contents
* [Home](README.md#home)
* [Sample Page 1](README.md#sample-page-1)
* [API Example](README.md#api-example)

# Sample Page 1

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

# API Example
## Find Champion
### Overview
The **Find Champion** funtion returns champion info and allows searching by champion name, role, origin. This function returns a list of dictionaries. When searching by name, it will return a list with only one element. When searching by role or origin, this function will return a list with multiple dictionaries with each dictionary corresponding to a matching champion.

### Syntax

find_champion(name = None, role = None, origin = None)

### Examples
**Searching by Champion**

Searching for a single champion
```
champion_to_search_for = find_champion(name = 'miss_fortune')
```
will return:

> [{'name': 'miss fortune', 'role': 'marksman', 'origin': 'bilgewater'}]


**Searching by Origin**

Searching by origin
```
origin_to_search_for = find_champion(origin = 'bilgewater')
```
will return:
> [{'name': 'gangplank', 'role': 'top lane', 'origin': 'bilgewater'}, {'name': 'miss fortune', 'role': 'marksman', 'origin': 'bilgewater'}]

