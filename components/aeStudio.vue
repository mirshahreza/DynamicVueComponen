<template>
    <div>
        append studio header
    </div>
    <table style="width:100%;">
        <tr>
            <td style="width:50%">
                <ae-nav></ae-nav>
            </td>
            <td style="width:50%">
                <ae-docsview></ae-docsview>
            </td>
        </tr>
    </table>
</template>

<script>
    app.component('ae-nav', loadVM("/components/aeNav.vue"));
    app.component('ae-docsview', loadVM("/components/aeDocsview.vue"));    
</script>
