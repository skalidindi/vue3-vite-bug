# Run the code

```
npm install
npm run dev
```

Navigate to
```
http://localhost:3000/src/App.vue?vue&type=style&index=0&scoped=7a7a37b1&lang.css
```

This url returns the correct javascript output.

However, if you change the order of the query params such as
```
http://localhost:3000/src/App.vue?vue&type=style&lang.css&index=0&scoped=7a7a37b1
```

The returns a completely different result (parsed css).

This behavior is not consistent as order of query should not matter for a given output.

