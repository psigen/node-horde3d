node-horde3d
============

Node.js bindings to Horde3D through [node-ffi].

These bindings are automatically generated via [node-ffi-generate] from the Horde3D API header file (`Bullet-C-Api.h`).  They have a 1:1 mapping with the existing Horde3D API documentation.

  * [Documentation for the Horde3D API]

Installing this library via NPM
-------------------------------
Currently, this library is not published to `npm`.  However, you can use it in npm projects by adding it to your `package.json` using a git url:

```javascript
"dependencies": { 
  "bulletphysics": "git://github.com/psigen/node-horde3d.git"
}
```

Example Usage
-------------
```javascript
var h3d = require('horde3d').horde3d;
var sdk = h3d.Horde3DInit;
...
console.log('Doing Horde3D stuff...');
...
h3d.DeleteSdk(sdk);
```

Compilation notes
-----------------
  * Nothing weird just yet.

<!-- Link references -->
[node-ffi]: https://github.com/rbranson/node-ffi
[node-ffi-generate]: https://github.com/tjfontaine/node-ffi-generate
[Documentation for the Horde3D API]: http://horde3d.org/docs/manual.html

