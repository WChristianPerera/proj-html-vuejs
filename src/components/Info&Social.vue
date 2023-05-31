<script>
import Footerposts from './Footerposts.vue';
import Footerservices from './Footerservices.vue';

export default {
    components: {Footerposts, Footerservices},
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
    <div class="row footer-top">

        <div class="col-3">
            <img src="../../public/img/finance_logo_footer.png" alt="">
        </div>


        <div class="col-5">
            <div class="row">
                <div class="col">
                    <h4>RECENT POSTS</h4>
                    <ul>
                        <li v-for="post in list.posts" :key="post.id">
                            <Footerposts :question="post.question"/>
                        </li>
                    </ul>
                </div>
                <div class="col">
                    <h4>SERVICES</h4>
                    <ul>
                        <li v-for="service in list.services" :key="service.id">
                            <Footerservices :question="service.question"/>
                        </li>
                    </ul>
                </div>
            </div>
        </div>


        <div class="col-4">
            <h4>LATEST</h4>
            <i class="fa-brands fa-twitter"></i>
        </div>
    </div>

    <div class="footer-bot">
        <div>
            <ul class="last-info">
                <li>Copyright 2012-2020 |</li>
                <li>Avada Theme by Theme Fusion |</li>
                <li>All Rights Reserved |</li>
                <li>Powered by WordPress</li>
            </ul>
        </div>
        <div>
            <ul class="social">
                <li>
                    <div class="icon-bg">
                        <i class="fa-brands fa-facebook"></i>

                    </div>
                </li>
                <li>
                    <div class="icon-bg">
                        <i class="fa-brands fa-twitter"></i>

                    </div>
                </li>
                <li>
                    <div class="icon-bg">
                        <i class="fa-brands fa-youtube"></i>

                    </div>
                </li>
                <li>
                    <div class="icon-bg">
                        <i class="fa-brands fa-instagram"></i>

                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>


<style lang="scss">
    .footer-top{
        background-color: #2D2D2D;
        color: white;
    }   


    li{
        list-style: none;
    }

    .footer-bot{
        background-color: black;
        display: flex;
        justify-content: space-between;

        .last-info, .social{
            display: flex;
            gap: 0.5rem;
            color: #5D5D5E;
        }



        .icon-bg{
            background-color: #5ADDCD;
            width: 30px;
            height: 30px;
            text-align: center;
            border-radius: 50%;
            color: white;

        }
    }
</style>