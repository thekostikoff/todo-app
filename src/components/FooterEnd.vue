<template>
  <div :class="$style.buttons">
    <div :class="$style.oneofthird">1/3 left</div>
    <div :class="$style.info">
      <ButtonsInfo />
    </div>
  </div>
</template>

<script>
import ButtonsInfo from "@/components/ButtonsInfo.vue";
export default {
  components: {
    ButtonsInfo,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss" module>
.buttons {
  display: flex;
  flex-direction: row;
  align-items: self-start;
  justify-content: center;
  gap: 180px;
  max-width: 540px;
  background: #ffca93;
  font-family: "Open Sans";
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  color: #c9955d;
  line-height: 28px;
  padding: 11px 22px;
  .oneofthird {
    font-family: "Open Sans";
    padding-left: 10px;
    min-width: 100px;
  }
  .info {
    display: flex;
    flex-direction: row;
  }
  .info button:hover {
    border: 1px solid #c9955d;
    border-radius: 10px;
    cursor: pointer;
  }
}
</style>
