<template>
    <button @click="show('this is a message')">Click to add Component here</button>
    <div id="comPlace">A place for new component</div>
</template>

<script>    
    export default {
        setup(props) {
            return {
                show: (msg) => {

                    console.log(msg);
                    let cPlace = document.getElementById("comPlace");
                    app.component('ae-test', loadVM("/components/aeTest.vue"));
                    cPlace.innerHTML='<ae-test>qqqqqqqqqqqqqqqqqqq</ae-test>';
                }
            };
        }
    }
</script>
