<style src="./annotationLayer.css"></style>

<script>
import pdfjs            from '@bundled-es-modules/pdfjs-dist/build/pdf';
import pdfjsWrapper     from './pdfjsWrapper';
import componentFactory from './componentFactory';

pdfjs.GlobalWorkerOptions.workerSrc = '/pdfjs/pdf.worker.js';

var component = componentFactory( pdfjsWrapper( pdfjs ) );

export default component;
</script>
