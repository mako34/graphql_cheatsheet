**Introspection**  
Check schema
```javascript
{
  __schema {
    types {
      name
    }
  }
}
````

types with __ mean from introspection system

**Check a type**
````javascript
{
  __type(name: "User") {
    name
    kind
    description
  }
}
````

**Fields of an object**
````javascript
{
  __type(name: "User") {
    name
    fields {
      name
      type {
        name
        kind
        ofType {
          name
          kind
        }
      }
    }
  }
}
````

