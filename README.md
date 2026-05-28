# Lab8-Starter

## How are graceful degradation and service workers related?

Graceful degradation is the principle that a web application should continue to provide a usable experience even when certain features or resources are unavailable, such as when the user loses network connectivity or is using an older browser. Service workers support this principle directly: they sit between the page and the network and can intercept fetch requests, serving cached responses when the network fails. This means that a site backed by a service worker can still load pages, display content, and respond to user actions offline, degrading from a full online experience to a still-functional offline one rather than breaking entirely. In browsers that do not support service workers, registration simply fails silently and the app falls back to standard network behavior, which is itself a form of graceful degradation.
