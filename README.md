# vuetify-upload-btn
Simple component to handle file selection for upload.

## Installation

Copy ```UploadButton.vue``` to part of our project and require/import if using bundler.

Tested to work with Vue 2.5.x and Vuetify 1.0.3 

## How to use

In your view or component import file:

```
import UploadButton from './UploadButton';
```

add it to components section:

```  export default {
    components: {
      UploadButton,
```

Set title of the button and callback function via props:

```
<upload-button title="Browse" :selectedCallback="fileSelectedFunc">
</upload-button>
```

### Callback function

Vital part of functionality is the callback function. When you have selected file or cancelled new selection you will get callback with the given file (as ```File``` -object). File can be then passed to e.g. to Vue-Resource to do the actual upload. Callback will send ```null``` if selection of new file was cancelled.
More info about [File -object](https://developer.mozilla.org/en-US/docs/Web/API/File) in the MDN. 

### Styling
If you want to modify styles do it in the component file directly. Currently defines as:

```
<v-btn dark class="btn--dark-flat-focused jbtn-file">
```

&copy; 2018 Janne Hämäläinen.
 
## License 
Released under [MIT](https://opensource.org/licenses/MIT) license.