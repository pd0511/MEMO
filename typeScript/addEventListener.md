# addEventListener() / removeEventListener()

多分こう

```typescript
const OPRTION:(boolean | AddEventListenerOptions | EventListenerOptions) = {passive: true};
addEventListener(EVENT_NAME, FUNCTION, OPRTION);

removeEventListener(EVENT_NAME, FUNCTION, OPRTION);
```

## Link
- https://github.com/microsoft/TypeScript/issues/32912
- https://dom.spec.whatwg.org/#dom-eventtarget-removeeventlistener
- https://dom.spec.whatwg.org/#dictdef-eventlisteneroptions