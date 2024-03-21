<script>
    export default{}
</script>

<template>
    <footer>
        <section class="container d-flex">
            <div>
                <p>Boolando s.r.l</p>
                <div class="d-flex">
                    <span>Informazioni legali</span>
                    <span>Normativa sulla privacy</span>
                    <span>Diritto di recesso</span>
                </div>
            </div>
            <div class="social">
                <p>Trovaci anche su</p>
                <a href="#"><i class="fa-brands fa-square-x-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-square-facebook"></i></a>
                <a href="#"><i class="fa-brands fa-square-instagram"></i></a>
                <a href="#"><i class="fa-brands fa-square-pinterest"></i></a>
                <a href="#"><i class="fa-brands fa-square-youtube"></i></a>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;
@use '../assets/scss/partials/utils' as *;

    footer{
        background: $bg-footer;
        color: white;
        padding: 20px 0;
        p{
            font-size: 1.4rem;
            font-weight: 600;
        }
        i{
            font-size: 1.5rem;
            border-radius: 5px;
            margin-left: 7px;
        }
        .container{
            justify-content: space-between;
            span{
                font-size: .8rem;
                &:hover{
                cursor: pointer;
                text-decoration: underline;
                }
            }
            
            div.d-flex{
                justify-content: space-between;
                width: 350px;
                font-size: .7rem;
            }
            .social{
                text-align: center;
                a{
                    color: white;
                }
                p{
                    font-size: .9rem;
                    margin-bottom: 5px;
                }
            }
        }
    }
</style>
