# React Basic Syntax
## Time:
```bash
const hour = new Date().gethours(); // Gives hours
const time = new Date().toLocaleTimeString(); // Gives Time
```
## If, else if and else Loop for Selecting:
```bash
const data = hour<12 ? "Good Morning" : hour<18 ? "Good AfterNoon" : "Good Evening;
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
Example:
```bash
<u>