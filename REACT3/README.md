# LETS DO REAL SHIT NOW PROP TYPES

## Array for a useState Variable

```bash
const [Contact , setContact] = useState([
    {id: 1 , Name:"Alice"}, // You must use : for specifying the values inside an object variable
    {id: 2 , Name:"Ayush"}
]);
```

### Using setContact     for this is lil Different
```bash
const [input, setInput] = useState(''); // For adding input values
setContact([...Contact , {id: Date.now() , name: input} ]);
```

## Prop Types 
Its actually nothing but just to add a constraint on your input so it is seen early in dev warning

### Import the Prop Types
```bash
import PropTypes from 'prop-types';
```

### Now we have to specify inside a function
```bash
function contact({contact , onDelete}){ // Here u see we are treating the onDelete as a Function type , it is used a function
    return()
        <div>
            <button onClick={()=> onDelete(contact.id)>Delete</button>;
        </div>
    );
}
```

### At the End Specify the Prop constraints
```bash
contact.propTypes = {
    contact: PropTypes.object.isRequired,
    onDelete: PropTypes.func.isRequired
};
```

Now export and when u are calling in App.js there wlll be two types
1. Where u specify a key . generally when you are using a list or object
2. Where u just specify the parameters not a key

## I will use here a key
```bash
import contact from './file_name';
function deleteContact(){} // Just for a PlaceHolder Function
fuction App(){
    return(
        <contact key={Contact.id} contact={Contact} oneDelete={deleteContact}>
    );
}
```

## eval in js - convert string into maths expression to calculate











