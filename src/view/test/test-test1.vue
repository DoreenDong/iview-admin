<template>
  <div>
      <!-- 自定义顶栏弹窗 -->
    <Button type="primary" @click="modal1 = true">自定义顶栏弹窗</Button>
    <Modal
        v-model="modal1"
        title="自定义顶栏"
        @on-ok="ok"
        @on-cancel="cancel">
        <CheckboxGroup v-model="social">
        <Row>
            <Col span="8" style="padding-bottom:20px">
                <Checkbox label="twitter">
                    <img src="../../assets/images/logo-min.jpg" alt="111" style="vertical-align:middle;margin:0px 10px"><span>吾享云端</span>
                </Checkbox>
            </Col>
            <Col span="8" style="padding-bottom:20px">
                <Checkbox label="facebook">
                    <img src="../../assets/images/logo-min.jpg" alt="111" style="vertical-align:middle;margin:0px 10px"><span>吾享云端</span>
                </Checkbox>
            </Col>
            <Col span="8" style="padding-bottom:20px">
                <Checkbox label="github">
                    <img src="../../assets/images/logo-min.jpg" alt="111" style="vertical-align:middle;margin:0px 10px"><span>吾享云端</span>
                </Checkbox>
            </Col>
        </Row>
        <Row>
            <Col span="8" style="padding-bottom:20px">
                <Checkbox label="snapchat">
                   <img src="../../assets/images/logo-min.jpg" alt="111" style="vertical-align:middle;margin:0px 10px"><span>吾享云端</span>
                </Checkbox>
            </Col>
            <Col span="8" style="padding-bottom:20px">
                <Checkbox label="snapcha">
                    <img src="../../assets/images/logo-min.jpg" alt="111" style="vertical-align:middle;margin:0px 10px"><span>吾享云端</span>
                </Checkbox>
            </Col>
            <Col span="8" style="padding-bottom:20px">
                <Checkbox label="snapch">
                    <img src="../../assets/images/logo-min.jpg" alt="111" style="vertical-align:middle;margin:0px 10px"><span>吾享云端</span>
                </Checkbox>
            </Col>
        </Row>
         <Row>
            <Col span="8" style="padding-bottom:20px">
                <Checkbox label="snapc">
                    <img src="../../assets/images/logo-min.jpg" alt="111" style="vertical-align:middle;margin:0px 10px"><span>吾享云端</span>
                </Checkbox>
            </Col>
            <Col span="8" style="padding-bottom:20px">
                <Checkbox label="snap">
                    <img src="../../assets/images/logo-min.jpg" alt="111" style="vertical-align:middle;margin:0px 10px"><span>吾享云端</span>
                </Checkbox>
            </Col>
            <Col span="8" style="padding-bottom:20px">
                <Checkbox label="sna">
                    <img src="../../assets/images/logo-min.jpg" alt="111" style="vertical-align:middle;margin:0px 10px"><span>吾享云端</span>
                </Checkbox>
            </Col>
        </Row>
    </CheckboxGroup>
    </Modal>
  </div>
</template>
<script>
export default {
  data () {
    return {
      modal1: false,
      social: [],
      value: ''
    }
  },
  methods: {
    ok () {
      this.$Message.info('Clicked ok')
    },
    cancel () {
      this.$Message.info('Clicked cancel')
    }
  }
}
</script>
<style>
img {
    height: 40px;
    width: 40px;
}
</style>
