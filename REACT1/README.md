# React Basic Syntax

## Function definition new way
```bash
const ayush = ({paramters})=> {functionality};
```

## Time:
```bash
const hour = new Date().gethours(); // Gives hours
const time = new Date().toLocaleTimeString(); // Gives Time
```

## If, else if and else Loop for Selecting:
```bash
const data = hour<12 ? "Good Morning" : hour<18 ? "Good AfterNoon" : "Good Evening";
```

## Calling Different files in a Div:
### First Import The Files
```bash
import Header from './Header';
```
Note: Your File Name Should Be Header for this Import to Work

```bash
<div>
    <Header />
    <Footer />
</div>
```

## Displaying Lists with map function:
```bash
<ul>
{list.map((list , iterator)=>(
    <li key={iterator}>{list}</li>
))}
<ul>
```
### All should be under {list.map()} and inside this how the function is being defined will be there like ({paramters}) => (functionality)

Example:
const fruits = ["Apple" , "Banana" , "Cherry"];

```bash
<ul>
{fruits.map(()=>(
    <li key={index}>{fruits}</li>
))}
</ul>
```

## inline CSS
```bash
const mystyle = {
    color : "blue";
    fontSize : "20px";
}

return (
    <h1 style={mystyle} > Styled Theme </h1> 
);
```

## Button Definition
### Two Ways:
Example: Define The Function Earlier
```bash
// Its Wrong But You understand the Logic
function haha(){
    return (<h1> "haha" </h1>);
}

function Main(){
    return(
        <div>
        <button onClick = {haha}> Click Me <button>;

    );
}
```
OR
```bash
function Main(){
    return(
        <div>
        <button onClick = {()=>{return (<h1> "haha" </h1>);}}> Click Me <button>;

    );
}
```

## useState and useEffect

### useState
Syntax
### const [variable , setVariable] = useState("Any Pre Defined Value of variable)
So Always when we have to dynamically change the variable name we use this , and only the setVaribale is used even in funvtions to chage it.
Example:
```bash
const [time , setTime] = useState(new Date().toLocaleTimeString);
const function = () => {setTime("MadarChod")};
Now call it in Main function which u are exporting
```

### useEffect
### Before let's see what setInterval does
setInterval("Your Functionality");
```bash
setInterval(() => {
    // Function You want to perform Mutiple Times
    when u want to fetch latest value use setVariable(varibale=>variable+1);

},1000);
```

### useEffect
Syntax
```bash
useEffect(() => {
  // do something after render

  return () => {
    // cleanup when component unmounts or before next effect
  };
}, [dependencies]); // controls when it runs
```
Example:
```bash
useEffect(()=>{
    setInterval(()=>{
        setCount(count=>count+1);
    },1000);
},[]);
```





