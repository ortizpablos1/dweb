<template>
    <div class="contaner-fluid">
        <header>
      <h1 class="text-center">Directivas de VueJs</h1>
      <p class="border">
        Las directivas de Vue son atributos especiales que se colocan en las
        etiquetas HTML y están prefijados por v-, como por ejemplo, v-for,
        v-bind o v-on, entre muchas otras. Estas directivas permiten realizar
        acciones dinámicas potentes (bucles, condicionales, etc...) que no se
        pueden realizar en HTML por si solo, pero que Vue permite utilizar en
        sus etiquetas del template <br />
        <a href="https://vuejs.org/api/built-in-directives.html"
          >Documentacion</a
        >
      </p>

      <img src="@/assets/img/directivas-vue.png" alt="vue" />
      <p class="border">
        <b>Directiva:</b> El nombre de la directiva, que a veces, es posible
        abreviarlo con un carácter. <br />
        <b>Argumento:</b> En ciertas directivas se indica un parámetro. <br />
        <b>Modificador:</b> En ciertas directivas se puede modificar el
        comportamiento. <br />
        <b>Valor:</b> En ciertas directivas, se requiere establecer un valor. Se
        escribe como el valor de un atributo HTML.
      </p>
    </header>

    <table class="table table-success table-hover">
      <thead>
        <tr>
          <td colspan="3" class="text-center"><b>DIRECTIVAS INTEGRADAS</b></td>
        </tr>
      </thead>
      <thead>
        <tr class="text-center">
          <th class="col-sm-3">DIRECTIVA</th>
          <th class="col-sm-6">DESCRIPCION</th>
          <th class="col-sm-3">EJEMPLO</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><b>v-text</b></td>
          <td>
            Actualiza el contenido de texto del elemento <br />
            Funciona configurando la propiedad textContent del elemento, por lo
            que sobrescribirá cualquier contenido existente dentro del elemento.
            Si necesita actualizar la parte de textContent, debe usar
            interpolaciones de bigote en su lugar
          </td>
          <td></td>
        </tr>
        <tr>
          <td><b>v-html</b></td>
          <td>
            Actualiza el HTML interno del elemento. igual que el InnerHtml
            <br />
            El contenido de v-html se inserta como HTML sin formato; la sintaxis
            de la plantilla de Vue no se procesará. Si se encuentra tratando de
            componer plantillas usando v-html, intente repensar la solución
            usando componentes en su lugar.
          </td>
          <td></td>
        </tr>
        <tr>
          <td><b>v-show</b></td>
          <td>
            Alterna la visibilidad del elemento en función de la veracidad del
            valor de la expresión <br />
            v-show funciona configurando la display propiedad CSS a través de
            estilos en línea e intentará respetar el display valor inicial
            cuando el elemento esté visible. También desencadena transiciones
            cuando cambia su condición.
          </td>
          <td></td>
        </tr>
        <tr>
          <td><b>v-if</b></td>
          <td>
            Representa condicionalmente un elemento o un fragmento de plantilla
            en función de la veracidad del valor de la expresión. <br />

            Cuando v-ifse alterna un elemento, el elemento y sus
            directivas/componentes contenidos se destruyen y reconstruyen. Si la
            condición inicial es falsa, el contenido interno no se representará
            en absoluto.
          </td>
          <td></td>
        </tr>
        <tr>
          <td><b>v-for</b></td>
          <td>
            Renderiza el elemento o el bloque de plantilla varias veces en
            función de los datos de origen. <br />
            El valor de la directiva debe usar la sintaxis especial alias in
            expression para proporcionar un alias para el elemento actual que se
            está iterando <br />
            Para obligarlo a reordenar los elementos, debe proporcionar una
            sugerencia de orden con el key atributo especial <br />
            <a
              href="https://lenguajejs.com/vuejs/directivas-vue/v-for/directiva-v-for.png"
              >Explicacion Grafica</a
            >
          </td>

          <td></td>
        </tr>
        <tr>
          <td><b>v-on</b></td>
          <td>
            Directiva utilizada para gestionar los eventos del DOM desde los
            templates de Vue, haciendo más cómodo y práctico su utilización,
            permitiendo escribir mucho menos código. Así pues, nos ahorramos
            realizar .addEventListener(), y en su lugar definimos las acciones
            de forma mucho más directa. <br />
            <a href="https://lenguajejs.com/vuejs/directivas-vue/v-on/v-on.png">
              Acciones Directas</a
            >
          </td>
          <td></td>
        </tr>
        <tr>
          <td><b>v-bind</b></td>
          <td>
            Permite enlazar (bindear) una variable de Vue con un atributo
            específico de una etiqueta HTML. De esta forma, podemos colocar como
            valor de un atributo HTML el contenido que tengamos almacenado en
            una variable de la lógica de Javascript. <br />
            <a
              href="https://lenguajejs.com/vuejs/directivas-vue/v-bind/v-bind.png"
              >Uso</a
            >
          </td>
          <td></td>
        </tr>
        <tr>
          <td><b>v-model</b></td>
          <td>
            Cree un enlace bidireccional en un elemento de entrada de formulario
            o un componente. <br />
          </td>
          <td></td>
        </tr>
        <tr>
          <td colspan="3">
            Teoria: <br />
            Data : Billy - Isaac - Hernan dario<br />
            Methods: felipe -carlos <br />
            Props: felipe s - jhon hurtado <br />
            Mounted: Esteba s- jhonatan s - <br />
            Created: jhoan mu- santiago vial-miguel <br />
            Computed: wilmer - yeison -karen <br />
            Whatch: wilosn f -ricardo g <br />
            Destroyed: Andrea -angie <br />
            ciclo de vida de vue: fernando g - jhon ri <br />
            Components: Eleny
          </td>
        </tr>
      </tbody>
    </table>
    </div>
</template>

<script>
export default {
    name: 'DirectivasComponent',
    setup() {
        
    }
}
</script>
<style scoped>

</style>
