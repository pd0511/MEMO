# setTimeout
`window.setTimeout` にしないと Node.js のものを参照してしまう

```typescript
let timer:(number | null) = null;

timer = window.setTimeout(() => {}, 100);

clearTimeout(timer);
```