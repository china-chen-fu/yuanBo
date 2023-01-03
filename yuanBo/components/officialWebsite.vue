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


                    <div class="tab-content">
                        <div class="left">

                        </div>
                    </div>
                </div>

            </div>


            <div class="service-scope-header">
                <div class="main">

                </div>
            </div>
        </div>

        <div class="service-scope">
            <div class="main">
                <div class="left">
                    <div class="title">
                        水电收费
                    </div>
                    <ul class="content">
                        <li>核心业务：水电充值、配额下发</li>
                        <li>能耗分析：用能监测、缴费提醒</li>
                        <li>财务管理：配额指标、收支核算</li>
                        <li>后台工具：统计报表、信息维护</li>
                    </ul>
                    <div class="detail">
                        <span>
                            了解详情
                        </span>
                    </div>
                </div>

                <div class="right">
                    <img src="@/assets/image/service-scope/water-power.png" alt="">
                </div>
            </div>
        </div>

        <div class="solution">
            <div class="main">
                <div class="tab-bar">

                    <div>
                        智能电表
                    </div>
                    <div>
                        智能水表
                    </div>
                    <div>
                        敏捷网关
                    </div>
                    <div>
                        路灯控制
                    </div>
                    <div>
                        灯光控制
                    </div>
                    <div>
                        湿度监测
                    </div>
                    <div>
                        湿度监测
                    </div>

                    <div class="active">
                        智能硬件
                    </div>

                </div>

                <div class="tab-container">
                    <div class="content">
                        <div class="title">
                            智能硬件解决方案
                        </div>
                        <div class="cutting-line">

                        </div>

                        <div class="introduce">
                            硬件定位智能升级
                        </div>

                        <div class="describe-box">
                            <template v-for="(item, index) in ['敏捷网关', '敏捷网关', '敏捷网关', '敏捷网关记录']">
                                <div class="describe">
                                    <div class="dot">

                                    </div>
                                    <div class="text">
                                        {{ item }}
                                    </div>
                                </div>
                            </template>

                        </div>

                        <div class="detail">
                            <span>
                                了解详情
                            </span>
                        </div>
                    </div>

                    <div class="client">
                        <div>
                            <img src="@/assets/image/solution/jndx.png" alt="">
                            <span>江南大学</span>
                        </div>
                        <div>
                            <img src="@/assets/image/solution/xys.png" alt="">
                            <span>西雅斯学院</span>
                        </div>
                    </div>

                </div>



            </div>
        </div>

        <div class="data-presentation">
            <div class="main">
                <div class="title">
                    海量数据，铸就强大行业优势！
                </div>

                <div class="content">
                    <template v-for="(item, index) in dataPresentation">
                        <div class="item">
                            <img :src="`/_nuxt/assets/image/${item.imgURL}`" alt="">
                            <span>
                                {{ item.number }}
                            </span>

                            <div class="describe">
                                <span>
                                    {{ item.describe }}
                                </span>
                            </div>

                        </div>
                    </template>

                </div>
            </div>
        </div>

        <div class="case">
            <div class="main case-top">
                <div class="title">
                    <span class="mainheading">
                        服务支持
                    </span>
                    <span class="subheading">
                        全面AI赋能，助力产业智能化升级
                    </span>
                </div>

                <div class="content">
                    <div class="left">
                        <div class="top">
                            <div class="content-title">
                                数字能源
                            </div>
                            <div class="cutting-line">

                            </div>

                            <div class="content-describe">
                                鼋博紧随时代，以国家“双碳战略”为目标，以“零碳校园”为驱动，以“能源管理、绿色发展”为核心，以“数字物联、应用开放、服务运维”为基座，以“应用场景”为引擎。提供业务可视、场景可视和数据可视的智慧物联产品。
                            </div>


                            <div class="describe-box">
                                <template v-for="(item, index) in caseList">
                                    <div class="describe">
                                        <div class="dot">

                                        </div>
                                        <div class="text">
                                            {{ item }}
                                        </div>
                                    </div>
                                </template>

                            </div>

                            <div class="detail">
                                <span>
                                    了解更多
                                </span>
                            </div>
                        </div>

                        <div class="client">
                            <div>
                                <img src="@/assets/image/case/jndx.png" alt="">
                            </div>
                            <div>
                                <img src="@/assets/image/case/xys.png" alt="">
                            </div>
                        </div>
                    </div>

                    <div class="right">
                        <div class="tab-bar">
                            <template v-for="(item, index) in caseTabBar">
                                <div class="item" :class="caseTabBarIndex == index ? 'active' : ''">
                                    {{ item }}
                                </div>
                            </template>

                        </div>

                        <div class="more">
                            <span>
                                更多行业案例...
                            </span>
                        </div>
                    </div>
                </div>


            </div>

            <div class="data">
                <div class="main">
                    <div class="item1">
                        <span class="number">
                            100+
                        </span>
                        <span class="describe">
                            落地行业
                        </span>
                        <div class="cutting-line">

                        </div>
                    </div>

                    <div class="item2">
                        <span class="number">
                            4000
                        </span>
                        <span class="describe">
                            落地项目
                        </span>
                        <div class="cutting-line">

                        </div>
                    </div>

                    <div class="item3">
                        <span class="number">
                            8000+
                        </span>
                        <span class="describe">
                            企业用户
                        </span>
                    </div>
                </div>
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
//data-presentation
const dataPresentation = [
    {
        imgURL: 'data-presentation/img1.png',
        number: '2000万',
        describe: '数据能力优势内容展现数据能力优势内容展现',
    },
    {
        imgURL: 'data-presentation/img2.png',
        number: '7000万',
        describe: '数据能力优势内容展现数据能力优势内容展现',
    },
    {
        imgURL: 'data-presentation/img3.png',
        number: '3500万',
        describe: '数据能力优势内容展现数据能力优势内容展现',
    },
    {
        imgURL: 'data-presentation/img4.png',
        number: '95%',
        describe: '数据能力优势内容展现数据能力优势内容展现',
    },
    {
        imgURL: 'data-presentation/img5.png',
        number: '300+',
        describe: '数据能力优势内容展现数据能力优势内容展现',
    },
]

const caseList = ['路灯照明监控系统', '路灯照明监控系统', '路灯照明监控系统', '路灯照明监控系统', '路灯照明监控系统', '路灯照明监控系统']

const caseTabBar = ['数字能源', '智慧校园', '智慧交通', '住宅建筑', '医疗卫生', '工商企业', '数字乡村',]
const caseTabBarIndex = 4
const caseBottomData = [
    { number: '100+', describe: '落地行业' },
    { number: '4000', describe: '落地项目' },
    { number: '8000+', describe: '企业用户' }
]

</script>
<style lang="scss" scope>
$container-width: 100%;
$main-width: 1200px;

@font-face {
    font-family: Source Han Sans CN-Regular;
    src: url('@/assets/font/SourceHanSansCN-Regular.otf');
    font-weight: lighter;
    font-style: normal;
}

@font-face {
    font-family: Source Han Sans CN-Medium;
    src: url('@/assets/font/SourceHanSansCN-Regular.otf');
    font-weight: 500;
    font-style: normal;
}

@font-face {
    font-family: Source Han Sans CN-Bold;
    src: url('@/assets/font/SourceHanSansCN-Regular.otf');
    font-weight: bold;
    font-style: normal;
}

.container {
    width: $container-width;
    display: flex;
    flex-direction: column;
    align-items: center;


    .main {
        width: $main-width;
        margin: 0 auto;
    }

    .header {
        width: $container-width;
        height: 63px;
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
                    font-family: Source Han Sans CN-Medium;
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
                    font-family: Source Han Sans CN-Medium;
                    color: #18191A;
                    line-height: 37px;
                }

                .describe {
                    padding-bottom: 65px;
                    font-size: 14px;
                    font-family: Source Han Sans CN-Regular;
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
                            font-family: Source Han Sans CN-Regular;
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


        .service-scope-header {}
    }

    .service-scope {
        width: $container-width;
        height: 525px;
        background: #202638;

        .main {
            display: flex;

            .left {
                padding-top: 143px;
                color: #FFFFFF;
                padding-right: 270px;

                .title {
                    height: 36px;
                    font-size: 25px;
                    font-family: Source Han Sans CN-Medium;
                    color: #FFFFFF;
                    line-height: 29px;
                }

                .content {
                    padding-top: 31px;
                    margin: 0;
                    padding-inline-start: 28px;
                    padding-bottom: 20px;

                    li {
                        height: 23px;
                        padding-bottom: 13px;
                        font-size: 16px;
                        font-family: Source Han Sans CN-Regular;
                        color: #FFFFFF;
                        line-height: 18px;
                    }

                    li::marker {
                        color: #8645FF;
                    }
                }

                .detail {
                    width: 88px;
                    height: 28px;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    border-radius: 44px 44px 44px 44px;
                    opacity: 1;
                    border: 1px solid #FFFFFF;


                    span {
                        font-size: 12px;
                        font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                        font-weight: 400;
                        color: #FFFFFF;
                        line-height: 14px;
                    }
                }


            }


            .right {
                padding-top: 87px;

                img {
                    width: 525px;
                }
            }
        }

    }

    .solution {
        width: $container-width;
        height: 595px;
        background-image: url('@/assets/image/solution/bck.jpg');
        background-size: cover;

        .main {
            height: 100%;
            display: flex;
            padding-top: 77px;
            padding-bottom: 76px;

            .tab-bar {
                height: 442px;
                border-right: 1px solid #BCC2CA;

                div {
                    height: 20px;
                    padding-left: 46px;
                    padding-right: 19px;
                    margin-bottom: 28px;
                    font-size: 14px;
                    font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                    font-weight: 400;
                    color: #2F3133;
                    line-height: 20px;
                }

                div:first-of-type {
                    margin-top: 22px;
                }


                .active {
                    height: 26px;
                    border-right: 3px solid #8645FF;
                    background: linear-gradient(270deg, #D4C0FF 0%, rgba(212, 192, 255, 0) 100%);
                    border-radius: 0px 0px 0px 0px;
                    opacity: 1;
                }



            }

            .tab-container {
                padding-left: 69px;

                .content {
                    width: 535px;
                    border-bottom: 1px solid #9FA0A0;

                    .title {
                        height: 29px;
                        padding-top: 22px;
                        padding-bottom: 23px;
                        font-size: 25px;
                        font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                        font-weight: 500;
                        color: #18191A;
                        line-height: 29px;
                    }

                    .cutting-line {
                        width: 35px;
                        height: 3px;

                        background: #2F3133;
                        border-radius: 0px 0px 0px 0px;
                        opacity: 1;
                    }

                    .introduce {
                        height: 25px;
                        margin-top: 42px;
                        font-size: 21px;
                        font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                        font-weight: 400;
                        color: #8645FF;
                        line-height: 25px;

                    }

                    .describe-box {
                        width: 400px;
                        height: 60px;
                        margin-top: 18px;
                        display: flex;
                        flex-wrap: wrap;

                        .describe {
                            display: flex;
                            align-items: center;

                            .dot {
                                width: 5px;
                                height: 5px;
                                border-radius: 50%;
                                background: #8D9094;
                            }

                            .text {
                                height: 18px;
                                margin-left: 11px;
                                margin-right: 70px;
                                font-size: 16px;
                                font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                                font-weight: 400;
                                color: #8D9094;
                                line-height: 18px;

                            }
                        }
                    }

                    .detail {
                        width: 88px;
                        height: 28px;
                        margin-top: 42px;
                        margin-bottom: 42px;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        border-radius: 44px 44px 44px 44px;
                        opacity: 1;
                        border: 1px solid #8645FF;


                        span {

                            height: 14px;
                            font-size: 12px;
                            font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                            font-weight: 400;
                            color: #8645FF;
                            line-height: 14px;

                        }
                    }


                }

                .client {
                    margin-top: 44px;
                    display: flex;

                    div {

                        height: 32px;
                        margin-right: 28px;
                        display: flex;
                        justify-content: center;
                        align-items: center;

                        img {
                            width: 32px;
                            margin-right: 11px;
                        }

                        span {
                            height: 21px;
                            font-size: 18px;
                            font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                            font-weight: 400;
                            color: #2F3133;
                            line-height: 21px;
                        }
                    }
                }
            }



        }
    }

    .data-presentation {
        width: $container-width;
        height: 525px;
        background-image: url('@/assets/image/data-presentation/bck.png');
        background-size: cover;

        .main {
            display: flex;
            flex-direction: column;
            align-items: center;

            .title {
                height: 33px;
                margin-top: 68px;
                font-size: 28px;
                font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                font-weight: 400;
                color: #FFFFFF;
                line-height: 33px;

            }

            .content {
                display: flex;
                margin-top: 58px;

                .item {
                    margin-right: 51px;
                    display: flex;
                    flex-direction: column;
                    justify-content: center;
                    align-items: center;

                    img {
                        width: 63px;
                        height: 63px;
                        margin-top: 23px;
                    }

                    span {
                        height: 49px;
                        font-size: 42px;
                        font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                        font-weight: 500;
                        color: #FFFFFF;
                        line-height: 49px;
                    }

                    .describe span {
                        width: 140px;
                        margin-top: 14px;
                        display: flex;
                        justify-content: center;
                        text-align: center;
                        font-size: 12px;
                        font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                        font-weight: 400;
                        color: rgba(255, 255, 255, 0.6);
                        line-height: 14px;
                    }
                }
            }


        }
    }

    .case {
        width: $container-width;
        padding-bottom: 173px;
        position: relative;
        background-image: url('@/assets/image/case/bck.jpg');
        background-size: cover;

        .case-top.main {
            display: flex;
            flex-direction: column;


            .title {
                margin-top: 73px;
                display: flex;
                flex-direction: column;
                align-items: center;

                .mainheading {

                    height: 40px;
                    font-size: 28px;
                    font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                    font-weight: 500;
                    color: #FFFFFF;
                    line-height: 33px;

                }

                .subheading {
                    height: 23px;
                    margin-top: 11px;
                    font-size: 16px;
                    font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                    font-weight: 400;
                    color: #FFFFFF;
                    line-height: 18px;
                }
            }

            .content {
                display: flex;
                justify-content: space-between;

                .left {

                    .top {
                        border-bottom: 1px solid rgba(255, 255, 255, 0.4);

                        .content-title {

                            height: 36px;
                            font-size: 25px;
                            font-family: Source Han Sans CN-Bold, Source Han Sans CN;
                            font-weight: bold;
                            color: #FFFFFF;
                            line-height: 29px;

                        }

                        .cutting-line {
                            width: 42px;
                            height: 2px;
                            margin-top: 12px;
                            background: rgba(255, 255, 255, 0.6);
                            border-radius: 0px 0px 0px 0px;
                            opacity: 1;
                        }

                        .content-describe {
                            width: 667px;
                            height: 74px;
                            margin-top: 21px;
                            font-size: 14px;
                            font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                            font-weight: 400;
                            color: #FFFFFF;
                            line-height: 25px;
                        }

                        .describe-box {
                            width: 650px;
                            height: 60px;
                            margin-top: 18px;
                            display: flex;
                            flex-wrap: wrap;

                            .describe {
                                display: flex;
                                align-items: center;

                                .dot {
                                    width: 5px;
                                    height: 5px;
                                    border-radius: 50%;
                                    background: #FCFDFF;
                                }

                                .text {
                                    height: 25px;
                                    padding-left: 10px;
                                    padding-right: 53px;
                                    font-size: 14px;
                                    font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                                    font-weight: 400;
                                    color: #FFFFFF;
                                    line-height: 25px;
                                }
                            }
                        }

                        .detail {
                            width: 84px;
                            height: 32px;
                            margin-top: 42px;
                            margin-bottom: 32px;
                            display: flex;
                            justify-content: center;
                            align-items: center;
                            border-radius: 1px 1px 1px 1px;
                            opacity: 1;
                            border: 1px solid #FFFFFF;

                            span {
                                height: 18px;
                                font-size: 12px;
                                font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                                font-weight: 500;
                                color: #FFFFFF;
                                line-height: 14px;
                            }
                        }
                    }

                    .client {
                        display: flex;
                        margin-top: 35px;

                        div {
                            margin-right: 42px;

                            img {
                                width: 112px;
                            }
                        }
                    }




                }

                .right {
                    .tab-bar {
                        height: 388px;
                        padding-top: 26px;
                        background: rgba(0, 0, 0, 0.48);
                        border-radius: 3px 3px 3px 3px;
                        opacity: 1;

                        .item {
                            padding: 10px 56px;
                            height: 23px;
                            font-size: 16px;
                            font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                            font-weight: 500;
                            color: rgba(255, 255, 255, 0.87);
                            line-height: 18px;

                        }

                        .active {
                            border-left: 4px solid #B187FF;
                            border-radius: 0px 0px 0px 0px;
                            opacity: 1;
                            background: linear-gradient(270deg, #8544EE 0%, rgba(133, 68, 238, 0) 100%);
                        }
                    }

                    .more {
                        margin-top: 18px;
                        padding: 11px 33px;
                        background: rgba(0, 0, 0, 0.48);
                        border-radius: 3px 3px 3px 3px;

                        span {
                            height: 23px;
                            font-size: 16px;
                            font-family: Source Han Sans CN-Bold, Source Han Sans CN;
                            font-weight: bold;
                            color: rgba(255, 255, 255, 0.87);
                            line-height: 18px;
                        }
                    }
                }
            }


        }

        .data {
            position: absolute;
            bottom: 0;
            width: $container-width;
            height: 112px;
            display: flex;

            background: rgba(0, 0, 0, 0.6);
            border-radius: 0px 0px 0px 0px;
            opacity: 1;

            .main {
                display: flex;

                >div {
                    display: flex;
                    position: relative;
                    flex-direction: column;
                    align-items: center;
                }

                .number {
                    margin-top: 20px;
                    height: 53px;
                    font-size: 37px;
                    font-family: Source Han Sans CN-Bold, Source Han Sans CN;
                    font-weight: bold;
                    color: #FFFFFF;
                    line-height: 43px;
                }

                .describe {
                    height: 18px;
                    font-size: 12px;
                    font-family: Source Han Sans CN-Bold, Source Han Sans CN;
                    font-weight: bold;
                    color: #FFFFFF;
                    line-height: 14px;
                }

                .item1 {
                    width: 324px;
                }

                .item2 {
                    width: 403px;
                }

                .item3 {
                    width: 324px;
                }

                .cutting-line {                   
                    width: 0px;
                    height: 53px;
                    position: absolute;
                    top: 34px;
                    right: 0;
                    opacity: 1;
                    border: 1px solid rgba(255, 255, 255, 0.4);
                }
            }




        }

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


