# Atomic Gallery

Atomic Video/Image Gallery based on https://github.com/blueimp/Gallery.


## Setup

Include .css:
```scss
@import "atomic-gallery/atomic-gallery";
```

Include .js:
```js
//=include atomic-gallery/atomic-gallery.js
```

Include assets (example via gulp):
```js
function copy_gallery_assets() {
  return gulp.src(`${paths.modules}/blueimp-gallery/img/**/*`)
    .pipe(gulp.dest(`${paths.static}/img`));
}
// ...
const compile = gulp.series(
  gulp.parallel(
    copy_gallery_assets
  )
);
```
