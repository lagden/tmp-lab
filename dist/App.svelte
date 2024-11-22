<script>
    import {tick} from 'svelte'
    import {Loading, acts as loadingActs} from '@tadashi/svelte-loading'

    tick().then(() => {
        loadingActs.show(true)
        setTimeout(() => {
            loadingActs.show(false)
        }, 1000)
    })
</script>

<Loading animation="ChaoticOrbit" />
<h1>Estamos no app</h1>