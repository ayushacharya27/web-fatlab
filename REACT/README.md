# React Basic Syntax
## Time:
```bash
const hour = new Date().gethours();
const time = new Date().toLocaleTimeString();
```
### If else if and elseLoop for Selecting:
```bash
const data = hour<12 ? "Good Morning" : hour<18 ? "Good AfterNoon" : "Good Evening;
```
## Calling Different files in a Div:
## First Import The Files
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