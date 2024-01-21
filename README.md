# useCont

> One hook to rule them all,  
>   one hook to find them,  
> One hook to bring them all  
>   and in the darkness transform them.

This is a parady custom React hook.

## Usage

```typescript
import { useCont } from '@caasi/use-cont'

function App() {
  const sayHello = useCallback(
    (f: (x: string) => void) => { setTimeout(f, 5000, ':D') },
    []
  )
  const [hello, error] = useCont(sayHello, '')

  return (
    // your app here
  )
}

```

