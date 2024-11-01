# addEventListener() / removeEventListener()

多分こう

```typescript
const OPRTION:(boolean | AddEventListenerOptions | EventListenerOptions) = {passive: true};
addEventListener(EVENT_NAME, FUNCTION, OPRTION);

removeEventListener(EVENT_NAME, FUNCTION, OPRTION);
```

後で理解する

### Link
https://github.com/microsoft/TypeScript/issues/32912

https://dom.spec.whatwg.org/#dom-eventtarget-removeeventlistener

https://dom.spec.whatwg.org/#dictdef-eventlisteneroptions