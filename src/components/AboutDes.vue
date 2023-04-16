<template>
    <div class="about-des mt-5 mb-5">
        <div class="container">
            <div class="row">
                <div class="col-lg-6">
                <div class="about-image">
                    <img src="../assets/about-img.jpg" alt="" class="img-fluid">
                </div>
            </div>
            <div class="col-lg-6">
                <div class="about-cont mt-5">
                    <h3 class="text-capitalize">we have best courses for you</h3>
                    <p class="text-black-50">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam hic magnam fugit exercitationem neque, quae laboriosam natus. Ut maxime assumenda facere ea quasi accusamus dolores delectus tempora animi, expedita iste.</p>
                    <div class="row">
                        <div class="col-lg-4">
                            <div class="cont-image">
                                <img src="../assets/about-icon-1.png" alt="">
                                <h3 class="mt-4 mb-4">350+</h3>
                                <span>courses</span>
                            </div>
                        </div>
                        <div class="col-lg-4">
                            <div class="cont-image">
                                <img src="../assets/about-icon-2.png" alt="">
                                <h3 class="mt-4 mb-4">1200+</h3>
                                <span>students</span>
                            </div>
                        </div>
                        <div class="col-lg-4">
                            <div class="cont-image">
                                <img src="../assets/about-icon-3.png" alt="">
                                <h3 class="mt-4 mb-4">10+</h3>
                                <span>awards</span>
                            </div>
                        </div>
                    </div>
                    
                </div>
            </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:"AboutDes"
}
</script>

<style lang="scss">
    .about-des{

        .cont-image{
            margin: 0 0 15px;
            padding: 15px 20px;
            text-align: center;
            border: 1px solid var(--green-color);
            background-color: #f0fdfa;
            span{
                color:#777;
            }
        }
    }
</style>