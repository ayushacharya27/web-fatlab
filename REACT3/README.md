# LETS DO REAL SHIT NOW PROP TYPES

## Array for a useState Variable

```bash
const [Contact , setContact] = useState([
    {id: 1 , Name:"Alice"}, // You must use : for specifying the values inside an object variable
    {id: 2 , Name:"Ayush"}
]);
```

### Using useState for this is lil Different
```bash
setContact([...Contact , {id: Date.now() , name: input} ]);
```







