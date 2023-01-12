<script>

</script>

<template>
    <footer>

        <section class="top-footer">
            <div class="container-lg">
                <div class="row">
                    <div class="col-1">
                        <h6>DC COMICS</h6>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>

                        <h6>SHOP</h6>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>

                    <div class="col-1">
                        <h6>DC</h6>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshop</li>
                            <li>CPSC Certificate</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>

                    <div class="col-1">
                        <h6>SITES</h6>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                </div>
            </div>

        </section>

        <section class="bot-footer">
            <div class="container-lg">
                <div class="row justify-content-between py-3">
                    <div class="col-2">
                        <button class="p-3">SIGN-UP NOW!</button>
                    </div>
                    <div class="col-6 d-flex">
                        <span class="mt-3 me-5">FOLLOW US</span>
                        <img class="p-2" src="../assets/img/footer-facebook.png" alt="">
                        <img class="p-2" src="../assets/img/footer-periscope.png" alt="">
                        <img class="p-2" src="../assets/img/footer-pinterest.png" alt="">
                        <img class="p-2" src="../assets/img/footer-twitter.png" alt="">
                        <img class="p-2" src="../assets/img/footer-youtube.png" alt="">
                    </div>
                </div>
            </div>
        </section>

    </footer>
</template>

<style lang="scss">
@use "../styles/partials/variables" as *;

footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    section.top-footer {
        color: white;
        font-size: .7rem;

        h6 {
            margin-top: 3rem;
            margin-bottom: 2rem;
        }

        ul {
            padding-left: 0rem;
            margin-bottom: 2rem;

            li {
                color: #8f8f8f;
                width: max-content;
            }
        }
    }

    section.bot-footer {
        background-color: #303030;

        button {
            color: white;
            background-color: #303030;
            border-color: $main-color ;
        }

        span {
            color: $main-color;
            font-weight: 700;
            font-size: 1.5rem;
        }
    }
}
</style>