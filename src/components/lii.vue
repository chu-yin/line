<template>
  <input type="hidden" id="_csrf" value="df2de973-bb61-4567-a4b7-ed8cf12c2b19" />
  <input type="hidden" id="contextPath" value="/portal" />
  <input type="hidden" id="nationCode" value="tw" />
  <input type="hidden" id="loginResult" value="" />

  <div class="wrap twlogin">
    <section class="container login">
      <h1 class="logo_login"><img src="https://d.line-scdn.net/linepay/portal/v-230403/portal/assets/img/portal/login-logo-pay.svg?dm=1681885798399" alt="LINE pay"></h1>
      <ul class="login_tab">
        <li id="twTabLine" class="line on">
          <a href="#" class="tab">以商店ID登入</a>
        </li>
      </ul>
      <div id="twLineArea" class="login_line" style="display: block;">
        <p class="noti_tit">我目前只有使用LINE Pay綁定信用卡及LINE POINTS收款服務</p>
        <div class="flex-container">
          <div>·我想確認信用卡及LINE POINTS的帳款資訊</div>
          <div>·我要登入Agency ID或是Group ID</div>

          <div id="allDivWrapper" class="inp">
            <div id="idDivWrapper" class="inp_unit form_id">
              <label for="id" class="form_label" style="display: none;">商店ID</label>
              <div class="input_wrap">
                <div id="inputBox" class="input_box" style="display: inline-block;">
                  <label for="id" class="form_label">商店ID</label>
                  <input type="text" id="id">
                </div>
                <span id="idCloneArea" class="input_clone"></span>
              </div>
            </div>

            <label for="password" class="form_label">密碼</label>
            <input type="password" id="password">
          </div>
          <button  id="loginActionButton" class="btn_login" >登入</button>
        </div>
      </div>
      <div class="login_bottom">
        <div class="login_rel">
          <a href="/portal/tw/auth/find/id" class="login_lk">忘記商店ID</a>
          <a href="/portal/tw/auth/reset/passwd" class="login_lk">重設密碼</a>
        </div>
        <p class="login_noti">如果您是管理者，請使用LINE帳號登入</p>
        <button type="button" class="btn_line_login linkButton">以LINE帳號登入</button>
      </div>
  </div>
  </section>
  </div>
  <div id="loginAccessErrorLayerPop" class="ly_pop">
    <div class="ly_cont">
      <p class="tit"><em>重新設置密碼</em></p>
      <p class="txt">如果您是管理者，請使用LINE帳號登入</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "lii"
}
</script>

<style scoped>
input::placeholder { color: gray; }

.flex-container {
  display: flex;
  flex-direction: column;
  color:gray;
}

</style>