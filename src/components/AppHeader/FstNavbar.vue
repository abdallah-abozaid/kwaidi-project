<template>
  <div class="FstNavbar">
    <div class="container">
      <div class="row">
        <div
          class="col-6 col-md-4 Location d-flex justify-content-start align-items-center order-2 order-md-1"
        >
          <div>
            <div class="dropdown fst">
              <a
                class="btn dropdown-toggle"
                href="#"
                role="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                AR
              </a>

              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">AR</a></li>
                <li><a class="dropdown-item" href="#">AR</a></li>
              </ul>
            </div>
          </div>
          <div>
            <div class="dropdown">
              <a
                class="btn dropdown-toggle"
                href="#"
                role="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                السعودية
              </a>

              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">السعودية</a></li>
                <li><a class="dropdown-item" href="#">السعودية</a></li>
                <li>
                  <a class="dropdown-item" href="#">السعودية</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="Title col-12 col-md-4 order-1 mb-2 mb-md-0 order-md-2">
          <p class="m-0">أهلا بكم في كوايدي</p>
        </div>
        <div class="StartSell col-6 col-md-4 order-2 order-md-3">
          <a href="/"
            >إبدا البيع
            <img
              src="../../assets/arrow-circle-left.png"
              alt="arrow-circle-left"
          /></a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "FstNavbar",
};
</script>
<style lang="scss" scoped>
.FstNavbar {
  background: #3ac2cb;
  padding: 2px 0;
  .StartSell {
    display: flex;
    justify-content: end;
    align-items: center;
    a {
      background: #fff;
      border-radius: 20px;
      font-size: 12px;
      padding: 6px 20px;
      font-weight: 500;
      color: #3ac2cb !important;
    }
    img {
      margin-right: 4px;
      widows: 13px;
      height: 13px;
      display: inline-block;
      margin-bottom: -2px;
    }
  }
  .Title {
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 14px;
    font-weight: 500;
    color: #5f5f5f;
    font-family: "DIN Next LT Arabic bold", sans-serif;
  }
  .dropdown a:hover,
  .dropdown *,
  .dropdown *:hover {
    border: 1px solid transparent !important;
  }
  .dropdown * {
    color: #5f5f5f;
    font-size: 12px;
  }
  .dropdown .dropdown-menu {
    border-radius: 14px;
    background: #fafafa;
    border: 1px solid #f7f7f7 !important;
    padding: 5px 10px;
    li {
      border-bottom: 1px solid rgba(217, 217, 217, 1) !important;
      font-size: 12px;
    }
  }
  .dropdown-toggle::after {
    border-top: 0.35em solid #5f5f5f;
    border-right: 0.35em solid transparent;
    border-left: 0.35em solid transparent;
    vertical-align: 1px;
  }
  .fst {
    position: relative;
  }
  .fst::after {
    position: absolute;
    content: "";
    top: 20%;
    left: 0;
    width: 2px;
    height: 60%;
    background: #5f5f5f;
  }
}
</style>
