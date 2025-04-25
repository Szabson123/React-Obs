```JS
import './App.css'
import Welcome from './components/Welcome'
import { useState } from 'react'

function App() {
  const[name] = useState("Władek")
  
  return(
   <div>
    <Welcome name={name}/>
  </div>
  )
}
export default App
```

[[Dynamiczne przekazywanie (input)]]
[[Zmiana zmiennej za pomocą kliknięcia przycisku]]
