<script>
  export let pais;
  let p;
  const paises = {
  "colombia": ["Colombia", "Bogota", "51,52 Millones", "Peso Colombiano", "1.142 millones","Colombia.png"],
  "venezuela": ["Venezuela", "Caracas", "28,52 Millones", "Bolívar Venezolano", "482.4 mil millones","Venezuela.jpg"],
  "ecuador": ["Ecuador", "Quito", "17,08 Millones", "Dólar(USD) ", "184.9 mil millones","Ecuador.svg"],
  "brasil": ["Brasil", "Brasilia", "212,55 Millones", "Real Brasileño", "1.869 billones","Brasil.jpg"],
  "peru": ["Perú", "Lima", "32,17 Millones", "Sol Peruano", "227.5 mil millones","Peru.png"]
};


  p=paises[pais];
</script>

<div class="mainDiv">
  <div class="col1">
    <img draggable="false" src="../public/{p[5]}" alt="Hola"  width="300" height="300"/>
  </div>

  <div class="col2">
    <div class="linea"><strong>Pais: </strong>{p[0]}</div>
    <div class="linea"><strong>Capital: </strong>{p[1]}</div>
    <div class="linea"><strong>Poblacion: </strong>{p[2]}</div>
    <div class="linea"><strong>Moneda: </strong>{p[3]}</div>
    <div class="linea"><strong>Extension: </strong>{p[4]}</div>
  </div>
</div>

<style>

  img{
    object-fit: cover;
  }
    
    .mainDiv{
        user-select: none;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 10px;
        border-style: solid;
        border-color: rgb(186,190, 182);
        border-width: 2px;
        margin: left;
        width: 600px;
        box-shadow: 1px 2px 5px black;
        margin-right: 5px;
        margin-bottom: 10px;
    }

    .col1{
        width: auto;
        margin: 5px;
        padding: 15px;
    }

    .col2{
        text-align: start;
        margin: 5px;
        padding: 5px;
        border-color: black;
        width: max-content;
    }

    strong{
        color: red;
        font-weight: bolder;
    }

    .linea{
        color: black;
        font-size: 20px;
        margin-bottom: 18px;
    }

</style>