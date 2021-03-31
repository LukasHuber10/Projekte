<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
    <link rel="stylesheet" href="https://code.getmdl.io/1.3.0/material.indigo-pink.min.css">
    <script defer src="https://code.getmdl.io/1.3.0/material.min.js"></script>
    <title>Document</title>
    <style>
        .page-content{
            padding: 50px 200px;
        }
        .demo-list-control {
          width: 300px;
        }
    </style>
    <script>
        function Funktion(){
            Ausgabe.innerHTML += `
            <li class="mdl-list__item">
                  <span class="mdl-list__item-primary-content">
                    <i class="material-icons  mdl-list__item-avatar">label</i>
                    ${todofield.value}
                  </span>
                  <span class="mdl-list__item-secondary-action">
                    <label class="mdl-checkbox mdl-js-checkbox mdl-js-ripple-effect" for="list-checkbox-1">
                      <input type="checkbox" id="list-checkbox-1" class="mdl-checkbox__input" />
                    </label>
                  </span>
                </li>
            `;
            todofield.value = ""
        }
    </script>
</head>
<body>
            <!-- Always shows a header, even in smaller screens. -->
<div class="mdl-layout mdl-js-layout mdl-layout--fixed-header">
    <header class="mdl-layout__header">
      <div class="mdl-layout__header-row">
        <!-- Title -->
        <span class="mdl-layout-title">To do Liste</span>
        <!-- Add spacer, to align navigation to the right -->
        <div class="mdl-layout-spacer"></div>
        <!-- Navigation. We hide it in small screens. -->
        <nav class="mdl-navigation mdl-layout--large-screen-only">
          <a class="mdl-navigation__link" href="">Link</a>
          <a class="mdl-navigation__link" href="">Link</a>
          <a class="mdl-navigation__link" href="">Link</a>
          <a class="mdl-navigation__link" href="">Link</a>
        </nav>
      </div>
    </header>
    <div class="mdl-layout__drawer">
      <span class="mdl-layout-title">To do Liste</span>
      <nav class="mdl-navigation">
        <a class="mdl-navigation__link" href="">Link</a>
        <a class="mdl-navigation__link" href="">Link</a>
        <a class="mdl-navigation__link" href="">Link</a>
        <a class="mdl-navigation__link" href="">Link</a>
      </nav>
    </div>
    <main class="mdl-layout__content">
      <div onsubmit="Funktion()" class="page-content">
        <div>
            <div class="mdl-textfield mdl-js-textfield mdl-textfield--floating-label">
            <input class="mdl-textfield__input" type="text" id="todofield">
            <label class="mdl-textfield__label" for="todofield">To do einfügen</label>
        </div>

            <button onclick="Funktion()" class="mdl-button mdl-js-button mdl-button--raised mdl-button--colored">
                Hinzufügen
            </button>
            
        </div>

        <ul class="demo-list-control mdl-list" id="Ausgabe">

        </ul>
    </div>




        </div>
    </main>
  </div>


    
</body>
</html>
