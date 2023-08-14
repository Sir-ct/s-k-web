<script>
    import { Link } from "svelte-routing";
    import Icon from "@iconify/svelte";

    export let link
    export let active
</script>

<main>
    <Link to={link}>
        <div class={`flex ${active ? 'text-white bg-[#111111] ' : 'text-[#DDDDDD]'} hover:text-white hover:bg-[#111111] border-[#222222] border-b-2 items-center p-2 `}>
            <slot />
        </div>
    </Link>
</main>