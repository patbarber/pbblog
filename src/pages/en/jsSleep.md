---
title: Javascript Sleep 
description: How to create a sleep function in javascript
layout: ../../layouts/MainLayout.astro
---

Ever need to test a loading function or just delay calling the next part of a function. Use this simple timeout function to test it out.

```
 async sleep(milliseconds) {
      return new Promise((resolve) => setTimeout(resolve, milliseconds));
    }
```

This function will wait for the timeout to finish before moving on to the next section.

Eg:

```
function previewImage(){
    this.loading = true     // show loading svg
    this.sleep(1000)        // call sleep for 1 second
    this.loading = false    // hide loading svg
}
```

