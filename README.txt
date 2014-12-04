A responsive portfolio site for Actor and Writer Patrick Askin.

Features a flat, minimalistic design, a fully animated 
interface and noscript fallbacks.

Initial page load time was over 15 sec, so I included the following optimizations:
* Pictures minimized: resized and compressed (using http://pictureslash.com/)

* Load CSS in header, and JS files in footer to ensure asynchronous loading.

* Youtube was requesting HTML, CSS, JS, and even Flash with its iframes, so instead of using iframe, I load a static image with an overlayed "play" icon which then loads the actual video when clicked.

* Vimeo is also causing delays with its iframes, requesting ConviviaCommunications, testing https connections and servers, and slowing everything down immensely. These will be moved to youtube as well, and will use the previous fix.

Credits:
		
	Icons:
		Font Awesome (fortawesome.github.com/Font-Awesome)

  Amazing Youtube ptimizations:
    Amit Agarwal (http://www.labnol.org/internet/light-youtube-embeds/27941/)
		
	Other:
		jQuery (jquery.com)
		html5shiv.js (@afarkas @jdalton @jon_neal @rem)
		background-size polyfill (github.com/jefferyto)
    HTML5UP (html5up.net)
		skel (n33.co)



