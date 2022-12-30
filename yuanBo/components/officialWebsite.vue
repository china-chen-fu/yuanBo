<template>
    <div class="container">
        <div class="header">
            <div class="main">
                <div class="header-logo">
                    <img src="@/assets/image/header/logo.png" alt="">
                </div>

                <div class="header-nav">
                    <div class="header-nav-item active">
                        关于我们
                    </div>
                    <div class="header-nav-item">
                        三大基座
                    </div>
                    <div class="header-nav-item">
                        产品应用
                    </div>
                    <div class="header-nav-item">
                        企业文化
                    </div>
                    <div class="header-nav-item">
                        发展历程
                    </div>
                </div>
            </div>
        </div>

        <div class="carousel">
            <div class="main">
                TODO
            </div>
        </div>

        <div class="concept">
            <div class="concept-header">
                <div class="main">
                    <div class="title">
                        三大基座
                    </div>
                    <div class="describe">
                        以“数字 物联、应用开放、服务运维”为基座， 以“应用场景”为引擎。提供业务可视、场景可视和数据可视的智慧物联产品。
                    </div>
                </div>
            </div>

            <div class="concept-content">
                <div class="main">
                    <div class="tab-bar">
                        <div class="tab-bar-item active">
                            <img src="@/assets/image/concept/figure.png" alt="">
                            <span>数字物联基座</span>
                        </div>
                        <div class="tab-bar-item">
                            <img src="@/assets/image/concept/application.png" alt="">
                            <span>应用开发基座</span>
                        </div>
                        <div class="tab-bar-item">
                            <img src="@/assets/image/concept/service.png" alt="">
                            <span>服务运维基座</span>
                        </div>
                    </div>

                    
                </div>
            </div>

        </div>

        <div class="service-scope">

            <div class="service-scope-header">
                <div class="main">

                </div>
            </div>
            <div class="service-scope-content">
                <div class="main">

                </div>
            </div>
        </div>

        <div class="solution">
            <div class="main">

            </div>
        </div>

        <div class="data-presentation">
            <div class="main">

            </div>
        </div>

        <div class="case">
            <div class="main">

            </div>
        </div>

        <div class="culture">
            <div class="main">

            </div>
        </div>

        <div class="breaking-news">
            <div class="main">

            </div>
        </div>

        <div class="cooperative-partner">
            <div class="main">

            </div>
        </div>

        <div class="relevant-information">
            <div class="main">

            </div>
        </div>
    </div>
</template>
<script setup>

</script>
<style lang="scss" scope>
$container-width: 100%;
$main-width: 1200px;

.container {
    width: $container-width;
    display: flex;
    flex-direction: column;
    align-items: center;


    .main {
        width: $main-width;
    }

    .header {
        width: $container-width;
        height: 63px;
        display: flex;
        justify-content: center;
        background: #5A3791;
        align-items: center;

        .main {
            display: flex;
            align-items: center;

            .header-logo {
                margin-right: 381px;

                img {
                    width: 129px;
                }
            }

            .header-nav {
                display: flex;
                justify-content: center;

                .header-nav-item {
                    margin-right: 63px;
                    position: relative;
                    font-size: 14px;
                    font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                    font-weight: 500;
                    color: #FFFFFF;
                    line-height: 16px;
                }

                .active::after {
                    content: "";
                    position: absolute;
                    top: 37px;
                    left: 0px;
                    width: 56px;
                    height: 2px;
                    background: #FFFFFF;
                }
            }
        }
    }

    .carousel {
        width: $container-width;
        height: 572px;
        background-color: #202638;
    }

    .concept {
        width: $container-width;
        height: 1174px;
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: #fff;

        .concept-header {
            height: 190px;

            .main {
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;

                .title {
                    padding-top: 40px;
                    padding-bottom: 21px;
                    font-size: 32px;
                    font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                    font-weight: 500;
                    color: #18191A;
                    line-height: 37px;
                }

                .describe {
                    padding-bottom: 65px;
                    font-size: 14px;
                    font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                    font-weight: 400;
                    color: #8D9094;
                    line-height: 16px;
                }
            }
        }

        .concept-content {
            height: 983px;
            width: $container-width;
            background-image: url('@/assets/image/concept/concept-bck.png');
            background-size: cover;
            display: flex;
            justify-content: center;

            .main {
                display: flex;
                flex-direction: column;
                align-items: center;

                .tab-bar {
                    width: 100%;
                    padding-bottom: 71px;
                    display: flex;
                    justify-content: space-around;

                    .tab-bar-item {
                        position: relative;
                        display: flex;
                        flex-direction: column;
                        align-items: center;

                        img {
                            width: 126px;
                            padding-bottom: 14px;
                        }

                        span {
                            font-size: 25px;
                            font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                            font-weight: 500;
                            color: #18191A;
                            line-height: 29px;
                        }
                    }

                    .active::after {
                        content: "";
                        position: absolute;
                        top: 200px;
                        left: 0px;
                        width: 147px;
                        height: 4px;
                        background: #8645FF;
                        border-radius: 42px 42px 42px 42px;
                    }
                }
            }
        }
    }

    .service-scope {
        width: $container-width;

        .service-scope-header {
            width: $container-width;
            background-color: #fff;
        }

        .service-scope-content {
            width: $container-width;
            height: 525px;
            background: #202638;
        }

    }

    .solution {
        width: $container-width;
        height: 595px;
        border-color: aquamarine;
    }

    .data-presentation {
        width: $container-width;
        height: 525px;
        background-color: #202638;
    }

    .case {
        width: $container-width;
        height: 824px;
        background: orange;
    }

    .culture {
        width: $container-width;

        height: 595px;
        background-color: purple;

    }

    .breaking-news {
        width: $container-width;
        height: 595px;
        background: #EFF3FC;
    }

    .cooperative-partner {
        width: $container-width;
        height: 239px;
        background: #FFFFFF;
    }

    .relevant-information {
        width: $container-width;
        height: 245px;
        background: #5A3791;
    }
}
</style>


