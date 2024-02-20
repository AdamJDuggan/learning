## CORS
A JavaScript application running in the browser can usually only access HTTP resources on the same domain (origin) that serves it.

Loading images or scripts/styles always works, but XHR and Fetch calls to another server will fail, unless that server implements a way to allow that connection.

## PREFLIGHT
There are some requests that are handled in a “simple” way. All GET requests belong to this group.

Also some POST and HEAD requests do as well.
ll other requests must run through a pre-approval phase, called preflight. The browser does this to determine if it has the permission to perform an action, by issuing an OPTIONS request.

A preflight request contains a few headers that the server will use to check permissions.
