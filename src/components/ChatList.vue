<template>
  <div>
    <form class="chatList">
      <div class="chatListChild" />
      <div class="chatEntry">
        <div class="contactDetails">
          <div class="profileInfo">
            <div class="frameParent">
              <div class="whyDoWeNeedAWalletParent">
                <img
                  class="whyDoWeNeedAWallet"
                  loading="lazy"
                  alt="anil"
                  src="/Friends/ellipse-11@2x.png"
                />
                <div class="frameWrapper">
                  <div class="anilParent">
                    <h1 class="anil">Anil</h1>
                    <div class="onlineLast">
                      Online - Last seen, 2.02pm
                    </div>
                  </div>
                </div>
              </div>
              <div class="moreOptions">
                <img
                  class="bithreeDotsVerticalIcon"
                  loading="lazy"
                  alt=""
                  src="/Friends/bithreedotsvertical.svg"
                />
              </div>
            </div>
          </div>
          <div class="separator" />
        </div>
      </div>
      <div class="messagePreview">
        <div class="messageContainerParent">
          <div class="messageContainer">
            <div class="rectangleParent">
              <div class="frameChild" />
              <div class="heyThere">Hey There!</div>
            </div>
          </div>
          <div class="rectangleGroup">
            <div class="frameItem" />
            <h2 class="howAreYou">How are you?</h2>
          </div>
        </div>
      </div>
      <div class="chatMessages">
        <div class="sentMessageContainerParent">
          <div class="sentMessageContainer">
            <div class="messageContent">
              <div class="messageBackground" />
              <h2 class="hello">Hello!</h2>
            </div>
            <div class="today833pmWrapper">
              <div class="today833pm">Today, 8.33pm</div>
            </div>
          </div>
      
        </div>
      </div>
    
      <div class="inputContainerParent">
        <div class="inputContainer">
          <div class="rectangleContainer">
            <div class="frameInner" />
            <div class="antDesignpaperClipOutlinedParent">
              <img
                class="antDesignpaperClipOutlinedIcon"
                loading="lazy"
                alt=""
                src="/Friends/antdesignpaperclipoutlined.svg"
              />
              <div class="typeYourMessageHereWrapper">
                <h3 class="typeYourMessage">Type your message here...</h3>
              </div>
            </div>
            <div class="fluentemojiLaugh16RegularParent">
              <img
                class="fluentemojiLaugh16RegularIcon"
                loading="lazy"
                alt=""
                src="/Friends/fluentemojilaugh16regular.svg"
              />
              <div class="fluentcamera24RegularWrapper">
                <img
                  class="fluentcamera24RegularIcon"
                  loading="lazy"
                  alt=""
                  src="/Friends/fluentcamera24regular.svg"
                />
              </div>
            </div>
          </div>
        </div>
        <div class="frameDiv">
          <div class="rectangleDiv" />
          <img class="bimicFillIcon" alt="" src="/Friends/bimicfill.svg" />
        </div>
      </div>
    </form>
  </div>
  </template>
  
  <script>
    import { defineComponent } from "vue";
  
    export default defineComponent({
      name: "ChatList",
    });
  </script>
  
  <style scoped>
    /* Your scoped styles here */
    /* .chatListChild, .chatEntry, .contactDetails, .profileInfo, and so on... */
    .chatListChild {
      width: 952px;
      height: 1010px;
      position: relative;
      border-radius: var(--br-6xl);
      background-color: var(--color-white);
      box-shadow: 0px 4px 5px 2px rgba(121, 197, 239, 0.38);
      display: none;
      max-width: 100%;
    }
    .whyDoWeNeedAWallet {
      height: 50px;
      width: 50px;
      position: relative;
      border-radius: 50%;
      object-fit: cover;
      z-index: 3;
    }
    .anil {
      margin: 0;
      width: 90px;
      position: relative;
      font-size: var(--font-size-1xl);
      letter-spacing: 0.05em;
      font-weight: 600;
      font-family: var(--font-roboto);
      color: var(--color-darkslategray);
      text-align: left;
      display: inline-block;
      z-index: 3;
    }
    .onlineLast {
      align-self: stretch;
      position: relative;
      font-size: var(--font-size-lg);
      letter-spacing: 0.05em;
      font-weight: 300;
      font-family: var(--font-roboto);
      color: var(--color-darkslategray);
      text-align: left;
      z-index: 3;
    }
    .anilParent {
      align-self: stretch;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      gap: var(--gap-12xs);
    }
    .frameWrapper {
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-end;
      padding: 0px 0px var(--padding-9xs);
      box-sizing: border-box;
      min-width: 226px;
      max-width: 100%;
    }
    .whyDoWeNeedAWalletParent {
      width: 447px;
      display: flex;
      flex-direction: row;
      align-items: flex-end;
      justify-content: flex-start;
      gap: var(--gap-6xl);
      max-width: 100%;
    }
    .bithreeDotsVerticalIcon {
      width: 40px;
      height: 40px;
      position: relative;
      z-index: 3;
    }
    .moreOptions {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-end;
      padding: 0px 0px var(--padding-mid);
    }
    .frameParent {
      flex: 1;
      display: flex;
      flex-direction: row;
      align-items: flex-end;
      justify-content: space-between;
      max-width: 100%;
      gap: var(--gap-xl);
    }
    .profileInfo {
      align-self: stretch;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      padding: 0px 0px 0px var(--padding-9xs);
      box-sizing: border-box;
      max-width: 100%;
    }
    .separator {
      width: 876px;
      height: 1px;
      position: relative;
      border-top: 1px solid var(--color-darkgray);
      box-sizing: border-box;
      max-width: 100%;
      z-index: 3;
    }
    .contactDetails {
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      gap: var(--gap-xl-5);
      max-width: 100%;
    }
    .chatEntry {
      align-self: stretch;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      padding: 0px 0px 0px var(--padding-7xs);
      box-sizing: border-box;
      max-width: 100%;
    }
    .frameChild {
      height: 59px;
      width: 221px;
      position: relative;
      border-radius: var(--br-6xl);
      background-color: var(--color-gainsboro);
      display: none;
    }
    .heyThere {
      width: 152px;
      position: relative;
      font-size: var(--font-size-7xl);
      letter-spacing: 0.05em;
      font-family: var(--font-roboto);
      color: var(--color-darkslategray);
      text-align: left;
      display: inline-block;
      flex-shrink: 0;
      z-index: 4;
    }
    .rectangleParent {
      flex: 1;
      border-radius: var(--br-6xl);
      background-color: var(--color-gainsboro);
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-end;
      padding: var(--padding-sm) var(--padding-9xl);
      white-space: nowrap;
      z-index: 3;
    }
    .messageContainer {
      width: 225px;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      padding: 0px var(--padding-11xs);
      box-sizing: border-box;
    }
    .frameItem {
      height: 59px;
      width: 267px;
      position: relative;
      border-radius: var(--br-6xl);
      background-color: var(--color-gainsboro);
      display: none;
    }
    .howAreYou {
      margin: 0;
      width: 209px;
      position: relative;
      font-size: var(--font-size-7xl);
      letter-spacing: 0.05em;
      font-weight: 400;
      font-family: var(--font-roboto);
      color: var(--color-darkslategray);
      text-align: left;
      display: inline-block;
      flex-shrink: 0;
      z-index: 4;
    }
    .rectangleGroup {
      align-self: stretch;
      border-radius: var(--br-6xl);
      background-color: var(--color-gainsboro);
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-end;
      padding: var(--padding-sm) var(--padding-mid);
      white-space: nowrap;
      z-index: 3;
    }
    .messageContainerParent {
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      gap: var(--gap-4xl);
    }
    .messagePreview {
      width: 307px;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      padding: 0px var(--padding-xl) var(--padding-10xl-5);
      box-sizing: border-box;
    }
    .messageBackground {
      position: absolute;
      width: calc(100% - 4px);
      top: 0px;
      right: 4px;
      left: 0px;
      border-radius: var(--br-6xl);
      background-color: var(--color-blue);
      height: 59px;
      z-index: 3;
    }
    .hello {
      margin: 0;
      position: absolute;
      top: 15px;
      left: 53px;
      font-size: var(--font-size-7xl);
      letter-spacing: 0.05em;
      font-weight: 400;
      font-family: var(--font-roboto);
      color: var(--color-white);
      text-align: left;
      display: inline-block;
      width: 132px;
      height: 31px;
      z-index: 4;
    }
    .messageContent {
      width: 185px;
      height: 59px;
      position: relative;
    }
    .today833pm {
      flex: 1;
      position: relative;
      font-size: var(--font-size-xl);
      letter-spacing: 0.05em;
      font-weight: 300;
      font-family: var(--font-roboto);
      color: var(--color-dimgray);
      text-align: left;
      z-index: 3;
    }
    .today833pmWrapper {
      align-self: stretch;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      padding: 0px 0px 0px var(--padding-lg);
    }
    .sentMessageContainer {
      width: 189px;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      gap: var(--gap-5xs);
    }
    .receivedBackground {
      align-self: stretch;
      flex: 1;
      position: relative;
      border-radius: var(--br-6xl);
      background-color: var(--color-blue);
      z-index: 3;
    }
    .today834pm {
      width: 171px;
      position: relative;
      font-size: var(--font-size-xl);
      letter-spacing: 0.05em;
      font-weight: 300;
      font-family: var(--font-roboto);
      color: var(--color-dimgray);
      text-align: left;
      display: inline-block;
      flex-shrink: 0;
      z-index: 3;
    }
    .today834pmWrapper {
      align-self: stretch;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-end;
    }
    .receivedBackgroundParent {
      align-self: stretch;
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      gap: var(--gap-5xs);
    }
    .sentMessageContainerParent {
      align-self: stretch;
      width: 437px;
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      justify-content: flex-start;
      gap: var(--gap-12xl);
      max-width: 100%;
    }
    .chatMessages {
      align-self: stretch;
      height: 233.5px;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-end;
      padding: 0px var(--padding-8xl) var(--padding-base-5);
      box-sizing: border-box;
      max-width: 100%;
    }
    .messageLongBackground {
      position: absolute;
      top: 0px;
      left: 0px;
      border-radius: var(--br-6xl);
      background-color: var(--color-gainsboro);
      width: 100%;
      height: 100%;
      z-index: 3;
    }
    .iAmDoing {
      position: absolute;
      top: 12.6px;
      left: 41px;
      font-size: var(--font-size-7xl);
      letter-spacing: 0.05em;
      font-family: var(--font-roboto);
      color: var(--color-darkslategray);
      text-align: left;
      display: inline-block;
      width: 550px;
      height: 31px;
      z-index: 4;
    }
    .messageLongBackgroundParent {
      align-self: stretch;
      height: 53px;
      position: relative;
    }
    .today836pm {
      flex: 1;
      position: relative;
      font-size: var(--font-size-xl);
      letter-spacing: 0.05em;
      font-weight: 300;
      font-family: var(--font-roboto);
      color: var(--color-dimgray);
      text-align: left;
      z-index: 3;
    }
    .today836pmWrapper {
      width: 213px;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      padding: 0px var(--padding-2xl);
      box-sizing: border-box;
    }
    .frameGroup {
      width: 591px;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      gap: var(--gap-4xs);
      max-width: 100%;
    }
    .longMessageContainerInner {
      align-self: stretch;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      max-width: 100%;
    }
    .responseContainerChild {
      height: 59px;
      width: 201px;
      position: relative;
      border-radius: var(--br-6xl);
      background-color: var(--color-blue);
      display: none;
    }
    .yesSure {
      width: 139px;
      position: relative;
      font-size: var(--font-size-7xl);
      letter-spacing: 0.05em;
      font-family: var(--font-roboto);
      color: var(--color-white);
      text-align: left;
      display: inline-block;
      flex-shrink: 0;
      z-index: 4;
    }
    .responseContainer {
      width: 201px;
      border-radius: var(--br-6xl);
      background-color: var(--color-blue);
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-end;
      padding: var(--padding-sm) var(--padding-xs);
      box-sizing: border-box;
      white-space: nowrap;
      z-index: 3;
    }
    .today858pm {
      flex: 1;
      position: relative;
      font-size: var(--font-size-xl);
      letter-spacing: 0.05em;
      font-weight: 300;
      font-family: var(--font-roboto);
      color: var(--color-dimgray);
      text-align: left;
      z-index: 3;
    }
    .today858pmWrapper {
      align-self: stretch;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      padding: 0px 0px 0px var(--padding-19xl);
    }
    .responseContainerParent {
      width: 209px;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      gap: var(--gap-5xs);
    }
    .longMessageContainer {
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      justify-content: flex-start;
      gap: var(--gap-2xl);
      max-width: 100%;
    }
    .longMessageContainerWrapper {
      align-self: stretch;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      padding: 0px var(--padding-8xl) var(--padding-sm-5) var(--padding-xl);
      box-sizing: border-box;
      max-width: 100%;
    }
    .frameInner {
      height: 79px;
      width: 783px;
      position: relative;
      border-radius: var(--br-6xl);
      background-color: var(--color-aliceblue);
      display: none;
      max-width: 100%;
    }
    .antDesignpaperClipOutlinedIcon {
      height: 42px;
      width: 42px;
      position: relative;
      z-index: 4;
    }
    .typeYourMessage {
      margin: 0;
      align-self: stretch;
      position: relative;
      font-size: var(--font-size-5xl);
      letter-spacing: 0.05em;
      line-height: 26px;
      font-weight: 300;
      font-family: var(--font-roboto);
      color: var(--color-darkslategray);
      text-align: left;
      z-index: 4;
    }
    .typeYourMessageHereWrapper {
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      padding: var(--padding-6xs) 0px 0px;
      box-sizing: border-box;
      min-width: 226px;
      max-width: 100%;
    }
    .antDesignpaperClipOutlinedParent {
      width: 420px;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      gap: var(--gap-12xl);
      max-width: 100%;
    }
    .fluentemojiLaugh16RegularIcon {
      height: 43px;
      width: 43px;
      position: relative;
      min-height: 43px;
      z-index: 4;
    }
    .fluentcamera24RegularIcon {
      width: 38px;
      height: 38px;
      position: relative;
      z-index: 4;
    }
    .fluentcamera24RegularWrapper {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      padding: var(--padding-11xs) 0px 0px;
    }
    .fluentemojiLaugh16RegularParent {
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      gap: var(--gap-6xl);
    }
    .rectangleContainer {
      align-self: stretch;
      border-radius: var(--br-6xl);
      background-color: var(--color-aliceblue);
      display: flex;
      flex-direction: row;
      align-items: flex-end;
      justify-content: space-between;
      padding: var(--padding-lgi) var(--padding-4xl) var(--padding-mid)
        var(--padding-3xl);
      box-sizing: border-box;
      max-width: 100%;
      gap: var(--gap-xl);
      z-index: 3;
    }
    .inputContainer {
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      padding: var(--padding-11xs) 0px 0px;
      box-sizing: border-box;
      max-width: 100%;
    }
    .rectangleDiv {
      height: 78px;
      width: 78px;
      position: relative;
      border-radius: var(--br-xl);
      background-color: var(--color-blue);
      display: none;
    }
    .bimicFillIcon {
      height: 38px;
      width: 38px;
      position: relative;
      z-index: 4;
    }
    .frameDiv {
      border-radius: var(--br-xl);
      background-color: var(--color-blue);
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: flex-start;
      padding: var(--padding-xl) var(--padding-lg) var(--padding-xl)
        var(--padding-3xl);
      z-index: 3;
    }
    .inputContainerParent {
      align-self: stretch;
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      align-items: flex-start;
      justify-content: flex-start;
      gap: var(--gap-5xl);
      max-width: 100%;
    }
    .chatList {
      margin: 0;
      position: absolute;
      top: 15px;
      left: 780px;
      border-radius: var(--br-6xl);
      background-color: var(--color-white);
      box-shadow: 0px 4px 5px 2px rgba(121, 197, 239, 0.38);
      width: 800px;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      padding: var(--padding-10xl) var(--padding-4xl) var(--padding-11xl)
        var(--padding-15xl);
      box-sizing: border-box;
      gap: var(--gap-19xl-5);
      max-width: 100%;
      z-index: 2;
    }
  
    @media screen and (max-width: 750px) {
      .anil {
        font-size: var(--font-size-7xl);
      }
    }
    @media screen and (max-width: 675px) {
      .frameParent {
        flex-wrap: wrap;
      }
  
      .rectangleContainer {
        flex-wrap: wrap;
      }
  
      .inputContainer {
        min-width: 100%;
      }
    }
    @media screen and (max-width: 450px) {
      .anil {
        font-size: var(--font-size-lgi);
      }
  
      .onlineLast {
        font-size: var(--font-size-base);
      }
  
      .whyDoWeNeedAWalletParent {
        flex-wrap: wrap;
      }
  
      .hello {
        font-size: var(--font-size-2xl);
      }
  
      .today833pm {
        font-size: var(--font-size-base);
      }
  
      .today834pm {
        font-size: var(--font-size-base);
      }
  
      .iAmDoing {
        font-size: var(--font-size-2xl);
      }
  
      .today836pm {
        font-size: var(--font-size-base);
      }
  
      .today858pm {
        font-size: var(--font-size-base);
      }
  
      .typeYourMessage {
        font-size: var(--font-size-lgi);
        line-height: 21px;
      }
  
      .antDesignpaperClipOutlinedParent {
        flex-wrap: wrap;
      }
    }
  </style>
  