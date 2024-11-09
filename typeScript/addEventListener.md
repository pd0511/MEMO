# addEventListener() / removeEventListener()

多分こう

```typescript
const OPTIONS:(boolean | AddEventListenerOptions | EventListenerOptions) = {passive: true};
addEventListener(EVENT_NAME, FUNCTION, OPTIONS);

removeEventListener(EVENT_NAME, FUNCTION, OPTIONS);
```

## Link
- https://github.com/microsoft/TypeScript/issues/32912
- https://dom.spec.whatwg.org/#dom-eventtarget-removeeventlistener
- https://dom.spec.whatwg.org/#dictdef-eventlisteneroptions