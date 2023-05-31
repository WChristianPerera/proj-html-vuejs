<script>
    export default {}
</script>

<template>
<!-- Section 1 -->
<div class="container">
    <div class="row based-finance">
        <div class="col-6 description">
            <h2>Cloud Based Finance</h2>
    
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit, sed do tempor incididunt ut labore et dolore magna aliqua.</p>
    
            <p>Laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident.</p>
        
            <button class="g-btn">LEARN MORE</button>
        </div>
    
    
        <div class="col-6 graphic">
            <div class="image-container">
                <img src="../../public/img/graph-600x457.jpg" alt="">
            </div>
        </div>
    </div>
</div>

<!-- section 2 -->

<div class="special-services">
    <div class="container">
        <div class="row">

            <div class="col-12">
                <h2>Specialty Services</h2>
    
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit, sed do tempor incididunt ut labore et dolore magna aliqua. Laboris nisi ut aliquip ex ea commodo consequat.</p>
            </div>



            <div class="col-4 service">
                <div class="content">
                    <i class="fa-solid fa-globe logo"></i>
                    <h3>Small Business Loans</h3>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit, sed do tempor incididunt ut labore et dolore magna aliqua.</p>
                </div>

                <div class="button">Learn More</div> 
                
            </div>

            <div class="col-4 service ">
                <div class="content">
                    <i class="fa-regular fa-gem logo"></i>
                    <h3>Credit Rating Advice</h3>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit, sed do tempor incididunt ut labore et dolore magna aliqua.</p>
                </div>

                <div class="button">Learn More</div>

            </div>

            <div class="col-4 service">
                <div class="content">
                    <i class="fa-solid fa-chart-line logo"></i>
                    <h3>Fast Crowd Funding</h3>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit, sed do tempor incididunt ut labore et dolore magna aliqua.</p>
                </div>
                
                <div class="button">Learn More</div>
                
            </div>

        </div>
    </div>

</div>
</template>

    







<style lang="scss">

    .special-services{
        text-align: center;
        background-color: #EBEBEB;


        .service{
            width: calc(95% / 3);

            .content{
                background-color: white;
                padding: 2rem;
                height: 270px;

                .logo{
                    font-size: 50px;
                    color: #4A75AC;
                }
            }
            .button{
                background-color: #5ADDCD;
                color: white;
            }

        }
    }

</style>
