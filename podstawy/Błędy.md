1.   Błąd kiedni nie dodamy export default

```
Uncaught SyntaxError: The requested module '/src/App.jsx' does not provide an export named 'default' (at main.jsx:4:8)
```
### Rozwiązanie:

```JavaScript
export default App
```
