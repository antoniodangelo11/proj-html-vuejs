<script></script>

<template>
    <section class="bg_copy">
        <div class="container">
            <div class="row justify-content-between">
                <div class="col-8">
                    <div class="copyright">
                        <i class="fa-regular fa-copyright px-2"></i>
                        <span>Copyright 2012 - 2020 | Avada Theme by <a href="">ThemeFusion</a> | All Rights Reserved |
                            Powered by <a href="">Wordpress</a></span>
                    </div>
                </div>
                <div class="col-4">
                    <div class="socials_icons text-light">
                        <i class="fa-brands fa-facebook px-2"></i>
                        <i class="fa-brands fa-twitter px-2"></i>
                        <i class="fa-brands fa-youtube px-2"></i>
                        <i class="fa-brands fa-instagram px-2"></i>
                    </div>
                </div>
            </div>
            <div class="chevron_fixed">
                <a href="#start"><i class="fa-solid fa-chevron-up fa-xs"></i></a>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
.bg_copy {
    background-color: rgb(28, 29, 30);
    height: 10rem;
}

.container {
    max-width: 1000px;
    padding-top: 4rem;
    padding-bottom: 3rem;
}

.copyright {

    i {
        color: #929aa3;
    }

    span {
        color: #929aa3;
        font-size: .8em;
        white-space: nowrap;

        a {
            text-decoration: none;
            color: #7ABC64;
        }
    }
}

.socials_icons {
    padding-left: 6rem;
}

.chevron_fixed {
    background-color: #494C4E;
    padding: .2rem 1rem;
    position: fixed;
    bottom: 0%;
    right: 5%;
    border-radius: 5px 5px 0px 0px;

    a {
        color: rgb(255, 255, 255)
    }
}
</style>