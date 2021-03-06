---
items:
  - src: http://via.placeholder.com/600x400
    thumbnail: http://via.placeholder.com/64x64
    w: 600
    h: 400
    alt: 'optional alt attribute for thumbnail image'
  - src: http://via.placeholder.com/1200x900
    thumbnail: http://via.placeholder.com/64x64
    w: 1200
    h: 900
  - src: http://via.placeholder.com/800x600
    thumbnail: http://via.placeholder.com/64x64
    w: 800
    h: 600
---

### Curved Thumbnails

We wrote a custom Vue wrapper for the `Photo Swipe` library so it makes it easy
for you to create image galleries seamlessly. Thumbnails border radius is
configurable. Pass a value of `5` to the `thumbnailRadius` to show curved
borders.

<!--code-->

```vue
<script setup lang="ts">
const items = [
  {
    src: 'http://via.placeholder.com/600x400',
    thumbnail: 'http://via.placeholder.com/64x64',
    w: 600,
    h: 400,
    alt: 'optional alt attribute for thumbnail image',
  },
  {
    src: 'http://via.placeholder.com/1200x900',
    thumbnail: 'http://via.placeholder.com/64x64',
    w: 1200,
    h: 900,
  },
  {
    src: 'http://via.placeholder.com/800x600',
    thumbnail: 'http://via.placeholder.com/64x64',
    w: 800,
    h: 600,
  },
]
</script>

<template>
  <V-PhotosSwipe :items="items" thumbnail-radius="5" />
</template>
```

<!--/code-->

<!--example-->

<V-PhotosSwipe :items="frontmatter.items" thumbnailRadius="5" />

<!--/example-->
