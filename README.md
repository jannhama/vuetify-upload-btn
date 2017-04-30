# vuetify-upload-btn
Simple component to handle file selection for upload.

## Installation

Copy ```UploadButton.vue``` to part of our project and require/import if using bundler.

Tested only to work with Vue2 and Vuetify 0.11.1

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

If you want to modify styles do it in the component file directly. Currently defines as:

```
<v-btn dark class="btn--dark-flat-focused jbtn-file">
```

&copy; 2016 Janne Hämäläinen.
 
## License 
Released under [MIT](https://opensource.org/licenses/MIT) license.