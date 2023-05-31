<script>
    import Item_1 from './Item_1.vue';
    import ClientLogo_1 from './ClientLogo_1.vue';

    export default {
        components: {Item_1,ClientLogo_1},
        data() {
            return {
                list:{
                    items: [
                        {
                            "id": "0",
                            "name": "HOME",
                        },
                        {
                            "id": "1",
                            "name": "ABOUT",
                        },
                        {
                            "id": "2",
                            "name": "SERVICES",
                        },
                        {
                            "id": "3",
                            "name": "PACKAGES",
                        },
                        {
                            "id": "4",
                            "name": "INSIGHT",
                        },
                    ],
                    clients: [
                        {
                            "id": "0",
                            "img": "../../public/img/client-logo-7.png",
                        },
                        {
                            "id": "1",
                            "img": "../../public/img/client-logo-8.png",
                        },
                        {
                            "id": "2",
                            "img": "../../public/img/client-logo-9.png",
                        },
                        {
                            "id": "3",
                            "img": "../../public/img/client-logo-5.png",
                        },
                        {
                            "id": "4",
                            "img": "../../public/img/client-logo-6.png",
                        },
                        {
                            "id": "5",
                            "img": "../../public/img/client-logo-7.png",
                        },
                    ]
                }
            }
        }
    };

</script>

<template>
    <div class="contain">
        <div class="logo">
            <img src="../../public/img/finance_logo_1x.png" alt="">
        </div>

        <div class="info">
            <ul>
                <li v-for="item in list.items" :key="item.id">
                    <Item_1 :name="item.name"/>

                    

                </li>
            </ul>

            <div class="buttons">
                <button class="g-btn">CONTACT</button>
                <button class="plus">+</button>
            </div>

        </div>
    </div>

    <div class="jumbo">
        <h1>Right People<span class="g-dot">.</span>Right Investments<span class="g-dot">.</span></h1>
    </div>

    <!-- <div class="clients">
        <ul>
            <li v-for="client in list.clients" :key="client.id">
                <ClientLogo_1 :img="client.img"/>
                 
            </li>
        </ul>
    </div> -->
                 
                             
                    


</template>

<style lang="scss">
    .contain{
        height: 70px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .logo{
            margin-left: 40px;
        }

        .info{
            display: flex;
            margin-right: 40px;

            ul{
                display: flex;
            }

            li{
                list-style: none;
                padding: .5rem;
            }

            .buttons{
                display: flex;

                .plus{
                    border: none;
                    background-color: white;
                    width: 40px;
                    font-size: medium;
                }
            }
        }
    }


    .jumbo{
        width: auto;
        height: 700px;
        background-image: url(../../public/img/home_finance_slider_bg.jpg);
        background-size: contain;

        h1{
            color: white;
            font-size: 50px;
            text-align: center;
            padding: 350px 0px;
        }


        .g-dot{
            color: #5ADDCD;
        }

      
    }


    .clients{
        background-color: #EBEBEB;

        ul{
            display: flex;
        }   

        li{
            list-style: none;
            width: calc(100% / 6); 
            max-width: 50px; 
            
            
        
            img{
                max-width: 100%; 
                height: auto;
            }

        
        
        }


    }

</style>
