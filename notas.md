Sin embargo, el contenido es estático. Soluciones para contenido dinámico:

1. Si los datos se envían: depúralos con Herramientas para desarrolladores -> Network -> XHR y obtendrás el origen directamente.

2. Si los datos se ejecutan: Mete el resultado de la petición en bruto en el srcdoc de un iframe y usa el atributo onload
para obtener el "this.contentDocument". Tendrás que adjuntarlo al documento, pero siempre puedes hacer iframe.hidden = true.
También puede ser necesario cambiar el base href.

3. Si los datos se envían y se ejecutan: Intenta el caso dos o busca una API. Si no, no puedes hacer web scraping desde el
navegador. Además, necesitarás una herramienta bastante avanzada para hacerlo.
