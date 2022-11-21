# css
@charset "utf-8";
#pre_wrapper{position: relative;display: flex;flex-direction: column;overflow: hidden;}

/* footer */
#pre_wrapper #footer{position: fixed;height: 57px;width: 100%;border-top: 1px solid rgba(255, 255, 255, 0.2);bottom: 0;left: 0;z-index: 1000;}
#pre_wrapper #footer .scroll_down{position: absolute;left: 50px;top: 0px;display: block;width: 40px;height: 51px;overflow: hidden;text-indent: -100000px;background:url(https://lwi.nexon.com/kartdrift/gow/pre/scroll.png) no-repeat;cursor: default;}
#pre_wrapper #footer .btn_top{position: absolute;right: 0;top: 0;display: block;width: 57px;height: 57px;overflow: hidden;background-color:#FFE500;text-indent: -100000px;}
#pre_wrapper #footer .btn_top::after{position: absolute;width: 100%;height: 0;left: 0;bottom: 0;background-color: #4096FB;content: '';transition: height .4s ease;}
#pre_wrapper #footer .btn_top::before{position: absolute;width: 100%;height: 100%;left: 0;bottom: 0;background:url(https://lwi.nexon.com/kartdrift/gow/common/ico_btn.png) 50% 0 no-repeat;background-size: cover;content:'';z-index: 1;}
#pre_wrapper #footer .btn_top:hover::after{height: 100%}
#pre_wrapper #footer .btn_top:hover::before{background-position-y: 100%;}
#pre_wrapper footer{position: absolute;max-width: 1268px;width:100%;height: 27px;background-color: #000;bottom: 15px;left: 50%;transform: translateX(-50%);border-radius: 10px;color: #949494;font-size: 0.75rem;text-align: center;line-height: 1.563rem;}

/* container */
#back{position: fixed;left: 0;right: 0;top: 0;object-fit: cover;object-position: center bottom;width: 100%;}
.cover{background: rgba(0, 0, 0, 0.5);backdrop-filter: blur(10px);-webkit-backdrop-filter: blur(10px);position: absolute;width: 100%;height: 100%;top: 0;left: 0;}
#pre_wrapper #container{position: relative;display: flex;flex-direction: column;align-items: center;}
#pre_wrapper #container::after{content: '';width: 1px;height: 100%;background: rgba(255, 255, 255, 0.2); ;right: 196px;top: 0;position: absolute;}
#container > section{position: relative;width: 100%;display: flex;justify-content:center;padding: 130px 10px;align-items:center;max-height: 1003px;}
#container .intro{flex-direction: column;background:url(https://news.samsungdisplay.com/wp-content/uploads/2020/06/0616_S.jpg) 50% 0 no-repeat;background-size: cover;height: 100vh;}
.mobile #container .intro{height: 100vh;min-height: auto !important;}
#container .intro::after{position: absolute;content:'';background: rgba(0, 0, 0, 0.5);width: 100%;height: 100%;top: 0;left: 0;right: 0;}
#container .intro .title{display: flex;flex-direction: column;z-index: 1;align-items:center;width: 100%;}
#container .intro .title h1{max-width: 492px;width:100%;background:url(https://lwi.nexon.com/kartdrift/gow/pre/logo.svg) center bottom no-repeat;background-size: contain;z-index: 1;text-indent: -1000000px;}
#container .intro .title h1::after{content:'';display:block;width:100%;padding-top: 32.114%;}
#container .intro .title button{width: 725px;height: 78px;background:url(https://lwi.nexon.com/kartdrift/gow/pre/bg_btn.png) 50% 50% no-repeat;background-size: contain;font-weight: 700;font-size: 2.188rem;color: #2C2E31;transition: all .1s ease;margin:40px 0 20px 0;line-height: 4.875rem;}
:lang(th) #container .intro .title button{font-size: 1.4rem;}
#container .intro .title button:hover{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/bg_btn_over.png);color:#fff}
#container .intro .title button::after{display: inline-block;vertical-align: middle;margin-top:-8px;content: '';width: 57px;height: 24px;background:url(https://lwi.nexon.com/kartdrift/gow/pre/ico_arrow.svg) no-repeat;background-size: contain;margin-left: 7px;}
#container .intro .title button:hover::after{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/ico_arrow_over.svg)}
#container .intro .title p{font-weight: 700;font-size: 1.65rem;line-height: 2.75rem;color: #FFF;z-index: 1;text-align: center;}
#container .intro .title .desc_pre{background-color: #fff;border-radius: 20px;font-weight: 700; font-size: 20px;color: #000;margin-top: 5px;line-height: inherit;padding:4px 50px;font-size: 1.25rem;}

#container .intro .platform{position: absolute;width: 100%;display: flex;bottom: 150px;left: 0;justify-content: center;z-index: 102;align-items:center;flex-direction: column;}
#container .intro .platform ul{display: flex;width: 100%;margin-left: -15px;justify-content:center;align-items:center;flex-wrap:wrap}
#container .intro .platform li{height: 23px;overflow: hidden;position: relative;margin-left:13px;padding-right:13px;margin-bottom: 10px;display: flex;}
/*
.mobile .all #container .intro .platform .nexon,
.mobile .all #container .intro .platform .steam,
.mobile .all #container .intro .platform .xbox,
.mobile .all #container .intro .platform .ps{height: 23px;width:auto;background: transparent;border:0;padding-right: 8px;}
.mobile .all #container .intro .platform .nexon button,
.mobile .all #container .intro .platform .steam button,
.mobile .all #container .intro .platform .xbox button,
.mobile .all #container .intro .platform .ps button{cursor: default;}
*/
.all #container .intro .platform li{height: 37px;width: 147px;background: #000;border: 1px solid #FFFFFF;border-radius: 10px;padding-right: 0;}
.mobile .final.all #container .intro .platform li.nexon{border: 1px solid rgba(255, 255, 255, 0.3);}
.mobile .final.all #container .intro .platform li.nexon button{cursor: default;}
#container .intro .platform li button{display: flex;text-indent: -100000px;justify-content:center;width: 100%;height: 100%;font-size: 0;cursor: default;}
.all #container .intro .platform li button{cursor: pointer;}
.all #container .intro .platform li button.btn_ios{display: none;}
:lang(en) #container .intro .platform .btn_check{max-width: 240px;}
#container .intro .platform li button::before{content: '';background:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_nexon.svg) center center no-repeat;width: 62px;height: 100%;background-size: contain;}
#container .intro .platform li button::after{content: '';width: 1px;height: 11px;position: absolute;right: 0;top: 50%;transform: translateY(-50%);background-color: #fff;}
.all #container .intro .platform li button::after{display: none;}
/*
.mobile .all #container .intro .platform .nexon button::after,
.mobile .all #container .intro .platform .steam button::after,
.mobile .all #container .intro .platform .xbox button::after{display: block;}
*/
#container .intro .platform .nexon button::before{margin-top: 2px;}
#container .intro .platform .steam button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_steam.svg);width: 66px}
#container .intro .platform .xbox button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_xbox.svg);width: 82px}
#container .intro .platform .ps button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_ps4.svg);width: 74px}
#container .intro .platform .apple button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_apple.png);width: 88px}
#container .intro .platform .google button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_google.png);width: 103px}
.final #container .intro .box{position: absolute;width: 100%;display: flex;bottom: 80px;justify-content: center;z-index: 102;align-items:center;flex-direction: column;background: rgba(26, 26, 26, 0.8);border: 1px solid #000000;backdrop-filter: blur(10px);-webkit-backdrop-filter: blur(10px);border-radius: 10px;max-width: 1206px;padding:8px}
.final #container .intro .line{border: 1px dashed #404040;border-radius: 8px;padding:15px 8px 5px 8px;width: 100%;}
.final #container .intro .txt1{font-size:1.125rem;color:#999;border-bottom: 1px dashed #404040;padding-bottom:15px;width: 100%;text-align: center;margin-bottom: 15px;}
.final #container .intro .txt1::before{display: inline-block;vertical-align:middle;margin-top:-4px;content: '';width:19px;height: 18px;background:url(https://lwi.nexon.com/kartdrift/gow/final/ico_wn.png) center 0 no-repeat;background-size: contain;margin-right: 5px;}
.final #container .intro .txt2{font-size:0.813rem;color:#9A9A9A;padding:3px;width: 98%;text-align: center;margin-top: 10px;background: #414141;border-radius: 20px;}
.final #container .intro .platform{position: relative;bottom: initial;}
.final #container .intro .platform .apple button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_ios.png);width: 48px}
.final #container .intro .platform .google button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_android.png);width: 80px}
.final #container .intro .platform .apple button{flex:1}
.final #container .intro .platform li .btn_ios{font-size: 11px;padding:3px 8px;background: #fff;border-radius: 3px;color:#000;margin-left: 5px;text-indent: 0;flex: auto;cursor: pointer;}
.final #container .intro .platform li .btn_ios::after{width: 3.5px;height: 5px;margin-left: 5px;background:url(https://lwi.nexon.com/kartdrift/gow/pre/ico_ios.png) no-repeat;background-size: contain;display: inline-block;content: '';position: relative;}
.final #container .intro .platform li button.btn_ios::before{display:none}
/*
.all #container .intro .platform .apple button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_apple_en.png);width: 100px}
.all #container .intro .platform .google button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_google_en.png);width: 106px}
:lang(ko) .all #container .intro .platform .apple button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_apple_kr.png);width: 108px}
:lang(ko) .all #container .intro .platform .google button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_google_kr.png);width: 105px}
:lang(ja) .all #container .intro .platform .apple button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_apple_jp.png);width: 108px}
:lang(ja) .all #container .intro .platform .google button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_google_jp.png);width: 105px}
:lang(zh) .all #container .intro .platform .apple button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_apple_tw.png);width: 90px}
:lang(zh) .all #container .intro .platform .google button::before{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/plat_google_tw.png);width: 106px}
*/
#container .intro .platform .btn_check,
.all #container .intro .platform .btn_check{border-color: #FFE600;background-color: #FFE600;border-radius: 10px;max-width: 180px;width: 100%;height: 37px;padding:0}
#container .intro .platform .btn_check::before{display: none;}
#container .intro .platform .btn_check button{font-size: 16px;color: #000;display: flex;align-items:center;justify-content: center;width: 100%;margin-right: 0;text-indent: 0;cursor: pointer;}
#container .intro .platform .btn_check button::after{content: '';width: 12px;height: 17px;margin-left: 5px;background:url(https://lwi.nexon.com/kartdrift/gow/pre/ico_pop.png) no-repeat;background-size: contain;position: sticky;}
#container .intro .platform .btn_check:hover{background-color: #4096FB;border-color: #4096FB}
#container .intro .platform .btn_check:hover button{color: #fff;}
#container .intro .platform .google button::after,
#container .intro .platform .btn_check button::before{display: none;}
#container .registration{padding-top: 180px;}
#container .preForm{position:relative;max-width: 1210px;border: 5px solid #FFFFFF;border-top:0; border-radius: 5px;padding: 20px;width: 100%;display: flex;padding-top: 0;justify-content:space-between}
#container .preForm::before{content: '';width: 1210px;height: 38px;background:url(https://lwi.nexon.com/kartdrift/gow/pre/frame.png) no-repeat;position: absolute;top:-34px;left: -5px;}
#container .preForm .tit{display: flex;flex-direction: column;padding:40px 25px;z-index: 1;}
:lang(th) #container .preForm .tit{padding:40px 15px}
#container .preForm::after{content: '';width: 614px;height: 508px;position: absolute;bottom: -97px;left: -40px;background:url(https://lwi.nexon.com/kartdrift/gow/pre/char_pre.png) no-repeat;}
#container .preForm .tit h2{position: relative;;font-size: 2.5rem;line-height: 3.688rem;color: #fff;font-weight: 400;}
#container .preForm .tit h2::before{content:'';width: 207px;height: 67px;background: url(https://lwi.nexon.com/kartdrift/gow/pre/logo.svg) no-repeat;display: block;margin-bottom: 10px;background-size: contain;}
#container .preForm .tit h2::after{content:'';background: url(https://lwi.nexon.com/kartdrift/gow/pre/ico_pre.png) no-repeat;width: 7px;height: 142px;position: absolute;left: -20px;top: 50%;transform: translateY(-50%);}
#container .preForm .tit .date{font-size: 1rem;color: #fff;display: flex;flex-direction: column;margin-top: 30px;}
#container .preForm .tit .date strong{font-size: 1.25rem;color: #FFE600;}
#container .preForm .tit .date span{color: #FFE600;}
#container .preForm .inner{background: rgba(0, 0, 0, 0.8);border: 1px solid #FFFFFF;border-radius: 3px;padding: 10px;max-width: 756px;z-index: 1;width: 100%;}
#container .preForm .noti{background-color: #ECECEC;min-height: 550px;}



#container .preForm .noti h3{font-weight: 700;font-size: 1.563rem;color: #000;padding:30px 5px 15px 45px}
#container .preForm .input_info{border-top: 1px solid #FFFFFF;border-bottom: 1px solid #FFFFFF;padding: 30px 45px;background:url(https://lwi.nexon.com/kartdrift/gow/common/bg_noise-wt.gif) no-repeat;display: flex;flex-direction: column;}
#container .preForm .input_info label{font-family: 'Roboto';font-weight: 700;font-size: 2.188rem;line-height: 2.5rem;color: #000000;margin-bottom: 10px;}
#container .preForm .input_info input{border: 5px solid #000000;border-radius: 60px;font-weight: 400;font-size: 1rem;color: #3D3D3D;line-height: 42px;text-indent: 20px;}
#container .preForm .txt_info{padding:20px 45px;font-weight: 400;font-size: 1rem;line-height: 1.438rem;color: #646464;word-break: keep-all;}
#container .preForm .txt_info strong{color: #000;}
#container .preForm .agree{padding:0 45px}
#container .preForm .agree ul{background: #FFFFFF;border-radius: 10px;padding: 10px 20px;}
.preForm .agree li{position: relative;width: 100%;margin: 7px 0;}
.agree li button,
.agree li a,
#container .preForm .noti_list li a{display: inline-block;font-size: 0.75rem;color: #3385FF;vertical-align: top;margin-left: 3px;}
#container .preForm .noti_list li a{display: contents;}

#container .preForm .noti_list{padding: 20px  20px 30px 65px;}
#container .preForm .noti_list li{font-size: 0.75rem;line-height: 1.438rem;color: #646464;display: flex;align-items:center}
#container .preForm .noti_list li::before{content: '';margin-right: 10px;width: 6px;height: 2px;background-color: #646464;}
#container .preForm .btn_confirm{width: 100%;height: 66px;background-color: #3385FF;font-weight: 700;font-size: 1.75rem;color: #FFF;margin: 10px 0;display: flex;align-items:center;justify-content:center}
#container .preForm .btn_confirm.disable,
#container .preForm .btn_confirm.disable:hover{cursor: default;background-color: #727272;}
#container .preForm .btn_confirm.disable::after{display: none;}
#container .preForm .btn_confirm::after{content: '';width: 0;height: 12px;background:url(https://lwi.nexon.com/kartdrift/gow/pre/ico_arrow_over.svg) no-repeat;background-size: contain;margin-left: 7px;transition: all .2s ease;transform: scale(0);margin-top: 8px;}
#container .preForm .btn_confirm:hover{background-color: #40BAFF;}
#container .preForm .btn_confirm:hover::after{transform: scale(1);width: 28px;}
#container .preForm .app_download{width: 100%;display: flex;justify-content:center;}

#afctv_cpa_proc{display: none;}



#container #event1{background:url(https://lwi.nexon.com/kartdrift/gow/pre/back_event.png) 50% 0 no-repeat;background-size: cover;max-height: fit-content;}
#container #event1 .inner{display: flex;max-width: 1290px;width: 100%;justify-content: space-between;align-items:center}
#event1 .info{max-width: 535px;width:100%;position: relative;display: flex;flex-direction: column;}
#event1 .char{max-width: 712px;width:100%;background: url(https://lwi.nexon.com/kartdrift/gow/pre/char_dizini.png) no-repeat;position: relative;background-size: contain;}
#event1 .char::after{display: block;width: 100%;padding-top: 101.686%;content: '';}
#event1 .char .msg{position: absolute;left:0;top:24%;width:31%;height: 23%;font-weight: 700;font-size: 1.5625rem;line-height: 2rem;color: #fff;display: flex;align-items:center;text-align: center;justify-content:center}
#event1 .char .name{position: absolute;right:19%;bottom:5.5%;width:15%;height: 15.6%;font-weight: 700;font-size: 1.563rem;line-height: 2rem;color: #9672FF;display: flex;align-items:center;text-align: center;justify-content:center;word-break: break-word;}
:lang(ko) #event1 .char .msg,
:lang(ko) #event1 .char .name{word-break: keep-all;}
#event1 .info h2{max-width: 351px;width:100%;background: url(https://lwi.nexon.com/kartdrift/gow/pre/tit_event.png) no-repeat;background-size: contain;text-indent: -100000px;}
:lang(zh) #event1 .info h2{background-image: url(https://lwi.nexon.com/kartdrift/gow/pre/tit_event_tw.png);max-width: 300px;}
:lang(en) #event1 .info h2{background-image: url(https://lwi.nexon.com/kartdrift/gow/pre/tit_event_en.png);max-width: 502px;}
:lang(th) #event1 .info h2{background-image: url(https://lwi.nexon.com/kartdrift/gow/pre/tit_event_th.png);max-width: 488px;}
#event1 .info h2::after{display: block;width: 100%;padding-top: 124.789%;content: '';}
:lang(en) #event1 .info h2::after,
:lang(th) #event1 .info h2::after{padding-top: 63%;}
#event1 .info .txt{font-weight: 700;font-size: 1.438rem;line-height: 2.063rem;color: #9D9FBF;}
.event .inner ul{margin-top: 20px;display: flex;flex-direction: column;width: 100%;}
.event .inner li{font-weight: 400;font-size: 1.125rem;line-height: 1.625rem;color: #FAFAFA;padding-left: 15px;}
.event .inner li::before{content: '-';margin-right: 10px;margin-left: -15px;}
.event .inner .app_download{width: 100%;display: flex;margin-top: 60px;max-width: 505px;}
#container #event2{flex-direction: column;padding:100px 10px 75px 0}
#container #event2 .inner{display: flex;align-items:center;flex-direction: column;background:url(https://lwi.nexon.com/kartdrift/gow/pre/character5.png) center 20% no-repeat;max-width: 1326px;width: 100%;height: 860px;justify-content:space-between}
:lang(en) #container #event2 .inner,
:lang(th) #container #event2 .inner{background-image:url(https://lwi.nexon.com/kartdrift/gow/pre/character6.png)}
#container #event2 h2{color: #A8A8A8;font-weight: 400;font-size: 1.563rem;line-height: 2.313rem;text-align: center;word-break: keep-all;width: 100%;}
#container #event2 h2 strong{display: block;font-size: 3.438rem;line-height: 5.063rem;color: #fff;}
#container #event2 .info{display: flex;flex-direction: column;align-items:center;width: 100%;}
#container #event2 .info .txt{font-size: 1.375rem;line-height: 2.063rem;color: #72CCFF;text-align: center;word-break: keep-all;width: 100%;}
#container #event2 .info ul li{text-align: center;word-break: keep-all;}

.select-hidden {display: none;visibility: hidden;}
.select {position: relative;cursor: pointer;display: inline-block;}
.select-styled{margin-bottom: 10px;font-family: 'Roboto';font-weight: 700;font-size: 2.188rem;line-height: 2.5rem;color: #000000;}
.select-styled:after {content: "";border-bottom: 10px solid transparent;border-top: 16px solid #000000;border-left: 10px solid transparent;border-right: 10px solid transparent;transform: rotate(0);display: inline-block;vertical-align: middle;transform-origin: center 30%;margin-left: 10px;}
.select-styled:active:after, .select-styled.active:after {transform: rotate(180deg);}
.custom_select .options {display: none;position: absolute;top:inherit;right: 0;left: 0;z-index: 999;margin: 0;padding: 0;color: #565656;border:3px solid #000;font-size: 1rem;background-color: #fff;width: 40%;}
.custom_select .options li {margin: 0;padding: 7px 0;text-align: center;transition: all 0.15s ease-in;}
.custom_select .options li:hover, .search .options li.is-selected {color: #009DDC;}
.custom_select .options li[rel="hide"] {display: none;}
#pre_wrapper header .floating_bn{display: none;}
#pre_wrapper > .floating_bn{position: fixed;left: 15px;bottom: 10%;width: 245px;height: 267px;background:url(https://lwi.nexon.com/kartdrift/gow/pre/banner.png) no-repeat;background-size: contain;z-index: 1000;}
.floating_bn a{display: block;width: 100%;height: 100%;text-indent: -100000px;}

.final #container > section{padding-top: 100px;}
.final #container .intro{background:url(https://lwi.nexon.com/kartdrift/gow/common/back.png) 50% 0 no-repeat;background-size: cover;}
.final #container .intro::after{background: rgba(0, 0, 0, 0.7);}
.mobile .final #container .intro{justify-content: flex-start;}
.final #container #event1{background:url(https://lwi.nexon.com/kartdrift/gow/final/bg_evt01.png) 50% 0 no-repeat;background-size: cover;min-height: 1176px;align-items: flex-start;}
.final #container #event1 .inner{flex-direction: column;text-align: center;}
.final #container #event1 h2{font-weight: 900;font-size: 3.75rem;line-height: 4.688rem;color: #3D3D3D;margin-bottom: 30px;word-break:keep-all}
.final #container #event1 p{font-size: 1.438rem;color: #3D3D3D;line-height: 2.063rem;margin-bottom:20px}
.final #container #event2{background:url(https://lwi.nexon.com/kartdrift/gow/common/bg_noise-wt.gif) 0 100% repeat-y;min-height: 1780px;justify-content: flex-start;max-height:fit-content}
.final #container #event2 .fire{position: absolute;top: 0;left: 50%;transform: translateX(-50%);overflow: hidden;width: 100%;height: 1003px;}
.final #container #event2 .fire::after{position: absolute;content:'';background: rgba(0, 0, 0, 0.3);width: 100%;height: 100%;top: 0;left: 0;right: 0;}
.final #container #event2 .fire #fire{width: 100%;height: 100%;object-fit: cover;object-position: center bottom;}
.final #container #event2 .inner{background: transparent;z-index: 1;justify-content:normal;height: auto;}
.final #container #event2 h2{background:url(https://lwi.nexon.com/kartdrift/gow/final/con2.png) no-repeat;max-width: 1065px;width: 100%;max-height: 1168px;background-size: contain;text-indent: -100000px;font-size: 0;margin-left: -100px;}
.final #container #event2 h2::after{padding-top: 109.6%;display: block;width: 100%;content: '';}
.final #container #event0 p.sharp,
.final #container #event1 p.sharp{position: relative;width: 100%;color: #fff;font-size: 1rem;padding:0 40px;text-align: center;line-height: 36px;background:url(https://lwi.nexon.com/kartdrift/gow/final/line.png), linear-gradient(90deg, rgba(29, 29, 29, 0) 0%, #1D1D1D 13.54%, #1D1D1D 86.46%, rgba(29, 29, 29, 0) 100%);border-radius: 10px;background-position:  50% 50%;height:100%;background-repeat: no-repeat;max-width: 980px;}
.final #container #event0 p.sharp{max-width: 762px;margin-top: 23px;margin-bottom: 15px;word-break: break-word;}
.final #container section p.sharp::before{content: '';width: 20px;height: 20px;background:url(https://lwi.nexon.com/kartdrift/gow/final/ico_sharp.png) no-repeat;background-size: contain;display: inline-block;vertical-align: middle;margin-right: 10px;margin-top: -2px;}
.final #container #event2 .info{border: 3px solid #000000;border-radius: 10px;margin-top: 70px;padding: 5px;max-width: 1268px;width:100%;}
.final #container #event2 .info ul{border: 1px dashed #000000;border-radius: 8px;width: 100%;height: 100%;margin-top: 0;padding: 20px;}
.final #container #event2 .info li{font-size: 0.938rem; line-height: 2.125rem;color: #686868;}
.final #container #event2 .info li a{font-weight: 700;color: #3162E1;display: inline-block;}
.final #container #event2 .info li::before{width: 3px;height: 3.5px;border-radius: 50%;background-color: #686868;display: inline-block;content: '';vertical-align: middle;margin-top: -4px;}
.final #container .intro .title h1{max-width: 990px;background: url(https://lwi.nexon.com/kartdrift/gow/final/title.png) center bottom no-repeat;background-size: contain;}
[lang]:not([lang=ko]) .final #container .intro .title h1 strong{display: block;font-weight: 800;font-size: 9rem;line-height: 9rem;color: #FFE600;}
[lang]:not([lang=ko]) .final #container .intro .title h1{background: transparent;max-width: inherit;text-indent: 0;text-align: center;font-family: 'Barlow Condensed';font-style: italic;font-weight: 700;font-size:5.625rem;line-height: 5.625rem;color: #FFFFFF;word-break: keep-all;}
[lang]:not([lang=ko]) .final #container .intro .title h1::after{padding-top: 0;}
.final #container .intro .title h1::after{padding-top: 17.307%;}
.final #container .intro .title .desc{font-size: 1.5rem;color: #3D3D3D;line-height: 2.063rem;color: #fff;font-weight: 500;margin-bottom: 20px;word-break: break-word;}
.final #container .intro .title .desc::before,
.final #container .intro .title .desc::after{content: '';width: 48.8px;height: 22px;display: inline-block;vertical-align: middle;}
.final #container .intro .title .desc::before{background: url(https://lwi.nexon.com/kartdrift/gow/final/ico_obj1.svg) no-repeat;margin-right: 5px;}
.final #container .intro .title .desc::after{background: url(https://lwi.nexon.com/kartdrift/gow/final/ico_obj2.svg) no-repeat;margin-left: 5px;}
.final #container .intro .title ul{max-width: 762px;width:100%;padding: 15px 0px;border-top: 1px solid rgba(255, 255, 255, .3);border-bottom: 1px solid rgba(255, 255, 255, .3);text-align: center;margin-top: 20px;}
.final #container .intro .title li{font-size: 1.5rem;line-height: 2.5rem;color: #fff;word-break: break-word;}
.final #container .intro .title li strong{font-weight: 500;color:#FFE600;}
:lang(ko) .modal_wrap h2,
:lang(ko) .modal_wrap p,
:lang(ko) .table table th,
:lang(ko) .table table td,
:lang(ko) #popCheck .tab button,
:lang(ko) #container .preForm .tit,
:lang(ko) #container .preForm .noti,
:lang(ko) .final #container section .inner{letter-spacing: -0.03em;}


@media all and (max-width: 1250px){
    #container .preForm::before{display: none;}
    #container .preForm{border-top: 5px solid #FFFFFF;padding-top: 20px;}
    #container .registration{padding-top: 130px;}
    .final #container .intro .box{width: 90%;}
    
}
@media all and (max-width: 1200px){
    #pre_wrapper #container::after{display: none;}
    #container #event2 .inner{background-size: contain;}
    .final #container #event2{min-height: auto;padding-bottom:120px}
    .final #container #event2 h2{margin-left: -30px;}
    
}
@media all and (max-width: 1100px){
    .final #container #event2 .fire{height: auto;}
    .final #container #event2 .fire #fire{width: 235%;}
    .final #container #event2 .info{margin-top: 30px;}
    
}
@media all and (max-width: 940px){
    .final #container .intro{justify-content: flex-start;padding-top: 150px;}
    
}

@media all and (max-width: 860px) {
    #container .registration,
    #container > section{padding:80px 20px 50px 20px;max-height: inherit;}
    #container .preForm{flex-direction: column;border:0;padding: 0;align-items: center;}
    #container .preForm::after,
    #container .preForm .tit h2::after{display: none;}
    #container .preForm .tit{width: 100%;padding:0 0 20px 5px;}
    .app_download a{margin-bottom: 5px;}
    .event .inner .app_download{justify-content: center;margin-top: 30px;}
    #container #event1 .inner{flex-direction: column;}
    #event1 .info{max-width: 100%;margin-top: 20px;align-items: center;order: 1}
    #event1 .char{order: 2;width: 70%;}
    #event1 .info h2{width: 43%;}
    #container .intro .title .desc_pre{padding:4px 30px;}
    #container #event2 .inner::after{display: block;width: 100%;padding-top: 64.857%;content: '';}
    .final #container #event2 .inner::after{display: none;}
    #container #event2 .inner{height: auto;background-position-y: 95%;}
    #container .intro .platform ul{flex-wrap:wrap;width: 95%;margin-left: 0;} 
    #container .intro .platform .btn_check{max-width:100% !important;flex-basis:100% !important;margin: 0;margin-top: 25px;}
    #container .intro .platform{bottom: 40px;padding: 0 10px;}
    #event1 .char .msg,
    #event1 .char .name{font-size: 1rem;line-height: 1.1rem;}
    #pre_wrapper header.sidebar .floating_bn{display: block;width: 100%;height: 110px;background:#0997FF url(https://lwi.nexon.com/kartdrift/gow/pre/banner_m.png) center center no-repeat;background-size: contain;margin-bottom: 34px;}
    #pre_wrapper > .floating_bn{display: none;}
    #popCheck .tab{height: 42px;}
    [lang]:not([lang=ko]) .final #container .intro .title h1{font-size: 4rem;line-height: 4rem;}
    [lang]:not([lang=ko]) .final #container .intro .title h1 strong{font-size: 4rem;line-height: 4rem;}
    .final #container .intro .txt2{width:95%}
}
@media all and (max-height:700px) {
    .mobile .final #container .intro{min-height: 900px !important;}    
}
@media all and (max-height:635px) {
    .mobile #container .intro{min-height: 700px !important;}    
}
@media all and (max-width:640px) {
    u{display: block;}
    #popCheck .table{flex-direction: column;}
    #container .preForm .noti h3,
    #container .preForm .input_info,
    #container .preForm .txt_info,
    #container .preForm .agree,
    #container .preForm .noti_list{padding-left: 20px;padding-right:20px;}
    #container .intro .title h1{max-width: 70vw;}
    #container .intro .title button{width: 100vw;margin:20px 0 0;height: auto;font-size: 1.6rem;}
    #pre_wrapper #footer{position: absolute;border-top: 0;}
    #pre_wrapper #footer .scroll_down{display: none;}
    #pre_wrapper #container{padding-bottom: 100px;}
    #pre_wrapper.final #container{padding-bottom: 0;}
    #pre_wrapper footer{bottom: 55px;max-width:90%;height: auto;padding: 0 10px;}
    #pre_wrapper #footer .btn_top{display: block;top: auto;right: 10px;bottom: 10px;width: 40px;height: 39px;background:url(https://lwi.nexon.com/kartdrift/gow/common/btn_top.png) no-repeat;background-size: contain;}
    #pre_wrapper #footer .btn_top::before,
    #pre_wrapper #footer .btn_top::after{display: none;}
    #container .intro .platform li{margin-left:5px;margin-bottom: 5px;}
    #container .intro .title button::after{width: 28px;height: 12px;margin-top: -4px;}
    #container .preForm .tit h2::before{width: 124px;height: 45px;margin-bottom:0}
    .final #container #event1 h2{font-size: 2.5rem;line-height: 3rem;}
    .final #container #event1 p{font-size: 1.3rem;line-height: 2rem;}
    .final #container #event0 p.sharp, .final #container #event1 p.sharp{font-size: 12px;line-height: 1rem;padding: 5px 10px;background-size: contain;}
    .final #container #event1{min-height: 620px;}
    #container .intro .platform{bottom: 20px;}
    .final #container .intro .box{width: 100%;border:0;border-radius: 0;bottom:0}
    .final #container .intro .line{border:0;}
    .final #container .intro .txt1{border:0;margin-bottom: 0;}
    .all #container .intro .platform .btn_check{margin-top: 5px;}
    .all #container .intro .platform{padding:0}
    .all #container .intro .platform ul,
    .final #container .intro .txt2{width: 100%;}
    .final #container .intro .txt1::before{display: block;width: 100%;margin:0 0 5px 0}
    .final #container #event1{background: url(https://lwi.nexon.com/kartdrift/gow/final/bg_evt01_m.jpg) 50% 0 no-repeat;background-size: cover;}
}
@media screen and (max-width: 920px) and (orientation: landscape) {
	.mobile #container .intro{min-height: 620px !important;}
    #container .intro .title h1{max-width: 50vw;}
    #container .intro .title button{width: 60vw;margin: 20px 0 0;}
    #container .intro .platform{bottom: 20px;}
