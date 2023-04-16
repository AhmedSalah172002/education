<template>
    <div class="touch mt-5 mb-5">
        <div class="container">
            <div class="main-head text-capitalize mb-5">
                get In Touch
            </div>
            <div class="row">
                <div class="col-lg-3 col-md-6 col-sm-12">
                    <div class="touch-cont mb-5">
                        <fontAwesome icon="clock" />
                        <h3 class="text-capitalize mb-3">opening hours :</h3>
                        <p>00:07am to 00:06pm</p>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 col-sm-12">
                    <div class="touch-cont mb-5">
                        <fontAwesome icon="phone" />
                        <h3 class="text-capitalize mb-3">phone :</h3>
                        <p>+123-456-7890</p>
                        <p>+111-222-3333</p>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 col-sm-12">
                    <div class="touch-cont mb-5">
                        <fontAwesome icon="envelope" />
                        <h3 class="text-capitalize mb-3">Email :</h3>
                        <p>shaikhanas@gmail.com</p>
                        <p>anasbhai@gmail.com</p>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 col-sm-12">
                    <div class="touch-cont mb-5">
                        <fontAwesome icon="map" />
                        <h3 class="text-capitalize mb-3">Address :</h3>
                        <p>mumbai, india - 400104</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:"GetTouch"
}
</script>

<style lang="scss">
    .touch{
        .touch-cont{
            height: 250px;
            padding: 15px 25px;
            background-color: #f0fdfa;
            border: 1px solid var(--green-color);
            svg{ 
                display: block;
                margin: 10px auto 20px;
                padding: 20px;
                border-radius: 50%;
                font-size: 2em;
                background-color:var(--green-color)!important;
                color: #f0fdfa;
            }
            p{
                color:#777;
            }
        }
    }
</style>