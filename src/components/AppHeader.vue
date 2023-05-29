<script>
import Item_1 from './Item_1.vue';

export default {
    components: {Item_1},
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


</template>

<style lang="scss" scoped>
    .contain{
        max-width: 1400px;
        margin-inline: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .info{
            display: flex;

            ul{
                display: flex;
            }

            li{
                list-style: none;
                padding: .5rem;
            }

            .buttons{
                display: flex;

                .g-btn{
                    border: none;
                    background-color: #5ADDCD;
                    padding: 0px 20px;
                    margin: 15px;
                    border-radius: 50px;
                    cursor: pointer;
                }

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
        width: 100%;
        height: 400px;
        color: white;
        background-image: url(../../public/img/home_finance_slider_bg.jpg);


      
    }

</style>
