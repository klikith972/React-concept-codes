# React-concept-codes
each concepts code will be updated here
//import logo from './logo.svg';
import { useState } from 'react';
import './App.css';
//import imageone from './images/1.img.JPG';
import './index.css'; 

function App() {

let [userdata,setUsername] = useState({
  username:"evado gottam gadu",
  salary: 32200,
  city: 'vikarabad'
})

const changeusername=()=>{
  setUsername({
    ...userdata,
    salary:80000,
    city: 'banglore'
  })
}


  return (

    <div className='text-center'>
    <h1 className='text-info display-1'>boku lo projectlu bro</h1>
    <button className="btn btn-info" onClick={changeusername}>changeusername</button>
    <p className="display-2 text-primary">{userdata.username}</p>
    <p className="display-2 text-warning">{userdata.salary}</p>
    <p className="display-2 text-danger">{userdata.city}</p>
  </div>  
);
};
 


export default App;
