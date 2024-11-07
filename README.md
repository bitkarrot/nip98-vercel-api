# NIP98-Vercel-api sample

## Usage notes

use `vercel dev` to run locally

deployed to vercel as https://nip98-vercel-api.vercel.app/

## API endpoint

### Test GET endpoint:
`curl -X GET https://nip98-vercel-api.vercel.app/api`


### Test POST endpoint:
`curl -X POST https://nip98-vercel-api.vercel.app/api/two`


### NIP98 POST Auth endpoint: 
requires Authorization header with nostr (in place of bearer)
and a body with `room`, `username`, `avatarURL`, `relays`, `isPresenter`

`curl -X POST https://nip98-vercel-api.vercel.app/api/auth -H "Authorization: Nostr <base64 encoded event>" -d '{"room": "test", "username": "test", "avatarURL": "test", "relays": [ "wss://relay.damus.io" ], "isPresenter": true}'`



