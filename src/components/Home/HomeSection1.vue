<template>
  <div class="Section1 mt-3">
    <div class="outer">
      <div class="form-check form-switch">
        <label class="switch">
          <input type="checkbox" checked />
          <span class="slider round"></span>
        </label>
      </div>
    </div>
    <div class="row">
      <div class="col-12 col-lg-7 d-flex fst">
        <img src="../../assets/home/Rectangle91.png" alt="Rectangle" />
        <img src="../../assets/home/Rectangle85.png" alt="Rectangle" />
      </div>
      <div class="col-12 col-lg-5 d-flex flex-wrap sec">
        <img src="../../assets/home/Rectangle89.png" alt="Rectangle" />
        <img src="../../assets/home/Rectangle52.png" alt="Rectangle" />
        <img src="../../assets/home/Rectangle90.png" alt="Rectangle" />
        <img src="../../assets/home/Rectangle88.png" alt="Rectangle" />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "HomeSection1",
};
</script>
<style lang="scss" scoped>
.Section1 {
  position: relative;
}

.fst {
  padding-left: 0%;
}
.sec {
  padding-right: 1%;
}
.fst img:first-of-type {
  height: 330px;
  width: 30%;
  margin-left: 13px;
}
.fst img:last-of-type {
  height: 330px;
  width: calc(70% - 13px);
}
.sec img {
  width: 48%;
  margin-bottom: 13px;
}
img {
  transition: all 0.3s linear;
}
img:hover {
  transform: translateY(-5px);
  opacity: 0.9;
}
.sec img:nth-of-type(1),
.sec img:nth-of-type(3) {
  margin-left: 3%;
}

// switch ------------------------
.Section1 .outer {
  position: absolute;
  top: 50%;
  right: -11%;
}

.form-switch {
  transform: rotate(-90deg);
}
.switch {
  position: relative;
  display: inline-block;
  width: 125px;
  height: 40px;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #fafafa;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.slider:before {
  position: absolute;
  content: "مظلم";
  height: 30px;
  width: 60px;
  left: 4px;
  bottom: 4px;
  background-color: white;
  -webkit-transition: 0.4s;
  transition: 0.4s;
  display: flex;
  align-items: center;
  font-weight: 700;
  justify-content: center;
  border: 1px solid #ccc;
  font-size: 12px;
}

input:checked + .slider {
  background-color: #5f5f5f;
}
input:checked + .slider::before {
  content: "مضيئ";
}

input:focus + .slider {
  box-shadow: 0 0 1px #5f5f5f;
}

input:checked + .slider:before {
  -webkit-transform: translateX(54px);
  -ms-transform: translateX(54px);
  transform: translateX(54px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
  border: 1px solid #ccc;
}

.slider.round:before {
  border-radius: 30px;
}
// responsive

@media (max-width: 992px) {
  .fst {
    padding: 0px 4%;
    margin-bottom: 13px;
  }
  .sec {
    padding: 0px 4%;
  }
  .fst img:first-of-type {
    margin-left: 14px;
  }
  .fst img:last-of-type {
    width: calc(70% - 14px);
  }
  .sec img {
    margin-bottom: 13px;
  }
  .sec img:nth-of-type(1),
  .sec img:nth-of-type(3) {
    margin-left: 3%;
  }
  .Section1 .outer {
    right: -20%;
  }
  .Section1 .outer {
    display: none;
  }
}
</style>
