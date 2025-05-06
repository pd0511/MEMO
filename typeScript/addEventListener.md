# addEventListener() / removeEventListener()

## 今時
```typescript
const ABORT = new AbortController();
addEventListener(EVENT_NAME, FUNCTION, {
	signal: ABORT.signal,
});

ABORT.abort();
```
`AbortController.abort()` を呼ぶと`AddEventListenerOptions.signal` で登録された　`AbortController.signal`と一致するイベントが削除される


## 古いらしい
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