import { useState } from "react"



export const counter= ()=> {

const [ counter, setstate]= useState(0);

const incrementar =(numero: number=1) :void =>{
    
    setCounter(counter + 1);
}


    return (
        <div className="mt-5">
            <h3> counter: usestates
        <span> valor:{ counter}</span>
        <br/>
        <button
        onClick={()=>incrementar()}
        className = "btn btn-outline-primary mt-2 "> 
            +1
        </button>
        <button
        onClick={()=>incrementar(2)}
        className = "btn btn-outline-primary mt-2 "> 
            +2
        </button>
        <button
        onClick={()=>setCounter(0)}
        className = "btn btn-outline-danger mt-2 "> 
            +2
        </button>
            </h3>
        </div>
    )
}

function setCounter(arg0: number) {
    throw new Error("Function not implemented.");
}
