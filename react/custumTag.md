# CustomTagComponent

任意のタグで出力できるコンポーネント作りましょうの話
refが取れなかった

多分、tagで入ってきた文字列を `tag as React.ElementType` にして取る

```typescript
import { useEffect, useRef, ComponentPropsWithRef, ElementType } from "react"

type Props<T extends ElementType> = {
    tag?: T;
} & Omit<ComponentPropsWithRef<T>, 'tag'>;

export default function CustomTagComponent<T extends ElementType = 'div'>({ tag, ...props }: Props<T>) {
	const Tag = tag as React.ElementType || 'div';
	const $EL = useRef<HTMLElement>(null!)

	return (
        <Tag ref={$G} {...props}>{props.children}</Tag>
    )
}
```

納得できていない気がする

## Link
- https://zenn.dev/sho_ts/articles/ff3082b1e3db5f
- https://zenn.dev/andynuma/articles/c7f6d6587c116d