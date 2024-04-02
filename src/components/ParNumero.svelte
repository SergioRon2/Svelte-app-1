<script>
    let numero
    let resultado 
    $:if(numero == 0 ){
        resultado = `El numero ${numero} es Neutro`;
        }
        else if(numero === undefined){
            resultado = `El numero aun no esta definido`
        }
        else{
            if(numero % 2 == 0){
                resultado=`El numero ${numero} es par`
            }else{
                resultado=`El numero ${numero} es impar`
            }
        }
    const listen = (event) => numero = event.target.value
</script>





<p>{resultado}</p>
<input type="number" on:input={listen} value={numero}>

<style>
    p{
        color: rgb(32,4,112);
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-size: 25px;
    }
    input{
        background-color: #fff;
        outline: none;
        border: none;
        border-bottom: 1px solid #000;
        color: #000;
    }
</style>

