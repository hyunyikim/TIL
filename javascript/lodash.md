## null 체크

### isNil

-   null, undefined 체크

```js
_.isNil(null);
// => true

_.isNil(NaN);
// => false
```

### isNull

-   null 체크

```js
_.isNull(null);
// => true
```

### isEmpty

-   empty object, collection, map, or set 체크

```js
_.isEmpty(null);
// => true

_.isEmpty(true);
// => true

_.isEmpty(1);
// => true

_.isEmpty([1, 2, 3]);
// => false

_.isEmpty({ a: 1 });
// => false
```

[https://lodash.com/docs/4.17.15](https://lodash.com/docs/4.17.15)
