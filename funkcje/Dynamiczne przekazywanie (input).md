Potrzebny jest nowy import:
```JS
import { useState } from 'react'
```

Dodajemy nową zmienna do const aby zmieniała stan naszej aplikacji:

```JS
const[name, setName] = useState("")
```

Teraz dodajemy nasz input:

```JS
	<input
		type="text"
		value = {name}
		onChange = {(e) => setName(e.target.value)}
	/>
```

Teraz input dynamicznie zmienia nam imię 

![[Pasted image 20250425190553.png]]

