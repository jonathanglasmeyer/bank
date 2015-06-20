### note: right now this is experimental and not usable for other persons, as you need a client secret for api access.

# bank

a banking cli that uses the figo api.


### get a session id from figo
- run `node build/server.js`
- open `localhost:3000/page`
- login to figo, supply the rights you want to give
- upon connecting you will see the session-id as a `res.write` output
- save the string into `configuration/constants.js` under `SESSION_ID`
- optional: get a new session id by `localhost:3000/logout` and repeating the steps


### run dev
- rebuild on file changes: `webpack -w`
- reexecute on build changes: `f=build/server.js; while watch $f; do node $f; done`


