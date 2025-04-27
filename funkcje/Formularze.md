1. Tworzymy Pola formularza:
```JS
    const[name, setName] = useState("")
    const[surname, setSurname] = useState("")
    const[email, setEmail] = useState("")
```
2. Tworzymy funkcje do submitowania i ustwania ayb nasza storna się nie odświeżała 
```JS
    const [submittetData, setSubmittedData] = useState(null)
    const handleSubmit = (e) => {
        e.preventDefault();
        setSubmittedData({
            name, surname, email
        })
    }
```
3. Formularz w html:
```JS
        <div>
            <form onSubmit={handleSubmit}>
			    <input type="text" value={name} onChange={(e) => setName(e.target.value)}/>
                <input type="text" value={surname} onChange={(e) => setSurname(e.target.value)}/>
                <input type="text" value={email} onChange={(e) => setEmail(e.target.value)}/>
                <button type="submit">Wyślij</button>
            </form>
            {submittetData && <p>Imię: {submittetData.name} Nazwisko: {submittetData.surname}, Email: {submittetData.email}</p>}
        </div>
```