Resizes the window to the specified dimensions

# Example
```js
async function createWin() {
    const app = await fin.Application.start({
        name: 'myApp',
        uuid: 'app-1',
        url: 'https://cdn.openfin.co/docs/javascript/stable/tutorial-Window.resizeTo.html',
        autoShow: true
    });
    return await app.getWindow();
}

async function resizeTo(left, top, anchor) {
    const app = await createWin();
    return await app.resizeTo(left, top, );
}

resizeTo(580, 300, 'top-left').then(() => console.log('Resized')).catch(err => console.log(err));
```
