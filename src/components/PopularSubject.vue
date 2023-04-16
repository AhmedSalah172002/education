<template>
    <div class="popular-subjects mt-5 mb-5">
        <div class="container">
            <div class="main-head text-capitalize mb-5">
                our popular subjects
            </div>
            <div class="row">
                <div class="col-lg-2 col-md-4 col-sm-6">
                    <div class="subject-cont">
                        <img src="../assets/subject-icon-1.png" class="img-fluid" alt="">
                        <h3>graphic design</h3>
                        <p>12 modules</p>
                    </div>
                </div>
                <div class="col-lg-2 col-md-4 col-sm-6">
                    <div class="subject-cont">
                        <img src="../assets/subject-icon-2.png" class="img-fluid" alt="">
                        <h3>mathemetics</h3>
                        <p>12 modules</p>
                    </div>
                </div>
                <div class="col-lg-2 col-md-4 col-sm-6">
                    <div class="subject-cont">
                        <img src="../assets/subject-icon-3.png" class="img-fluid" alt="">
                        <h3>teaching</h3>
                        <p>12 modules</p>
                    </div>
                </div>
                <div class="col-lg-2 col-md-4 col-sm-6">
                    <div class="subject-cont">
                        <img src="../assets/subject-icon-4.png" class="img-fluid" alt="">
                        <h3>development</h3>
                        <p>12 modules</p>
                    </div>
                </div>
                <div class="col-lg-2 col-md-4 col-sm-6">
                    <div class="subject-cont">
                        <img src="../assets/subject-icon-5.png" class="img-fluid" alt="">
                        <h3>science</h3>
                        <p>12 modules</p>
                    </div>
                </div>
                <div class="col-lg-2 col-md-4 col-sm-6">
                    <div class="subject-cont">
                        <img src="../assets/subject-icon-6.png" class="img-fluid" alt="">
                        <h3>engineering</h3>
                        <p>12 modules</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name:"PopularSubject"
}
</script>

<style lang="scss">
.main-head{
    font-size: 2.5em;
}
    .subject-cont{
        height: 222px;
        border-radius: 10px;
        border:1px solid var(--green-color);
        padding:20px 15px;
        margin-bottom: 15px;
        cursor: pointer;
        transition: .3s;
        h3{
            font-size: 1.2em;
            width: 100%;
            margin: 10px 0;
            text-transform: capitalize;
        }
        &:hover{
            background-color: var(--green-color);
            color: white !important;
            
        }
    }
</style>