<template>
    <div id="aaa">
        <!-- <img src="../../assets/images/talkingdata.png"> -->
        <div class="outer">
          <Row type="flex" justify="center" align="middle" class="code-row-bg">
            <div class="inner">
                <Row>
                    <Col span="12" offset="8" style="padding-top:20px;color:#fff;font-size:16px">
                        <p>商龙云商户平台</p>
                    </Col>
                    <Col span="18" offset="5" style="padding-top:30px">
                        <input icon="ios-contact" placeholder="请输入绑定手机号" style="color:#fff" />
                    </Col>
                    <Col span="18" offset="5" style="padding-top:20px">
                        <input icon="md-lock" placeholder="请输入密码" style="color:#fff" />
                    </Col>
                    <Col span="8" offset="16" style="padding-top:20px;">
                        <a href="" style="color:#FE8C00;">忘记密码</a>
                    </Col>
                    <Col span="18" offset="3" style="padding-top:20px;">
                        <Button type="warning" long>登录</Button>
                    </Col>
                </Row>
            </div>
          </Row>
        </div>
        <Button type="primary" @click="modal2 = true">修改登录密码弹窗</Button>
    <Modal
        v-model="modal2"
        title="修改登录密码"
        @on-ok="ok"
        @on-cancel="cancel">
        <Row>
            <p>修改密码时需要输入当前密码，如果你忘记了当前密码，您可以尝试<a href="">重置密码</a></p>
            <Col span="18" offset="5" style="padding-top:20px">
                <Input v-model="value" placeholder="请输入原登录密码" style="width: 300px" />
            </Col>
            <Col span="18" offset="5" style="padding-top:20px">
                <Input v-model="value" placeholder="请输入新密码" style="width: 300px" />
            </Col>
            <Col span="18" offset="5" style="padding-top:20px">
                <Input v-model="value" placeholder="请再输入一次新密码" style="width: 300px" />
            </Col>
        </Row>
    </Modal>
    </div>
</template>
<script>
export default {
  name: 'test_test_2',
  data () {
    return {
      modal2: false,
      value: ''
    }
  }
}
</script>
<style>
    #aaa {
      width: 1150px;
      height: 700px;
      background:url('../../assets/images/login-bg.jpg');
      background-size: 100% 100%;
      background-repeat: no-repeat;
    }
    .inner {
      /* background:url('../../assets/images/talkingdata.png'); */
      /* background-repeat:no-repeat; */
      margin-top: 15%;
      background-color: rgba(56, 56, 56, 0.3);
      position: absolute;
      width:267px;
      height:290px;
    }
    input {
      border:none;
      border-bottom:1px solid #FE8C00;
      outline: none;
      background-color:rgba(0,0,0,0);
      color:#eee
    }
</style>
