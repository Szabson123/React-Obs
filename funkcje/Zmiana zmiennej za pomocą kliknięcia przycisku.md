Tworzymy const który przekażemy do przycisku:
```JS
const [name, setName] = useState("Geralt");

const changeName = () => {
setName("Yennefer")
}

<button onClick={(e) => changeName()}>Zmień imię</button>
```

Można też zmieniać bo name przechowuje aktualny stan:

```JS
const changeName = () =>{
	if (name === "Geralt"){
		useState("Yennefer")
	}
	else{
		useState("Geralt")
	}
}
```

Przekazanie takie same:

```JS
<button onClick = {(e) => changeName()}>Aby zmienić imię naciśnij</button>
```
