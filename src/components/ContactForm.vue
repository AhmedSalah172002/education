<template>
    <div class="contact-form mt-3 mb-5">
        <div class="container">
            <div class="row">
                <div class="col-lg-6">
                    <div class="contact-image">
                        <img src="../assets/contact-img.png" alt="" class="img-fluid">
                    </div>
                </div>
                <div class="col-lg-6">
                    <form action="">
                        <h3>send us a message</h3>
                        <input type="text" placeholder="name" class="box">
                        <input type="email" placeholder="email" class="box">
                        <input type="number" placeholder="phone" class="box">
                        <textarea name="" class="box" placeholder="message" id="" cols="30" rows="10"></textarea>
                        <input type="submit" value="send message" class="btn1">
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:"ContactForm"
}
</script>

<style lang="scss">
    .contact-form{
        form{
            display: block;
            border: 2px solid var(--green-color);
            padding: 15px 20px;
            text-align: left;
            h3{
                text-transform: capitalize;
                margin-bottom: 15px;
            }
            .box{
                width: 100%;
                margin-bottom: 10px;
                padding: 7px 10px;
                border: 2px solid var(--green-color);
                font-size: .95em;
                transition: .3s;
                &:focus{
               background: var(--green-color);
               color:white;
               outline: none;

               &::placeholder{
                  color:#f0fdfa;
               }
            }
            }
            textarea{
            
            resize: none;
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
        }

    }
</style>