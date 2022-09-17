## [rsschool-cv](https://google.com)
***
# Roman Li
***
## Contacts
* Location: Moscow, Russia
* Mobile: +79037289196
* Email: romanri85@gmail.com
* Github:romanri85
## About Me
I have been interested in programming for several years already. I like coding because it gives me an opportunity 
to create something useful. Though my current job is rather far from web-development, I am really interested in this 
field.
***
## Skills
* HTML&CSS (Bootstrap, SASS)
* Javascript
* Node.js
* Python(Django, Flask, Beautiful Soup)
* REST API(Django Rest Framework, Swagger)
* GIT

### [Hackerrank Certificates](https://www.hackerrank.com/romanri85?hr_r=1)
***

## Code Example

Pete likes to bake some cakes. He has some recipes and ingredients. Unfortunately he is not good in maths. 
Can you help him to find out, how many cakes he could bake considering his recipes?

Write a function cakes(), which takes the recipe (object) and the available ingredients (also an object) and returns 
the maximum number of cakes Pete can bake (integer). For simplicity there are no units for the amounts (e.g. 1 lb of 
flour or 200 g of sugar are simply 1 or 200). Ingredients that are not present in the objects, can be considered as 0.

```javascript
function cakes(recipe, available) {
    for (let i of Object.keys(available)) {
        if (!recipe[i]) {
            delete available[i]
        }
    }
    if (Object.keys(available).length !== Object.keys(recipe).length) {
        return 0
    }
    let count = 0
    while (true) {

        if (Object.keys(available).every((el) => (available[el] >= recipe[el]))) {
            count++
            for (let i of Object.keys(recipe)) {
                available[i] = available[i] - recipe[i]
            }
        } else {
            break
        }
    }
    return count
}
```
## Education
***
Moscow State Institute Of International Relations (Oriental Studies)

### [JetBrains Academy](https://hyperskill.org/profile/147085522)

### [Code Academy](https://www.codecademy.com/profiles/romanLi9865307131)

## Language Proficiency
***
* Russian - Native
* English - Advanced
* Korean - Intermediate






