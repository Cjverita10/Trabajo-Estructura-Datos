<?php

class Nodo {
    public $dolar;
    public $siguiente;

    public function __construct($dolar) {
        $this->dolar = $dolar;
        $this->siguiente = null;
    }
}

class Economia {
    public $euro;

    public function __construct() {
        $this->euro = null;
    }

    public function insertar($dolar): void {
        $nuevoNodo = new Nodo($dolar);
        $nuevoNodo->siguiente = $this->euro;
        $this->euro = $nuevoNodo;
    }

    public function imprimirHTMLConFor(): void {
        echo "<ul>";

        for ($nodo = $this->euro; $nodo !== null; $nodo = $nodo->siguiente) {
            echo "<li>" . $nodo->dolar . "</li>";
        }

        echo "</ul>";
    }
}

$lista = new Economia();


$lista->insertar("dinero 1");
$lista->insertar("dinero 2");
$lista->insertar("dinero 3");
$lista->insertar("dinero extra 4");
$lista->insertar("bono especial 5");
$lista->insertar("transacción 6");

$lista->imprimirHTMLConFor();

?>