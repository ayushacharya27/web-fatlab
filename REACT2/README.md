# NOW DONE WITH BASICS LETS DO REAL SHIT
First You have to Import the the component from react
## import React , { Component } from "react";

```bash
class Example extends Component{
    constructor(props){
        super(props); // Just to call the constructor 

        this.state{name:"Alice"}; // State initialization
    }


    // Always use a Render Block for Class bullshit , just 

    render(){
        return(<h1> {this.state.name} </h1>);
    }
}
export default Example;
```
### You can as many functions you want inside the class component it will go modular wise

## Taking and storing input:

### SYNTAX

POINT: Always create a useState Variable before using input , because you want the value to show somewhere right??
```bash
const [field_name , setField] = useState("");
<input
    type="type of your input"
    value = {field_name} // if you want to directly save the value
    onChange = {(e) => setField(e.target.value)}
/>
```

