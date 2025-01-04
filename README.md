# counter-program
Increment decrement counters..
import react,{useState} from 'react'


function Counter(){
    const [number, setNum]=useState("0");
    const setNumber=()=> {
            setNum(number +1 );
    }
    const resetNumber=()=> {
        setNum(0);
}
const decrementNumber=()=> {
    setNum(number -1 );
}
    return(
        <div className="file">
        <p className="number">{number}</p>
        <button className="increment" onClick={setNumber}>Increment</button>
        <button className="reset" onClick={resetNumber}>Reset</button>
        <button className="decrement" onClick={decrementNumber}>Decrement</button>
        </div>
    );
}
export default Counter
<br> 
import Counter from './Counter.jsx'
function App() {
  return( <Counter/>);
}

export default App
<br>
*{
    margin: 0px;
    padding: 0px;
    
}

.increment{
    padding: 2px;
    font-size: 25px;
    font-family:'Times New Roman', Times, serif;
    color: black;
    border-radius: 10px;
    box-shadow: 3px 3px 5px;
    background-color: rgb(244, 240, 240);
    margin: 10px 10px;
    cursor: pointer;
    margin-top: 20px;
    margin-left: 550px;
}
.increment:hover{
    background-color: rgb(212, 207, 207);
    padding: 10px;
}
.reset{
    padding: 2px;
    font-size: 25px;
    font-family:'Times New Roman', Times, serif;
    color: black;
    border-radius: 10px;
    box-shadow: 3px 3px 5px;
    background-color: rgb(244, 240, 240);
    margin: 10px 10px;
    cursor: pointer;
}
.decrement{
    padding: 2px;
    font-size: 25px;
    font-family:'Times New Roman', Times, serif;
    color: black;
    border-radius: 10px;
    box-shadow: 3px 3px 5px;
    background-color: rgb(244, 240, 240);
    margin: 10px 10px;
    cursor: pointer;
}

.reset:hover{
    background-color: rgb(212, 207, 207);
    padding: 10px;
}
.decrement:hover{
    background-color: rgb(212, 207, 207);
    padding: 10px;
}
.number{
    font-size: 100px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    margin-left: 140px;
    margin-top: 200px;
    margin-left: 680px;
}

