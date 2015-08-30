Selectores
==========

Los selectores son probablemente la parte mas importante que necesitaras entender de css, el correcto uso de los selectores te permtira crear hojas de estilo funcionales y correctamente organizadas.

Por suerte los selectores css son bastante sencillos de entender y aprender.

Existen varios tipos de selectores

1. elemento
2. id
3. clase
4. pseudo clases
5. pseudo elementos

Los selectores siguen una estructura jerarquica, es decir se puede especificar un estilo para un elemento seleccionando su elemento padre y despues su desendencia.

Clarifiquemos esto aun mas con un ejemplo, considera el siguiente documento html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
</head>
<body>
    <header>
        <h1>Bajo la rueda</h1>
    </header>
    <main>
        <h1>Capitulo 1</h1>
    </main>
</body>
</html>
```

```css
h1: {
    color: navy;
}

head h1{
    font-size: 3em;
}

main h1{
    font-size: 1.5em;
}

```

Ambos elementos header y main cuentan con un elemento "hijo" h1, para referirnos a cada uno de esos elementos de manera individual podemos hacerlo mediante la seleccion de su elemento contenedor o padre y luego el selector del elemento particular.

