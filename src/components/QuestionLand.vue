
<template>
    <div class="questions-land mt-5 mb-5">
        <div class="container">
            <div class="main-head mb-4 ">
                Frequently Asked Questions
            </div>
            <div class="row">
                <div class="col-lg-6 col-md-12 col-sm-12">
                    <div class="questions mb-5">
                        <div class="box-question">
                        <h3 class="text-capitalize">{{questions.q1.ask}}</h3>
                        <div class="plus" @click="questions.q1.open=!questions.q1.open">{{questions.q1.open==false ?"+":"-"}}</div>
                        </div>
                        <div class="box-answer " v-show="questions.q1.open==true">
                            <p class="text-black-50">{{questions.q1.answer}}</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6 col-md-12 col-sm-12">
                    <div class="questions mb-5">
                        <div class="box-question">
                        <h3 class="text-capitalize">{{questions.q2.ask}}</h3>
                        <div class="plus" @click="questions.q2.open=!questions.q2.open">{{questions.q2.open==false ?"+":"-"}}</div>
                        </div>
                        <div class="box-answer " v-show="questions.q2.open==true">
                            <p class="text-black-50">{{questions.q2.answer}}</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6 col-md-12 col-sm-12">
                    <div class="questions mb-5">
                        <div class="box-question">
                        <h3 class="text-capitalize">{{questions.q3.ask}}</h3>
                        <div class="plus" @click="questions.q3.open=!questions.q3.open">{{questions.q3.open==false ?"+":"-"}}</div>
                        </div>
                        <div class="box-answer " v-show="questions.q3.open==true">
                            <p class="text-black-50">{{questions.q3.answer}}</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6 col-md-12 col-sm-12">
                    <div class="questions mb-5">
                        <div class="box-question">
                        <h3 class="text-capitalize">{{questions.q4.ask}}</h3>
                        <div class="plus" @click="questions.q4.open=!questions.q4.open">{{questions.q4.open==false ?"+":"-"}}</div>
                        </div>
                        <div class="box-answer " v-show="questions.q4.open==true">
                            <p class="text-black-50">{{questions.q4.answer}}</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6 col-md-12 col-sm-12">
                    <div class="questions mb-5">
                        <div class="box-question">
                        <h3 class="text-capitalize">{{questions.q5.ask}}</h3>
                        <div class="plus" @click="questions.q5.open=!questions.q5.open">{{questions.q5.open==false ?"+":"-"}}</div>
                        </div>
                        <div class="box-answer " v-show="questions.q5.open==true">
                            <p class="text-black-50">{{questions.q5.answer}}</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-6 col-md-12 col-sm-12">
                    <div class="questions mb-5">
                        <div class="box-question">
                        <h3 class="text-capitalize">{{questions.q6.ask}}</h3>
                        <div class="plus" @click="questions.q6.open=!questions.q6.open">{{questions.q6.open==false ?"+":"-"}}</div>
                        </div>
                        <div class="box-answer " v-show="questions.q6.open==true">
                            <p class="text-black-50">{{questions.q6.answer}}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
    let questions={
            "q1":{
                open:false,
                
                ask:"How To Contact For Help?",
                answer:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus, eligendi, facere dolorum tempora fuga voluptatibus officiis minus eveniet explicabo aperiam exercitationem neque sed quis odio similique reprehenderit harum sit excepturi!",
                
            },
            "q2":{
                open:false,
                
                ask:"What Is The Best Career In 2022?",
                answer:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus, eligendi, facere dolorum tempora fuga voluptatibus officiis minus eveniet explicabo aperiam exercitationem neque sed quis odio similique reprehenderit harum sit excepturi!"

            },
            "q3":{
                open:false,
                
                ask:"How Much Fees For Web Development?",
                answer:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus, eligendi, facere dolorum tempora fuga voluptatibus officiis minus eveniet explicabo aperiam exercitationem neque sed quis odio similique reprehenderit harum sit excepturi!"

            },
            "q4":{
                open:false,
                
                ask:"Can I Choose My Own Tutor?",
                answer:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus, eligendi, facere dolorum tempora fuga voluptatibus officiis minus eveniet explicabo aperiam exercitationem neque sed quis odio similique reprehenderit harum sit excepturi!"

            },
            "q5":{
                open:false,
                
                ask:"What Payment Methods Are Availabe?",
                answer:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus, eligendi, facere dolorum tempora fuga voluptatibus officiis minus eveniet explicabo aperiam exercitationem neque sed quis odio similique reprehenderit harum sit excepturi!"

            },
            "q6":{
                open:false,
                
                ask:"Can I Have Free Trial For A Month?",
                answer:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus, eligendi, facere dolorum tempora fuga voluptatibus officiis minus eveniet explicabo aperiam exercitationem neque sed quis odio similique reprehenderit harum sit excepturi!"

            },
            
        };
export default {
    name:"QuestionLand",
    el:".questions-land",
    data:function() {
    return {
        questions:questions,
        
        convert: function() {
        this.open=!this.open;
        if(this.open){
            this.plus="-"
        }
        else 
        this.plus="+"
    }
    };
}
    
  
  
}
</script>
<style lang="scss">
    .box-question{
        background-color: var(--green-color);
        padding: 3px 15px;
        margin: 0 5% ;
        width: 90%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        color: white;
        h3{
            font-size: 1.3em;
        }
        .plus{
            cursor: pointer;
            font-size: 1.8em;
        }
    }
    .box-answer{
        background-color: #f0fdfa;
        padding: 3px 15px;
        margin: 0 5% ;
        width: 90%;
        text-align: left;
        line-height: 2;
        
    }
    @media (max-width:530px) {
        .box-answer h3,.box-question h3{
            font-size:14px;
        }
        
    }
</style>