javascripting-with-dogs
===

javascript is fun and all, but javascripting with dogs is way more exciting. in this tutorial, i'll go over the basics of javascript, but add in some cute pups along the way. 

###setting a variable 
``` 
var dog = 'homer'

var puppy = 'plato'

console.log('meet ' + dog + ' and ' puppy) 
```

 ==> this will print: **meet homer and plato**

![homer](/img/homer.jpg)

##arrays
```
var dogs = ['homer', 'plato]

console.log(dogs[0] + ' loves ' + dogs[1])

```

==> this will print: **homer loves plato**

![Alt text](/img/homerandplato.jpg)

##objects in arrays 
```
var dogs = [{name: 'homer', age: 5}, {name: 'Plato', age: 4}]

console.log('the dogs are ' + dogs[0].age ' and ' + dogs[1].age)

```

==> this will print: **the dogs are 5 and 4**

![Alt text](/img/180831_1599740081972_7795070_n.jpg)

![Alt text](/img/plato3.jpg)


## the foreach loop
```
var dogs = [{name: 'homer', age: 5, breed: 'labradoodle'}, {name: 'Plato', age: 6, breed: 'husky'}]

dogs.forEach(function(dog) {
  
  console.log(dog.breed)

}
```

==> this will print: **{'labradoodle', 'husky'}**

![Alt text](/img/plato10.jpg)

![Alt text](/img/homer10.jpg)

##the push method
```
var dogs = [{name: 'homer', age: 5, food: 'hotdogs'}, {name: 'Plato', age: 6, food: 'chipotle'}, {name: 'Scooter', age: 10, food: 'greenies}]

var fav_food = []

dogs.forEach(function (dog) {
 fav_food.push(dog.food)
})

console.log(fav_food)
```
==> this will print: **['hotdogs','chipotle','greenies']**

![Alt text](/img/homerandplato2.jpg)

![Alt text](/img/scooter.jpg)


##thanks for reading!
hopefully you learned something about some javascipt basics...but if you didnt, hopefully you appreciated the cute puppies. shoutout to homer, plato, and scooter for their good looks.

<div align="center">
        <img width="45%" src="img/downingandplato.jpg" alt="Downing" title="I love my Plato!"</img>
        <img height="2" width="4px">
</div>
