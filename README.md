# WebSocket signaling server for [y-webrtc](https://github.com/yjs/y-webrtc)
A WebSocket signaling server for [y-webrtc](https://github.com/yjs/y-webrtc) peers.

## About
This WebSocket signaling server listens for messages sent by y-webrtc implementations responding to `subscribe`, `unsubscribe`, `publish`, and `ping` messages from peers.

## Getting Started
To get a local copy up and running follow these simple steps.

### Installation

1. Clone repository
```sh
git clone git@github.com:roymckenzie/y-webrtc-signaling.git
```

2. Install NPM packages
```sh
cd y-webrtc-signaling
npm install
```

## Usage
```sh
npm run dev
```

### Client code
```js
const provider = new WebrtcProvider('your-room-name', ydoc, {
  //...
  signaling: [
    'ws://localhost:8787'
  ]
});
```

## Deployment
You can deploy this code on:

### Heroku
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/roymckenzie/y-webrtc-signaling)

### Render
[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/roymckenzie/y-webrtc-signaling)

## Roadmap
- [ ] Make easily deployable to cloud services

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
y-webrtc-signaling is licensed under the [MIT License](./LICENSE).

Roy McKenzie - [roy@roymckenzie.me](mailto:roy@roymckenzie.me)