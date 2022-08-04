<script>
    import { onMount } from "svelte";
    onMount(() => {
        import('@alan-ai/alan-sdk-web').then(({ default: alanBtn }) => {
            const alanBtnInstance = alanBtn({
                key: 'ENTER_YOUR_API_KEY_HERE',
                onCommand: (data) => {
                    console.log(data);
                },
                rootEl: document.getElementById('alan-btn')
            });
        }).catch((err) => {
            console.log(err);
        });
    });
</script>

<div class="alan-btn"></div>