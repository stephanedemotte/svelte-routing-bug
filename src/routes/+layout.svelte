<script>
const {children} = $props()
import { onNavigate } from '$app/navigation'
onNavigate(() => new Promise((r) => setTimeout(r, 5000)))
</script>

<nav><a href="/">home</a> <a href="/about">about</a></nav>

{@render children()}
