```Js
    const like_name = () =>{
        if(counter>=10){
            return <p>Gratuluję masz już 10 lików</p>
        }
        return null
    }
    
```

Potem w kodzie używamy:
```Js
<div>
	{like_name()}
</div>
```

Można też krócej:
```JS
{counter >= 10 && <p>Gratulacje jest już 10</p>}
```