<script>
	import '../app.postcss';
    import { supabase } from "../supabase"
    console.log(supabase)
</script>

<div class="container mx-auto my-6 max-w-lg">
	<slot />
</div>
