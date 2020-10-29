#Primera parte
	Haz un audit en lighthouse
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
		"Comunican atributos que son escenciales para el comportamiento o significado de un elemento pero se suelen comunicar visualmente"
		"Mas común"
		--> Se usan arial-labels
	Estados
		"Comunnican estados y cambios de estados en elementos que se suelen comunicar visualmente"
		--> Se usa Area hiding en el container mayor
## Contraste
	En el developer tools si haces hover sobre el color te sale el contrast ratio, debes de tener un ratio elevado
	=>> Si no se cumple el ratio la herramienta muestra una herramienta para proponer un contraste
##Iconos
	"Trata de que todos los iconos tengan texto desciptivo"
##Skip links
	Un boton oculto que con focus se muestra primero y manda directamente a un main
##Estilos foco y hover
	"Reseteas los estilos del focus y le das los mismos del hover, además agregas un estilo focus-within que recibira todo contenido dentro de el"