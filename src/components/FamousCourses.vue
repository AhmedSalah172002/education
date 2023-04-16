<template>
    <div class="famous-courses mt-5 mb-5">
        <div class="container">
            <div class="row">
                <div class="col-lg-4 col-md-6 col-sm-12">
                    <div class="course mb-5">
                        <div class="student-image">
                            <img src="../assets/course-2-1.jpg" alt="" class="img-fluid">
                            <h3 class="text-capitalize">development</h3>
                        </div>
                        <div class="course-cont mt-4">
                            <h3>choose what's best for you!</h3>
                            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eaque, odit!</p>
                            <a href="#" class="btn1">read more</a>
                        </div>
                        <div class="container">
                            <div class="course-add d-flex justify-content-between">
                                <p> <fontAwesome icon="book" /> 12 Modules</p>
                                <p> <fontAwesome icon="clock" /> 6 Hours</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6 col-sm-12">
                    <div class="course mb-5">
                        <div class="student-image">
                            <img src="../assets/course-2-2.jpg" alt="" class="img-fluid">
                            <h3 class="text-capitalize">Engineering</h3>
                        </div>
                        <div class="course-cont mt-4">
                            <h3>choose what's best for you!</h3>
                            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eaque, odit!</p>
                            <a href="#" class="btn1">read more</a>
                        </div>
                        <div class="container">
                            <div class="course-add d-flex justify-content-between">
                                <p> <fontAwesome icon="book" /> 12 Modules</p>
                                <p> <fontAwesome icon="clock" /> 6 Hours</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6 col-sm-12">
                    <div class="course mb-5">
                        <div class="student-image">
                            <img src="../assets/course-2-3.jpg" alt="" class="img-fluid">
                            <h3 class="text-capitalize">Mathemetics</h3>
                        </div>
                        <div class="course-cont mt-4">
                            <h3>choose what's best for you!</h3>
                            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eaque, odit!</p>
                            <a href="#" class="btn1">read more</a>
                        </div>
                        <div class="container">
                            <div class="course-add d-flex justify-content-between">
                                <p> <fontAwesome icon="book" /> 12 Modules</p>
                                <p> <fontAwesome icon="clock" /> 6 Hours</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6 col-sm-12">
                    <div class="course mb-5">
                        <div class="student-image">
                            <img src="../assets/course-2-4.jpg" alt="" class="img-fluid">
                            <h3 class="text-capitalize">Doctor</h3>
                        </div>
                        <div class="course-cont mt-4">
                            <h3>choose what's best for you!</h3>
                            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eaque, odit!</p>
                            <a href="#" class="btn1">read more</a>
                        </div>
                        <div class="container">
                            <div class="course-add d-flex justify-content-between">
                                <p> <fontAwesome icon="book" /> 12 Modules</p>
                                <p> <fontAwesome icon="clock" /> 6 Hours</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6 col-sm-12">
                    <div class="course mb-5">
                        <div class="student-image">
                            <img src="../assets/course-2-5.jpg" alt="" class="img-fluid">
                            <h3 class="text-capitalize">Science</h3>
                        </div>
                        <div class="course-cont mt-4">
                            <h3>choose what's best for you!</h3>
                            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eaque, odit!</p>
                            <a href="#" class="btn1">read more</a>
                        </div>
                        <div class="container">
                            <div class="course-add d-flex justify-content-between">
                                <p> <fontAwesome icon="book" /> 12 Modules</p>
                                <p> <fontAwesome icon="clock" /> 6 Hours</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6 col-sm-12">
                    <div class="course mb-5">
                        <div class="student-image">
                            <img src="../assets/course-2-6.jpg" alt="" class="img-fluid">
                            <h3 class="text-capitalize">Business</h3>
                        </div>
                        <div class="course-cont mt-4">
                            <h3>choose what's best for you!</h3>
                            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eaque, odit!</p>
                            <a href="#" class="btn1">read more</a>
                        </div>
                        <div class="container">
                            <div class="course-add d-flex justify-content-between">
                                <p> <fontAwesome icon="book" /> 12 Modules</p>
                                <p> <fontAwesome icon="clock" /> 6 Hours</p>
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
    name:"FamousCourses"
}
</script>
<style lang="scss">
    .famous-courses{
        .course{
            border: 2px solid var(--green-color) ;
            border-radius: 10px;
            .student-image{
                border-radius: 10px 10px 0 0;
                position: relative;
                overflow: hidden;
                img{
                    border-radius: 10px 10px 0 0;
                    width: 100%;
                    transition: .3s;
                    &:hover{
                        transform: scale(1.1);
                    }
                }
                h3{
                    position: absolute;
                    top: 5%;
                    left: 5%;
                    transform: translate(-5%,-5%);
                    padding: 1px 10px;
                    font-size: 1.2em;
                    width: fit-content;
                    background-color: white;
                }
            }
            p{
                color: #777;
            }
            .btn1{
                display: block;
                margin: auto;
                padding: 3px 10px;
                text-align:center;
                background-color: #f0fdfa;
                color:var(--green-color)!important;
                text-transform: capitalize;
                border: 1px solid var(--green-color);
                width: fit-content;
                font-size: 1.3em;
                transition: .3s;
                &:hover{
                    color:#f0fdfa !important;
                    background-color: var(--green-color) !important;
                }
            
            }
            .course-add{
                margin-top: 15px;
                padding-top: 10px;
                border-top: 2px solid var(--green-color);
                svg{
                    color: var(--green-color);
                }
            }
        }
    }
</style>