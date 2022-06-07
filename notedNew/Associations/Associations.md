# Associations In Sequelize 

## Defining the Sequelize associations

In order to connect 2 models for example model food and clothes

```js 
const A = sequelize.define('food', /* ... */);
const B = sequelize.define('clothes', /* ... */);

food.hasOne(clothes); // A HasOne B
food.belongsTo(clothes); // A BelongsTo B
food.hasMany(clothes); // A HasMany B
food.belongsToMany(clothes, { through: 'C' }); // A BelongsToMany B through the junction table C
```
## Creating the standard relationships
### One-To-One relationships
The main setup to achieve the goal is as follows:


```js
Foo.hasOne(Bar);
Bar.belongsTo(Foo);
```
### One-To-Many relationships
The main way to do this is as follows:

```js
Team.hasMany(Player);
Player.belongsTo(Team);
```
 ### To change the name of the foreign key

 ```js
Team.hasMany(Player, {
  foreignKey: 'clubId'
});
Player.belongsTo(Team);
```
### Many-To-Many relationships
Implementation:

```js
const Movie = sequelize.define('Movie', { name: DataTypes.STRING });
const Actor = sequelize.define('Actor', { name: DataTypes.STRING });
Movie.belongsToMany(Actor, { through: 'ActorMovies' });
Actor.belongsToMany(Movie, { through: 'ActorMovies' });
```
## Creating, updating and deleting

```js
Bar.create({
  name: 'My Bar',
  fooId: 5
  ```
  




