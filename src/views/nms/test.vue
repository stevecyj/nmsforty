<template>
  <div>
    <!-- <a-breadcrumb separator="">
      <a-breadcrumb-item>Location</a-breadcrumb-item>
      <a-breadcrumb-separator>:</a-breadcrumb-separator>
      <a-breadcrumb-item href="">
        Application Center
      </a-breadcrumb-item>
      <a-breadcrumb-separator />
      <a-breadcrumb-item href="">
        Application List
      </a-breadcrumb-item>
      <a-breadcrumb-separator />
      <a-breadcrumb-item>An Application</a-breadcrumb-item>
    </a-breadcrumb> -->
    <a-page-header
      style="border: 1px solid rgb(235, 237, 240)"
      title="Title"
      sub-title="This is a subtitle"
      @back="() => null"
    />

    <a-select
      label-in-value
      :default-value="{ key: 'lucy' }"
      style="width: 120px"
      @change="handleChange"
    >
      <a-select-option value="jack">
        Jack (100)
      </a-select-option>
      <a-select-option value="lucy">
        Lucy (101)
      </a-select-option>
    </a-select>
  </div>
</template>

  <!-- <div>
    <h2>this is test page</h2>
  </div> -->
</template>

<script>
export default {
  methods: {
    handleChange(value) {
      console.log(value) // { key: "lucy", label: "Lucy (101)" }
    }
  }
}
</script>

<style lang="less" scoped>
@import '~ant-design-vue/lib/style/themes/default.less';
h2 {
  color: goldenrod;
  font-size: 26px;
}
</style>
