<script>
import StartTalkVue from './StartTalk.vue';
import InfoSocial from './Info&Social.vue';

export default {
    components: {StartTalkVue, InfoSocial},
    data() {
        return {
            list:{
                posts:[
                    {
                        "id": "0",
                        "question": "When is it the right time to sell your company?"
                    },
                    {
                        "id": "1",
                        "question": "Personal debt or company debt we explore your options"
                    },
                    {
                        "id": "2",
                        "question": "An interview with a so-called business angel"
                    },
                ],
                services:[
                    {
                        "id": "0",
                        "question": "SMALL BUSINESS LOAN SERVICES"
                    },
                    {
                        "id": "1",
                        "question": "CREDIT RATING ADVICE SERVICES"
                    },
                    {
                        "id": "2",
                        "question": "CROWD FUNDING SERVICES"
                    },
                ],  
            }
        }
    }
}
</script>

<template>
    <StartTalkVue></StartTalkVue>
    <InfoSocial></InfoSocial>
</template>

<style scoped>

</style>
