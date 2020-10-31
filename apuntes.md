##WCAG Web-content-accessibility-guideliness
	Creados por la w3c
	Tiene 3 niveles A-AA-AAA
	Sus criterios son Perceptible-Operable-Comprensible-Robusto
#Primera parte
	Haz un audit en lighthouse
##WCAG
##Tipos de discapacidades que seran testeadas
	(Extensión ==> No cofee)
	Vision borrosa
	Protanopia: Incapacidad de ver colores rojos
	Deutranopia: Se ven más amarillos los colores
	Acromatopsia: No se puede ver ningún color
##Pruebas Manuales con el teclado
	"con tab puedes comprobar tu movimiento y ver que tipo de componentes interactivos tienen
	un borde"
##Lectores de pantalla
	Lector de pantalla --> Navegador
	NVDA		-->	Firefox
	JAWS		-->	Explorer
	VoiceOver	-->	Safari
	Chrome vox	-->	Google Chrome
	"Para ver como funciona en entra a Accesibility en el editor de estilos en chromeDevTools"
	"Generic container no dice nada"
	"Los lectores observan containers tipo 'banner' 'heading' etc.."
##Arbol de accesibilidad
##Aria accesibleRichAplications
	Roles
		"Define el tipo general del objeto articulo una alerta un deslizador"
		"Raros"
	Propiedades
		"Comunican atributos que son escenciales para el comportamiento o significado de un elemento pero se suelen comunicar visualmente
		por ejemplo agregar un texto a un icono"
		"Mas común"
		--> Se usan arial-labels para describir lo que hace algún elemento
		--> También puedes unir con el atributo html for a un label para linkearlo con un input
	Estados
		"Comunnican estados y cambios de estados en elementos que se suelen comunicar visualmente"
		--> Se usa Area hiding en el container de el focus, y esto ocultara de el medio de escucha los elementos que visualmente no están
		disponibles
## Contraste
	En el developer tools si haces hover sobre el color te sale el contrast ratio, debes de tener un ratio elevado
	=>> Si no se cumple el ratio la herramienta muestra una herramienta para proponer un contraste
##Iconos
	"Trata de que todos los iconos tengan texto desciptivo"
##Aria roles
	Define el tipo general del objeto (como un articulo, una alerta o un deslizador, deben de usarse en ocasiones especificas)
	En especial son más usados en formularios que en texto estático, lugares más que nada con mucha interaccion por parte del usuario
##Skip links
	Un boton oculto que con focus se muestra primero y manda directamente a un main
##Estilos foco y hover
	"Reseteas los estilos del focus y le das los mismos del hover, además agregas un estilo focus-within que recibira todo contenido dentro de el"
##Agrega descipciones sobre hover con Title
##Tab Index
	"Numeros negativos para elementos que no se quieren mostrar"
	"Positivos para administrar elementos"
	"0 para seguir el flujo normal del navegador"
	=>> Recuerda remover tambien los aria-hidden cuando elimines los tab-index
##Agregar a modal focus
	"Esto se logra agregando un tabindex='0' a el html"
##aria-live
	Notifica eventos que suceden en la página para quienes no pueden verla tiene dos tipos de parametros assertive y polite una más agresiva y otra 
	que no interrumpe el flujo de el lector
	=>> El texto que se dirá se añade por javascript

Prender voice over
	funcion comando f5
Rangos de contraste
	AA => 4.5
	AAA => 7.0