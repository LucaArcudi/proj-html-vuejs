<script>
export default {

}
</script>

<template>
    <section class="footer-top container-fluid">
        <nav class="row justify-content-between">
            <div class="col-2">
                <ul class="d-flex flex-column order">
                    <li>
                        <h6>ORDER ONLINE</h6>
                    </li>
                    <li>Appetizers</li>
                    <li>Burgers</li>
                    <li>Pizza</li>
                    <li>Fries</li>
                    <li>Sides</li>
                    <li>Desserts</li>
                    <li>Beverages</li>
                    <li>Specials</li>
                </ul>
            </div>
            <div class="col-2">
                <ul class="d-flex flex-column navigate">
                    <li>
                        <h6>NAVIGATE</h6>
                    </li>
                    <li>Home</li>
                    <li>Alternate Home</li>
                    <li>Menu</li>
                    <li>About</li>
                    <li>News</li>
                    <li>Contact Us</li>
                    <li>Cart</li>
                </ul>
            </div>
            <div class="col-2">
                <ul class="d-flex flex-column information">
                    <li>
                        <h6>INFORMATION</h6>
                    </li>
                    <li>My Account</li>
                    <li>Terms Of Service</li>
                    <li>Privacy Policy</li>
                    <li>
                        <img src="../../assets/img/app-store-badge-200x67.png" alt="">
                    </li>
                    <li>
                        <img src="../../assets/img/play-store-badge-200x67.png" alt="">
                    </li>
                </ul>
            </div>
            <div class="col-2">
                <ul class="d-flex flex-column opening">
                    <li>
                        <h6>OPENING HOURS</h6>
                    </li>
                    <li>
                        Mon - <span>10AM to 11PM </span>
                    </li>
                    <li>
                        Tue - <span>10AM to 11PM </span>
                    </li>
                    <li>
                        Wed - <span>10AM to 11PM </span>
                    </li>
                    <li>
                        Thur - <span>10AM to 11PM </span>
                    </li>
                    <li>
                        Fri - <span>10AM to 11PM </span>
                    </li>
                    <li>
                        Sat - <span>10AM to 1AM </span>
                    </li>
                    <li>
                        Sun - <span>11AM to 10PM </span>
                    </li>
                </ul>
            </div>
            <div class="col-2">
                <ul class="d-flex flex-column voucher">
                    <li>
                        <h6>VOUCHER</h6>
                    </li>
                    <li>
                        <img src="../../assets/img/footer-coupon-200x200.png" alt="">
                    </li>
                    <li>
                        <p>Just Use The Code</p>
                    </li>
                    <li>
                        <h5>FIRSTORDER</h5>
                    </li>
                    <li>
                        <p>AtChekout</p>
                    </li>
                </ul>
            </div>
        </nav>
    </section>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;

section.footer-top {
    padding-top: 5rem;

    .row {
        padding: 5rem 10rem;

        h5 {
            color: $brand_primary;
        }

        ul {
            color: $brand_primary;
            list-style-type: none;
            justify-content: start;

            li {
                font-size: .8rem;
                margin-bottom: 1rem;
            }


        }

        ul.navigate li:nth-child(2) {
            color: $brand_secondary;
        }

        ul.opening {
            h6 {
                margin-bottom: 1rem;
            }

            li {
                margin-bottom: 0;
            }

            span {
                color: $brand_secondary;
            }
        }



        ul.information img {
            margin-bottom: 1rem;
            border: 1px solid $brand_primary;
            border-radius: 10px;
        }

        ul.voucher {
            text-align: center;

            img {
                color: antiquewhite;
            }

            li {
                margin-bottom: 0;
            }

            h5 {
                color: $brand_secondary;
            }
        }


    }


}
</style>