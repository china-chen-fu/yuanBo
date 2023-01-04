<template>

    <div class="container">
        <div class="header">
            <div class="main">
                <div class="header-logo">
                    <img src="@/assets/image/header/logo.png" alt="">
                </div>


                <div class="header-nav">
                    <template v-for="(item, index) in headerData">
                        <div class="header-nav-item" :class="index == headerDataIndex ? 'active' : ''">
                            {{ item }}
                        </div>

                    </template>
                </div>

            </div>
        </div>

        <div class="carousel">

            <div class="carousel-container">

                <div class="bottom">
                    <div class="main">
                        <div class="bottom-title">
                            <span>
                                三大平台
                            </span>
                            <img src="@/assets/image/carousel/icon.png" alt="">
                        </div>
                        <div class="bottom-content">
                            <template v-for="item in carouselBottomData">
                                <div class="item">
                                    <span class="item-title">
                                        {{ item.title }}
                                    </span>
                                    <span class="item-describe">
                                        {{ item.describe }}
                                    </span>
                                </div>
                            </template>

                        </div>

                        <div class="detail">
                            <span>
                                查看更多
                            </span>
                        </div>
                    </div>
                </div>
            </div>


        </div>

        <div class="service-scope">
            <div class="tab-bar">
                <div class="main">
                    <div class="tab-bar-title">
                        <span>智能化软件系统</span>
                    </div>
                    <div class="tab-bar-container">
                        <template v-for="(item, index) in serviceScopeTabData">
                            <div class="item" :class="index == serviceScopeTabIndex ? 'active' : ''">
                                <img :src="`/_nuxt/assets/image/${item.imgURL}${serviceScopeTabIndex == index ? '-active' : ''}.png`"
                                    alt="">
                                <span>{{ item.describe }}</span>
                            </div>
                        </template>
                    </div>
                </div>
            </div>

            <div class="tab-bar-content">
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


        </div>

        <div class="solution">
            <div class="main">
                <div class="tab-bar">
                   <template v-for="(item,index) in solutionTabData">
                    <div :class="index==solutionTabIndex?'active':''">
                       {{item}} 
                    </div>
                   </template>
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
                <div class="title">
                    鼋博企业文化
                </div>
                <div class="content">
                    <template v-for="item in cultureData">
                        <div class="item">
                            <img :src="`/_nuxt/assets/image/${item.imgURL}`" alt="">
                            <span class="core">{{ item.core }}</span>
                            <span class="describe">{{ item.describe }}</span>
                        </div>
                    </template>

                </div>
            </div>
        </div>

        <div class="breaking-news">
            <div class="main">
                <div class="title">
                    鼋博大事件
                </div>
                <div class="content">
                    <div class="left">
                        <div class="left-title">
                            <img src="@/assets/image/breaking-news/title.png" alt="">
                        </div>
                        <div class="left-content">
                            <div class="left-content-title">
                                2020年2月
                            </div>
                            <div class="left-content-describe">
                                创立江苏鼋博群智能技术有限公司创立江苏鼋博群智能技术有限公司创立江苏鼋博群智能技术有限公司...
                            </div>
                            <div class="pagination">

                            </div>
                        </div>
                    </div>
                    <div class="right">
                        <span class="right-title">
                            社会尊重、客户称赞、员工自豪
                        </span>
                        <div class="right-content">
                            <span>
                                元理、元动、元生，元创；
                                <br>
                                博文、博大、博智、博弈。
                            </span>
                        </div>
                    </div>
                </div>
                <div class="time-line">
                    <div class="image-container">
                        <template v-for="(item, index) in timeLineData">
                            <img :src="`/_nuxt/assets/image/${item}`" alt=""
                                :class="index == timeLineIndex ? 'active' : ''">
                        </template>
                    </div>
                </div>
            </div>
        </div>

        <div class="cooperative-partner">
            <div class="main">
                <div class="title">
                    携手共赢，与合作伙伴共建专业服务环境！
                </div>
                <img src="@/assets/image/cooperative-partner/partner.png" alt="">
            </div>
        </div>

        <div class="relevant-information">
            <div class="main">
                <div class="left">
                    <img :src="`/_nuxt/assets/image/${relevantInformationData.logoURL}`" alt="">
                    <div class="information">
                        <div class="address">
                            {{ relevantInformationData.address }}
                        </div>
                        <div class="telephone">
                            {{ relevantInformationData.telephone }}
                        </div>
                        <div class="e-mail">
                            {{ relevantInformationData.eMail }}
                        </div>

                    </div>
                    <div class="copy-right">
                        {{ relevantInformationData.copyRight }}
                    </div>
                </div>

                <div class="right">
                    <img :src="`/_nuxt/assets/image/${relevantInformationData.officialAccountURL}`" alt="">
                    <span>
                        微信公众号
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
//header
const headerDataIndex = 0
const headerData = ['产品应用', '平台介绍', '服务支持', '关于鼋博', '加入我们']


//carousel
const carouselBottomData = [
    {
        title: '数字物联平台',
        describe: '物连平台、设备接入、数据处理'
    },
    {
        title: '应用开放平台',
        describe: '身份认证、入口管理、统一标准'
    },
    {
        title: '服务运维平台',
        describe: '健康监控、效率监控、故障监控'
    }

]

//service-scope
const serviceScopeTabIndex = 3
const serviceScopeTabData = [{
    imgURL: 'service-scope/data-visualization',
    describe: '数据可视化',
}, {
    imgURL: 'service-scope/water-electricity',
    describe: '水电收费',
},
{
    imgURL: 'service-scope/lighting-monitoring',
    describe: '照明监控',
}, {
    imgURL: 'service-scope/home-automation',
    describe: '智能家居',
}, {
    imgURL: 'service-scope/water-supply',
    describe: '给水管网',
},
{
    imgURL: 'service-scope/power-supply',
    describe: '供电运维',
},
{
    imgURL: 'service-scope/electrical-fire',
    describe: '电气火灾',
}
]

//solution
const solutionTabIndex=7
const solutionTabData=['智能电表','智能电表','敏捷网关','路灯控制','灯光控制','湿度监测','湿度监测','智能硬件']

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

//culture
const cultureData = [{
    imgURL: 'culture/img1.png',
    core: '文化',
    describe: '守正创新、行稳致远',
},
{
    imgURL: 'culture/img2.png',
    core: '理念',
    describe: '德载万物、品行天下',
},
{
    imgURL: 'culture/img3.png',
    core: '使命',
    describe: '零碳赋能未来、服务创造价值',
},
{
    imgURL: 'culture/img4.png',
    core: '愿景',
    describe: '群可信 创未来',
},
]

//breaking-news
const timeLineIndex = 5
const timeLineData = [
    'breaking-news/yb.png',
    'breaking-news/jndx.png',
    'breaking-news/xys.png',
    'breaking-news/jndx.png',
    'breaking-news/jndx.png',
    'breaking-news/yb.png',
    'breaking-news/xys.png',
    'breaking-news/yb.png',
    'breaking-news/yb.png',
    'breaking-news/jndx.png',
    'breaking-news/xys.png',
    'breaking-news/jndx.png',
    'breaking-news/yb.png',
]

//relevant-information
const relevantInformationData = {
    logoURL: 'relevant-information/logo.png',
    address: '地址：江苏省无锡市滨湖区锦溪路99号B区3单元1楼',
    telephone: '电话：0510-85180206',
    eMail: '邮箱：YunBoo2020@yunboo.com.cn',
    copyRight: '© 2021 Landify UI Kit. All rights reserved',
    officialAccountURL: 'relevant-information/officialAccount.png'

}

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
        background: #4B2684;
        align-items: center;

        .main {
            display: flex;
            align-items: center;

            .header-logo {

                img {
                    width: 130px;
                    height: 48px;
                }
            }

            .header-nav {
                margin-left: 452px;
                display: flex;
                justify-content: center;
                align-items: center;

                .header-nav-item {
                    width: 64px;
                    height: 23px;
                    margin-right: 72px;
                    font-size: 16px;
                    font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                    font-weight: 500;
                    color: #FFFFFF;
                    line-height: 23px;
                }

                .active {
                    padding: 18px 0 17px 0;
                    border-bottom: 2px solid #FFFFFF;
                }
            }
        }
    }

    .carousel {
        width: $container-width;
        height: 666px;
        background-image: url('@/assets/image/carousel/carousel1.jpg');
        background-size: cover;

        .carousel-container {
            height: 666px;
            position: relative;

            .bottom {
                width: $container-width;
                height: 105px;
                position: absolute;
                left: 0;
                bottom: 0;
                background: rgba(48, 48, 81, 0.7);

                .main {
                    display: flex;
                    height: 100%;

                    .bottom-title {
                        padding-right: 36px;
                        border-right: 1px solid rgba(255, 255, 255, 0.6);
                        display: flex;
                        justify-content: center;
                        align-items: center;

                        span {
                            height: 26px;
                            margin-right: 2px;
                            font-size: 18px;
                            font-family: Source Han Sans CN-Bold, Source Han Sans CN;
                            font-weight: bold;
                            color: #8645FF;
                            line-height: 26px;
                        }

                        img {
                            height: 18px;
                            width: 18px;
                        }
                    }

                    .bottom-content {
                        display: flex;
                        align-items: center;

                        .item {
                            padding: 30px 36px 24px 72px;
                            border-right: 1px solid rgba(255, 255, 255, 0.6);
                            display: flex;
                            flex-direction: column;

                            .item-title {
                                height: 25px;
                                font-size: 18px;
                                font-family: PingFang SC-Medium, PingFang SC;
                                font-weight: 500;
                                color: rgba(255, 255, 255, 0.87);
                                line-height: 25px;
                            }

                            .item-describe {
                                height: 20px;
                                margin-top: 6px;
                                font-size: 14px;
                                font-family: PingFang SC-Medium, PingFang SC;
                                font-weight: 500;
                                color: rgba(255, 255, 255, 0.6);
                                line-height: 20px;
                            }
                        }
                    }

                    .detail {
                        height: 100%;
                        margin-left: 36px;
                        display: flex;
                        align-items: center;

                        span {
                            height: 26px;
                            padding-bottom: 4px;
                            border-bottom: 1px solid #3B82F6;
                            font-size: 18px;
                            font-family: Source Han Sans CN-Bold, Source Han Sans CN;
                            font-weight: bold;
                            color: #3B82F6;
                            line-height: 26px;
                        }
                    }
                }
            }
        }
    }


    .service-scope {
        width: $container-width;
        background: #202638;

        .tab-bar {
            background-color: #fff;

            .main {
                display: flex;
                flex-direction: column;
                align-items: center;

                .tab-bar-title {
                    margin-top: 45px;

                    span {
                        height: 41px;
                        font-size: 28px;
                        font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                        font-weight: 400;
                        color: #18191A;
                        line-height: 41px;
                    }
                }

                .tab-bar-container {
                    width: $main-width;
                    margin-top: 40px;
                    display: flex;
                    justify-content: space-between;

                    .item {
                        position: relative;
                        display: flex;
                        flex-direction: column;
                        align-items: center;

                        img {
                            width: 48px;
                            height: 48px;
                        }

                        span {
                            height: 23px;
                            margin-top: 14px;
                            margin-bottom: 31px;
                            font-size: 16px;
                            font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                            font-weight: 400;
                            color: #18191A;
                            line-height: 23px;
                        }
                    }

                    .active::after {
                        content: '';
                        position: absolute;
                        top: 101px;
                        border: 8px solid #23293D;
                        border-left-color: transparent;
                        border-top-color: transparent;
                        border-right-color: transparent;
                    }

                    .active {
                        span {
                            color: #8645FF;
                        }
                    }
                }
            }
        }

        .tab-bar-content {
            background: #202638;
            height: 600px;

            .main {
                display: flex;

                .left {
                    margin-top: 172px;
                    padding-right: 309px;
                    color: #FFFFFF;

                    .title {
                        height: 41px;
                        font-size: 28px;
                        font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                        font-weight: 500;
                        color: #FFFFFF;
                        line-height: 41px;

                    }

                    .content {
                        padding-top: 36px;
                        margin: 0;
                        padding-inline-start: 39px;
                        padding-bottom: 22px;

                        li {
                            height: 26px;
                            padding-bottom: 15px;
                            font-size: 18px;
                            font-family: Source Han Sans CN-Regular;
                            color: #FFFFFF;
                            line-height: 26px;
                        }

                        li::marker {
                            color: #8645FF;
                        }
                    }

                    .detail {
                        width: 100px;
                        height: 32px;
                        border-radius: 50px 50px 50px 50px;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        opacity: 1;
                        border: 1px solid #FFFFFF;


                        span {
                            height: 20px;
                            font-size: 14px;
                            font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                            font-weight: 400;
                            color: #FFFFFF;
                            line-height: 20px;
                        }
                    }


                }


                .right {
                    padding-top: 99px;

                    img {
                        width: 600px;
                    }
                }
            }
        }

    }

    .solution {
        width: $container-width;
        height: 680px;
        background-image: url('@/assets/image/solution/bck.jpg');
        background-size: cover;

        .main {
            height: 100%;
            display: flex;
            padding-top: 89px;
            padding-bottom: 87px;

            .tab-bar {
                width: 140px;
                height: 463px;
                border-right: 1px solid #BCC2CA;
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: space-around;

                div {
                    height: 23px;
                    padding-left: 52px;
                    padding-right: 24px;
                    border-right: 3px solid transparent;
                    font-size: 16px;
                    font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                    font-weight: 400;
                    color: #2F3133;
                    line-height: 23px;
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
        background-image: url('@/assets/image/culture/bck.png');
        background-size: cover;

        .main {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;

            .title {

                height: 40px;
                margin-top: 79px;
                font-size: 28px;
                font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                font-weight: 500;
                color: #18191A;
                line-height: 33px;

            }

            .content {
                width: $main-width;
                margin-top: 117px;
                display: flex;
                justify-content: space-around;

                .item {
                    display: flex;
                    flex-direction: column;
                    align-items: center;

                    img {
                        width: 100px;
                    }

                    .core {
                        height: 31px;
                        margin-top: 28px;
                        font-size: 21px;
                        font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                        font-weight: 500;
                        color: #18191A;
                        line-height: 25px;
                    }

                    .describe {
                        height: 25px;
                        margin-top: 7px;
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

    .breaking-news {
        width: $container-width;
        background: #EFF3FC;

        .main {
            .title {
                height: 40px;
                margin-top: 60px;
                font-size: 28px;
                font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                font-weight: 500;
                color: #18191A;
                line-height: 33px;
            }

            .content {
                display: flex;
                margin-top: 57px;

                .left {
                    width: 615px;
                    display: flex;

                    // box-shadow: 5px 5px 10px 0px RGBA(216, 219, 227, 0.5);
                    .left-title {
                        width: 301px;
                        height: 226px;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        background: #5A3791;
                        border-radius: 21px 0 0 21px;

                        img {
                            width: 172px;
                        }
                    }

                    .left-content {
                        padding: 29px 36px 28px 36px;
                        background: #FFFFFF;
                        border-radius: 0 21px 21px 0;

                        .left-content-title {
                            width: 242px;
                            height: 31px;
                            font-size: 21px;
                            font-family: Source Han Sans CN-Bold, Source Han Sans CN;
                            font-weight: bold;
                            color: #18191A;
                            line-height: 25px;
                        }

                        .left-content-describe {
                            width: 242px;
                            height: 60px;
                            margin-top: 14px;
                            font-size: 14px;
                            font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                            font-weight: 400;
                            color: #8D9094;
                            line-height: 16px;
                        }
                    }
                }

                .right {
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    margin-left: 141px;

                    .right-title {
                        height: 31px;
                        font-size: 21px;
                        font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                        font-weight: 500;
                        color: #18191A;
                        line-height: 25px;
                    }

                    .right-content {
                        width: 294px;
                        margin-top: 35px;

                        span {
                            width: 215px;
                            height: 51px;
                            font-size: 18px;
                            font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                            font-weight: 400;
                            color: #18191A;
                            line-height: 21px;
                            word-break: normal;
                            white-space: pre-wrap;
                            word-wrap: break-word;
                        }
                    }
                }
            }

            .time-line {
                width: 1050px;
                height: 53px;
                margin-top: 93px;
                margin-bottom: 67px;
                position: relative;
                opacity: 1;
                border-top: 1px solid #18191A;

                .image-container {
                    width: 1006px;
                    height: 53px;
                    top: -50%;
                    left: 22px;
                    position: absolute;
                    display: flex;
                    justify-content: space-around;
                    align-items: center;

                    img {
                        width: 32px;
                        height: 32px;
                    }

                    .active {
                        transform: scale(calc(52/32));
                    }
                }
            }
        }
    }

    .cooperative-partner {
        width: $container-width;
        background: #FFFFFF;

        .main {
            display: flex;
            justify-content: center;
            flex-direction: column;
            align-items: center;

            .title {
                height: 36px;
                margin-top: 84px;
                font-size: 25px;
                font-family: Source Han Sans CN-Medium, Source Han Sans CN;
                font-weight: 500;
                color: #2F3133;
                line-height: 29px;
            }

            img {
                width: 883px;
                margin-top: 42px;
                margin-bottom: 84px;
            }
        }
    }

    .relevant-information {
        width: $container-width;
        height: 245px;
        background: #5A3791;

        .main {
            height: 245px;
            display: flex;
            justify-content: space-between;
            align-items: center;

            .left {
                img {
                    width: 129px;
                    height: 42px;
                }

                .information {
                    margin-top: 14px;

                    div {
                        height: 18px;
                        margin-bottom: 7px;
                        font-size: 12px;
                        font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                        font-weight: 400;
                        color: #FFFFFF;
                        line-height: 14px;
                    }
                }

                .copy-right {
                    height: 18px;
                    margin-top: 14px;
                    font-size: 12px;
                    font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                    font-weight: 400;
                    color: #D1D5DB;
                    line-height: 18px;
                }
            }

            .right {
                display: flex;
                flex-direction: column;
                align-items: center;

                img {
                    height: 105px;
                    width: 105px;
                }

                span {
                    height: 18px;
                    margin-top: 14px;
                    font-size: 12px;
                    font-family: Source Han Sans CN-Regular, Source Han Sans CN;
                    font-weight: 400;
                    color: #FFFFFF;
                    line-height: 14px;
                }
            }
        }


    }
}
</style>


