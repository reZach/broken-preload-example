# broken-preload-example
This is a MVP explaining what is broken with the preload functionality. There is a problem where the ipcRenderer does not have access to [.on](https://electronjs.org/docs/api/ipc-renderer#ipcrendereronchannel-listener) in a renderer process. You can find more discussion on the [github issue](https://github.com/electron/electron/issues/21437).

## To run
```
git clone https://github.com/reZach/broken-preload-example
cd broken-preload-example
npm i
npm run start
```

## Output
The ipcRenderer _should_ be allowed to add an event with the .on method in the renderer process.
[![Console logs of the ipcRenderer](img/snippet.png)]()