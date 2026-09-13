# Ex06 BMI Calculator
## Date: 4-09-2026

## AIM
To create a BMI calculator using React Router 

## ALGORITHM
### STEP 1 State Initialization
Manage the current page (Home or Calculator) using React Router.

### STEP 2 User Input
Accept weight and height inputs from the user.

### STEP 3 BMI Calculation
Calculate the BMI based on user input.

### STEP 4 Categorization
Classify the BMI result into categories (Underweight, Normal weight, Overweight, Obesity).

### STEP 5 Navigation
Navigate between pages using React Router.

## PROGRAM
```
App.jsx
import { BrowserRouter, Routes, Route } from "react-router-dom";
import Home from "./Home";
import BMI from "./BMI";
import Result from "./Result";
import "./App.css";

function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/bmi" element={<BMI />} />
        <Route path="/result" element={<Result />} />
      </Routes>
    </BrowserRouter>
  );
}

export default App;
```
```
App.css
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: linear-gradient(135deg, #667eea, #764ba2);
  min-height: 100vh;
}

nav {
  background: white;
  padding: 18px;
  display: flex;
  justify-content: center;
  gap: 30px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
}

nav a {
  text-decoration: none;
  color: #333;
  font-weight: bold;
}

.page {
  min-height: 90vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: white;
  text-align: center;
}

.page h1 {
  font-size: 45px;
  margin-bottom: 10px;
}

.page p {
  font-size: 20px;
  margin-bottom: 30px;
}

.button,
button {
  background: white;
  color: #667eea;
  border: none;
  padding: 14px 25px;
  border-radius: 8px;
  font-size: 16px;
  font-weight: bold;
  cursor: pointer;
  text-decoration: none;
}

.card {
  background: white;
  color: #333;
  padding: 35px;
  width: 350px;
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
}

.card label {
  display: block;
  text-align: left;
  margin: 12px 0 6px;
  font-weight: bold;
}

.card input {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 6px;
  font-size: 16px;
}

.card button {
  width: 100%;
  margin-top: 25px;
  background: #667eea;
  color: white;
}

.back {
  display: block;
  margin-top: 20px;
  text-decoration: none;
  color: #667eea;
  font-weight: bold;
}
```
```
Main.jsx
import { StrictMode } from 'react'
import { createRoot } from 'react-dom/client'
import './index.css'
import App from './App.jsx'

createRoot(document.getElementById('root')).render(
  <StrictMode>
    <App />
  </StrictMode>,
)
```
```
index.css
html,
body,
#root {
  margin: 0;
  min-height: 100%;
}
```

## OUTPUT

<img width="1392" height="556" alt="image" src="https://github.com/user-attachments/assets/12674251-8776-473e-86dd-787391f6c9eb" />

<img width="1402" height="551" alt="image" src="https://github.com/user-attachments/assets/44110572-7e67-4740-9258-fc169806d7d0" />



## RESULT
The program for creating BMI Calculator using React Router is executed successfully.
